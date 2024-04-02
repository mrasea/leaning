# 学习笔记

## 安装

使用docker
```
docker pull squidfunk/mkdocs-material
```

### 创建
Unix, Powershell
```
docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material new .
```

Windows
```
docker run --rm -it -v "%cd%":/docs squidfunk/mkdocs-material new .
```

### 配置
```
theme:
  name: material
  
```

## 预览开发

当端口被占用，需要修改端口映射

Unix, Powershell
```
docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
```

Windows
```
docker run --rm -it -p 8000:8000 -v "%cd%":/docs squidfunk/mkdocs-material
```