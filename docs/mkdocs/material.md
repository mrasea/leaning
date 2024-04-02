# Material for MkDocs主题

## 安装


=== "使用pip"

    ```
    pip install mkdocs-material
    ```

=== "使用docker（推荐）"

    ```
    docker pull squidfunk/mkdocs-material
    ```

## 创建

=== "使用pip"

    ```
    mkdocs new .
    ```

=== "Unix, Powershell"

    ```
    docker run --rm -it -v ${PWD}:/docs squidfunk/mkdocs-material new .
    ```

=== "Windows"

    ```
    docker run --rm -it -v "%cd%":/docs squidfunk/mkdocs-material new .
    ```
## 配置
```
theme:
  name: material
  
```

## 预览开发

=== "Unix, Powershell"

    ```
    docker run --rm -it -p 8000:8000 -v ${PWD}:/docs squidfunk/mkdocs-material
    ```

=== "Windows"

    ```
    docker run --rm -it -p 8000:8000 -v "%cd%":/docs squidfunk/mkdocs-material
    ```

当端口被占用，需要修改端口映射

## 生成网站

[生成网站](./index.md)