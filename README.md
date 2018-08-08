# Why ?

CSS Grid  Layout 为 CSS 原本孱弱的 2 维布局能力带来了极大的提升，使 web 页面的排版可以更加接近于印刷品。另一方面，大量新属性与新规则的加入，难免会让人有些无所适从。考虑到行业中类似 [Bootstrap Grid system](https://getbootstrap.com/docs/4.1/layout/grid/) 的布局书写风格早已被广泛接受，Wholepage CSS 利用了 CSS Grid 属性，并采用 [Bootstrap Grid system](https://getbootstrap.com/docs/4.1/layout/grid/) 布局书写风格来方便你进行 2 维布局的书写。

# Wholepage CSS

wholepage.css 是一个暂未开源的主项目的副产物，主项目是一个应用于数据展示大屏的 UI 框架。由于主项目的性质：客户端分辨率固定、信息主要是单向传递（大屏 -> 用户）交互较少，这都是类似印刷品的特点，这是 wholepage.css 命名由来，也意味着在近期内 wholepage.css 将专注于固定分辨率下的布局工作，暂不对多分辨率自适应布局提供支持。

# Getting started

### 手动引入

下载已编译的 [Wholepage CSS 文件](https://github.com/aute/wholepage.css/tree/master/dist)。并将位于 `/dist` 的 wholepage.css 文件包含至你的网站或 Web 应用的 <head> 部分。

`<link rel="stylesheet" href="wholepage.css">`

### 使用 NPM 引入

`$ npm install wholepage.css --save`
