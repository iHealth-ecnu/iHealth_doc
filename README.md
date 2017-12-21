## iHealth_doc
iHealth 项目的文档（used by sphinx）

## 使用方法
1. 安装 Sphinx
```
pip install sphinx
```

2. 创建文档目录
```
mkdir xxx_doc
cd xxx_doc
```

3. 使用 Sphinx 初始化该目录
```
sphinx-quickstart
```
初始化过程有一些选项，一般默认就可以，选项都是什么意思可以参考：

[文档整体解决方案(readthedocs、github 、sphinx)使用](https://www.cnblogs.com/youxin/p/3594161.html)

目录创建好之后，结构如下：

```
readthedocs
│ make.bat
│ Makefile
├─build
└─source
　　│ conf.py
　　│ index.rst
　　├─_static
　　└─_templates
```

4. 添加 .gitignore 文件

因为 build 目录存放的是构建好的 html 页面等，我们不提交它们，在 .gitignore 中添加如下信息过滤掉。
```
build
*.pyc
```

5. 项目提交到 github
```
git init
git remote add origin git@github.com:xxx/xxx_doc.git
git add .
git commit -m 'first commit'
git push origin master
```

6. 在 read the docs 中连接 github 托管该项目

## 参考资料
* 如何用 ReadtheDocs、Sphinx 快速搭建写书环境（入门）  
http://www.jianshu.com/p/78e9e1b8553a

* 文档整体解决方案(readthedocs、github 、sphinx)使用（入门2）  
https://www.cnblogs.com/youxin/p/3594161.html

* Sphinx 使用手册（中文，深入学习）  
http://zh-sphinx-doc.readthedocs.io/en/latest/index.html
