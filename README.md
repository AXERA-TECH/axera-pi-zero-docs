# Pulsar2 User Manual

[Web 预览](TODO)

## 1. 项目背景

**爱芯派Zero** (AXera-Pi Zero) 开发板使用手册开源维护项目

- 提供 爱芯派Zero 使用文档
- 方便社区开发者对文档进行共创

## 2. 本地运行指南

### 2.1 git clone

```bash
git clone https://github.com/AXERA-TECH/axera-pi-zero-docs.git
```

目录树如下:

```bash
.
├── LICENSE
├── Makefile
├── README.md
├── build
├── requirements.txt
└── source
    ├── appendix
    ├── conf.py
    ├── doc_update_info
    ├── index.rst
    ├── media
    ├── other_tools
    ├── pulsar2
    ├── user_guides_advanced
    ├── user_guides_config
    └── user_guides_quick
```

### 2.2 编译

安装依赖

```bash
pip install -r requirements.txt
```

在项目根目录下执行以下命令

```bash
$ make clean
$ make html
```

### 2.3 预览

完成编译后，使用浏览器查看 `build/html/index.html` .

## 3. 参考

本项目基于 Sphinx 搭建，关于更多 Sphinx 的信息请见 https://www.sphinx-doc.org/en/master/

## 4. 发版

基于 [ReadtheDocs](https://readthedocs.org/) 平台进行在线代理

