# MkDocs

## 介绍

[官网](https://www.mkdocs.org/)

MkDocs 是一个快速、简单且华丽的静态站点生成器，适用于构建项目文档。文档源文件是用 Markdown 编写的，并使用单个 YAML 配置文件进行配置。首先阅读介绍性教程，然后查看用户指南以获取更多信息。

## 安装

```
pip install mkdocs
```

## 创建

```
mkdocs new my-project
cd my-project
```
以上操作会新建以下结构的文件：
```
.
├─ docs/
│  └─ index.md
└─ mkdocs.yml
```

在开发时可以启动预览服务。
```
mkdocs serve
```
## 生成网站

```
mkdocs build
```