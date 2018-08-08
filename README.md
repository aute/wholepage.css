# Why ?

CSS Grid Layout 为 CSS 原本孱弱的二维布局能力带来了极大提升，使 Web 页面的排版可以更加接近于印刷品。另一方面，大量新属性与新规则的加入，难免会让人有些无所适从。考虑到行业中类似 [Bootstrap Grid system](https://getbootstrap.com/docs/4.1/layout/grid/) 的布局书写风格早已被广泛接受，Wholepage CSS 利用了 CSS Grid 属性，并采用 [Bootstrap Grid system](https://getbootstrap.com/docs/4.1/layout/grid/) 布局书写风格来方便你进行二维布局书写。

# Wholepage CSS

Wholepage CSS 是一个暂未开源的主项目的副产物，主项目是一个应用于数据展示大屏的 UI 框架。由于主项目的性质：客户端分辨率固定、信息主要是单向传递（大屏 -> 用户）交互较少，这都是类似印刷品的特点，是 wholepage.css 命名由来，也意味着在近期内 wholepage.css 将专注于固定分辨率下的布局工作，暂不对多分辨率自适应布局提供支持。

# Getting started

### 手动引入

下载已编译的 [Wholepage CSS 文件](https://github.com/aute/wholepage.css/tree/master/dist)。并将位于 `/dist` 的 wholepage.css 文件包含至你的网站或 Web 应用的 <head> 部分。

`<link rel="stylesheet" href="wholepage.css">`

### 使用 NPM 引入

`$ npm install wholepage.css --save`

#Documentation and examples

### Grid system

Wholepage CSS 的网格系统默认占满整个父元素，网格系统为 60*60。传统的一维网格系统往往采用2、3、4 的最小公倍数 12 来进行划分，在大多数客户端（例如：常见的 PC 显示器、手机、Pad）12 列划分已表现良好。但是面对数据展示大屏这类拥有超高分辨率、超宽长宽比的客户端，以 12 进行划分就显得不太够用了，所以 Wholepage CSS 采用 2、3、4、5 的最小公倍数 60 进行划分。

*对于网格数的划分，可以通过覆盖 .scss 文件中的变量进行修改。需要注意的是，随着网格数的增长，编译后的 .css 文件体积也将明显增长*

