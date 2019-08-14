# projects 通用模板

## 项目初始化

在终端输入：

```sh
mkdir data draft models outputs utils notebook
```

进行项目的初始化。

## `.gitignore` 的模板

更多内容参考：[ xinetzone/gitignore](https://github.com/xinetzone/gitignore)
在 [demo/](demo.gitignore) 中放置了一些常用的 `gitignore` 文件。

## 项目的输出与中间结果存储目录

该项内容仅仅在本地磁盘创建，而不被上传到 github：

- `data/`: 数据的存放
- `models/`: 模型的参数存储
- `output/`: 模型的输出结果

## 项目的开发

- `utils/`：存放相关的 API
- `notebook/`：存放 jupyter notebook 等相关的文件
- `draft/`：(可以放置在任何位置)存放一些不成熟的或者未开发完成的一些相关内容，不被上传到 github

## nutsml

一个数据处理工具包 [nutsml](https://maet3608.github.io/nuts-ml/introduction.html)：

Deep-learning code is characterized by

```te
    data pre-processing on CPU and training on GPU
    mix of common and task-specific pre-processing steps
    training in epochs
    mini-batches of training data
    data transformation such as scaling, cropping and others
    data augmentation to increase amount of training data
    check-pointing of network weights
    logging of training progress
```
