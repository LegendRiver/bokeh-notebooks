## 克隆或者下载
首先，下载教程到本地：

```
$ git clone https://github.com/bokeh/bokeh-notebooks.git
```

或者从这个地址下载：https://github.com/bokeh/bokeh-notebooks/archive/master.zip

## 安装依赖包

这个教程经过如下版本测试：

* bokeh 0.12.7
* pandas 0.20.3
* notebook 5.0.0
* phantomjs 2.1.1
* pillow 4.2.1
* selenium 3.5.0

其它组合也可能可以工作。

最快最容易的方法是使用 Anaconda (或者 Miniconda):

#### 使用 anaconda 安装

安装 [anaconda](http://anaconda.com/downloads)

Anaconda 应该已经包括了所有需要的包，但是可能需要更新其版本。

#### 使用 miniconda 安装

安装 [miniconda](http://conda.pydata.org/miniconda.html).

使用如下命令创建一个环境并且安装包：

注意：在 `tutorial` 目录（有 `environment.yml` 文件的）运行这些命令。

```bash
$ conda env create
$ source activate bokeh-notebooks
```

----

以上安装好了后，接着安装剩下的依赖包：

```bash
conda install phantomjs pillow selenium
```

## 获取示例数据

Bokeh 有一些示例数据可下载，用于展示可视化效果。使用如下命令获取：

```bash
$ bokeh sampledata
```

### 安装 Datashader 和 Holoviews (可选)

有些可选章节需要附加的包 Flask，Datashader 和 Holoviews。

```bash
$ conda install -c datashader holoviews flask
```

## 运行 Jupyter notebook

从这个目录运行 jupyter notebook，然后打开 [00 - Introduction and Setup.ipynb](00 - Introduction and Setup.ipynb)。

```
$ jupyter notebook
```
