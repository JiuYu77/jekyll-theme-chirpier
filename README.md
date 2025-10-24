# jekyll-theme-chirpier

[jekyll-theme-chirpy](https://github.com/cotes2020/jekyll-theme-chirpy)的自定义

# 新特性
- 代码片段左上角的三个圆点使用不同的颜色。
- 优化单行代码颜色。
- 增加显示： 文章数、类别数、标签数。
- 增加分类文章树: 可以在浏览文章时，显示`文章列表`，点击按钮可以显示或隐藏文章列表。

# 模板

[**jekyll-theme-chirpier 主题模板 chirpier-starter**](https://github.com/JiuYu77/chirpier-starter)

# 构建&发布

## 构建（npm + gem）
脚本文件`tools/release.sh` 中定义了构建和发布的命令。
```shell
bash tools/release.sh -p  # 仅构建 gem 包
```

## 发布（gem）

1. `.gemspec` 文件中定义`主题名`和`版本号`等信息，如：
    ```shell
    spec.name          = "jekyll-theme-chirpier"
    spec.version       = "1.0.3"
    spec.authors       = ["Cotes Chung", "JiuYu77"]
    ```
    每次发布时，需要更新`.gemspec` 文件中的`版本号`。
2. 构建。
3. `gem` 命令发布 gem 包：
    ```shell
    gem push 定义的主题名-版本号.gem
    ```
