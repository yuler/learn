# css-for-js

> <https://css-for-js.dev/>

## 00 Introduction

> 课程被分 10 个模块, 每个模块 3 ~ 6 个小时

- [agneym/playground](https://github.com/agneym/playground)
- [code-of-conduct](https://courses.joshwcomeau.com/code-of-conduct)
- [Join Discord](https://discord.gg/99sDe5zDVA)

## 01 Fundamentals Recap

### Introduction

> 主要填补一些基础知识的空白

### Anatomy of a Style Rule

- [MDN Introductory Article](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/Getting_started)

### Media Queries

> 网络是一个极其宽广的平台：同样的 HTML 和 CSS 可以在 5 英寸的手机屏幕和 72 英寸的电视上运行！

```css
@media (condition) {

}
```

`@media (max-width: 300px) { ... }` => 屏幕宽度在 **0px ~ 300p** 之间的时候生效
`@media (min-width: 300px) { ... }` => 屏幕宽度在 **> 300px** 的时候生效

### Selectors

> CSS 提供了非常丰富的选择器，而且这些选择器可以以有趣的方式混合和匹配

#### Pseudo-classes

> 伪类可让我们根据元素的当前状态应用 CSS 样式

常用的有 `:hover`, `:focus`, `:checked`

- [MDN Pseudo classes](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)

#### Pseudo-elements

> 伪元素与伪类类似，但它们不以特定状态为目标。相反，它们的目标是元素中的 "子元素"。

常用的有 `::placeholder`, `::before`, `::after`

#### Combinators

> 术语 "组合器" 指的是组合多个选择器的字符

- Descendant combinator
- Child Selector

### Color

- Hex Codes `#FF0000`
- HSL Colors: `hsl(340deg 100% 50% / 0.75)`

### Units

> 与尺寸相关的最常用单位是像素(px)

- `em`: em 它是一个相对单位，等于当前元素的字体大小
- `rem`: rem 单元与 em 单元非常相似，但有一个关键区别：它总是相对于根元素，即 `<html>` 标签, 默认情况下，HTML 标签的字体大小为 16px，因此 1rem 等于 16px
- `percentages`： 百分比单位通常与宽度/高度一起使用，作为占用部分可用空间的方法
- `in`: 媒体印刷

### Typography

#### Font families

- `font-family`: 三种最流行的字体 Serif Sans-serif Monospace

使用 google 网络字体

```html
<link rel="preconnect" href="https://fonts.gstatic.com">
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

使用网络字体的时候, 我们一般用引号包裹起来

```css
html { 
  font-family: 'Roboto', sans-serif;
}
```

我们传递多个值（"font stack"），这样浏览器就可以在最初几秒内（或在字体下载失败时）返回到可用字体。逗号允许我们传递一个有序的字体列表，浏览器将使用第一个可用的字体。

#### Typical text formatting

- `bold`:  默认值是: 400, bold 表示 700
- `italic`: 在 web 端, 斜体通常用于强调、引用、外语词汇、书籍、电影等作品的标题
- `underline`: 在 web 端, 下划线往往表示链接

#### Alignment

`text-align`: left | right | center

#### Text transforms

`text-transform`: uppercase | capitalize

#### Spacing

- `letter-spacing`: 调整字符之间的水平间距
- `line-height`: 建议的最小值为 1.5 (最初，该属性的默认值是 1，但随着时间的推移，默认值在不断上升：在 Chrome 浏览器中，新的默认值是 1.15。在火狐浏览器中，默认值为 1.2。)

### Debugging in the Browser

`Command + Option + I` 打开调试工具
