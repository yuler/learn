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
