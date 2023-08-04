# 自定义 UI 主题
Narrat 引擎使用标准 Web 工具，即 HTML+CSS+JS 构建游戏，故能使用 CSS 定制游戏元素样式。

本文中一些内容涉及 CSS 基础，不予翻译，请自学。

## 如何在 Narrat 中应用 CSS？
要么直接修改原有 CSS 中的项目，要么自己写 CSS 类并覆盖现有类。

要查看/修改 CSS 设置，请看 main.css 文件。

## 关于图片预加载(preload)的进一步说明
默认情况下，引擎不会加载 CSS 中引用的图像。若要预加载它们，请将其添加到 config.yaml 的 images 列表中。
```CSS
images:
  myButtonBackground: /img/ui/button-background.png
```

> 危险警告！
>
> CSS 中 images(图片)的路径应以"/"开始，如不这样做，构建版本中就不会包含这些资源。
>
> 图片路径如：background-image: url('/images/my-image.png');
>
> 而不能使用: background-images: url('images/my-image.png');

关于自定义字体，请查看[相应文章]()。

## 创建自定义 CSS 类
### 安装
CSS 变量
