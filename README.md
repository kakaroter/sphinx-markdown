# sphinx-markdown

## 一、简介

使用开源的sphinx工具搭建markdown格式的html网站博客

## 二、环境安装

在项目根目录下执行 以下命令安装环境

```shell
bash env.sh
```

## 三、创建项目文档

### 1、创建项目目录

```shell
mkdir sphinx-test
cd sphinx-test
```

### 2、快速启动并配置

![img](file:////tmp/wps-qjx/ksohtml/wpsm3VWjQ.png)

### 3、配置完成后结构如下

![img](file:////tmp/wps-qjx/ksohtml/wpsYDALag.jpg)

### 4、编辑conf.py

```shell
extensions = ['recommonmark','sphinx_markdown_tables']
html_theme = 'sphinx_rtd_theme'
```

![img](file:////tmp/wps-qjx/ksohtml/wpsdo97sz.png)

### 5、将写好的test.md 放到 source目录下

```shell
cp test.md souce
```

### 6 、编辑index.rst添加test.md

![img](file:////tmp/wps-qjx/ksohtml/wpsqyhhxx.png)

### 7、生成静态html网页文件

```shell
make html
```

### 8、查看index/html

```shell
cd build/html/index.html
```

### 9、md文档更新后需要清空后重新生成html

```shell
make clean
```

### 10、在本机启用http服务

```shell
python3 -m http.server 8080
```

### 11、在局域网中的浏览器查看web

```shell
http://10.20.xx.xx:8080
```

