# 使用conda创建一个环境

---

## 为什么

在以后的时光里，你会接触到很多不同的深度学习方法和子领域。但是只要你还在用python，你就脱离不了大量的包和依赖。并且，在不同的深度学习项目中，往往要使用不同包甚至相同包的不同版本。你肯定不想每次创建或切换项目都重新打点一次你的包版本和依赖。

好消息是你可以使用工具来管理你的环境，也就是说，你可以在一台电脑上创建多个人不同的环境，就像是虚拟机，需要用哪个就激活哪个。这样能够大大节省不必要浪费掉的时间，让你全心全意投入学习和工作。

---

## 安装anaconda

anaconda是可靠的知名虚拟环境管理工具。你可以在[anaconda的官网](https://www.anaconda.com/)找到和下载安装包，并根据提示进行安装。

- 提示：在windows和mac上，你可以直接下载应用程序安装程序或镜像文件；在linux上，你可以更方便的使用包管理器来完成anaconda的安装。当然，anaconda也是有替代品的，比如更小巧的miniconda。

---

## 切换源

就像linux的包管理器一样，anaconda不但是个虚拟环境管理器，也是个包管理器。源可以理解为包管理器下载包的远程服务器。源有很多个，就像你下载软件时可能会有国内的下载站或是国外的下载站。由于中国大陆地区网络的特殊性，这里建议你**切换到国内源来提高包的下载速度**。

国内较为出名的公有源有清华源和中科大源。你可以通过下面的命令行将它们添加到你的conda源：

```bash
# 添加清华源
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge 
conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
```

```bash
# 添加中科大源
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/main/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/pkgs/free/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/conda-forge/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/msys2/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/bioconda/
conda config --add channels https://mirrors.ustc.edu.cn/anaconda/cloud/menpo/
```

你还可以通过下面这行命令让conda在搜索到包时显示它是在哪个源找到的：

```bash
conda config --set show_channel_urls yes
```

出了通过命令直接修改这些信息，你也可以修改anaconda的配置文件。详情可以自行探索。

---

## 创建环境

创建一个名称为mxnet的环境，并指定这个环境的python版本为3.8

```bash
conda create -n mxnet python=3.8
```

---

## 安装apache mx-net

- mx-net简介

  Apache MXNet（孵化）是一个深度学习框架，旨在提高效率和灵活性。它允许您混合符号和命令式编程，以最大限度地提高效率和生产力。MXNet的核心是一个动态依赖调度程序，可以动态地自动并行化符号和命令操作。最重要的图形优化层使符号执行更快，内存效率更高。MXNet便携且轻巧，可有效扩展到多个GPU和多台机器。

  更多的特点请参考[mx-net官网](https://mxnet.apache.org/versions/1.7.0/)。你也可以看到[mx-net的开源项目仓库](https://github.com/apache/incubator-mxnet)

- 使用conda安装

  ```bash
  
  ```

- 使用pip安装

### 为什么使用conda的时候要使用pip？

- 在同个环境下，pip和conda不会冲突

### pip换源

和conda同理，**将pip切换至国内源可以提高包的下载速度**。你可以从下面的命令行中选择一条来执行。

```bash
# 阿里源
pip config set global.index-url https://mirrors.aliyun.com/pypi/simple/
# 清华源
pip config set global.index-url https://pypi.tuna.tsinghua.edu.cn/simple
# 腾讯源
pip config set global.index-url http://mirrors.cloud.tencent.com/pypi/simple
# 豆瓣源
pip config set global.index-url http://pypi.douban.com/simple/
```

在这里推荐截止到本文写作日期时表现更加稳定的阿里源。

