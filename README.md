# AXera-Pi Zero User Manual

[Web 预览](https://axera-pi-zero-docs-cn.readthedocs.io/zh-cn/latest/index.html)

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
    ├── conf.py
    ├── doc_appendix.md
    ├── doc_guide_advanced.md
    ├── doc_guide_quick_start.md
    ├── doc_introduction.md
    ├── doc_update_info.md
    ├── index.rst
    └── media
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

