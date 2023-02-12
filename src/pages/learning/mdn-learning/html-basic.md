---
title: HTML Basic
---

# HTML Basic

HTML是*H*yper*T*ext *M*arkup *L*anguage的简称, 即超文本标记语言。

HTML不是一门编程语言，而是一种用于定义内容结构的标记语言。

## HTML元素详解

* 开始标签
* 结束标签
* 内容
* 元素: 开始标签，结束标签与内容相结合，便是一个完整的元素。

元素也可以包含属性，事件等。

## 嵌套元素

## 空元素

不包含任何内容的元素称为空元素。比如`<img>`元素:

```html
<img src="images/firefox-icon.png" alt="My test image" />
```

## HTML文档详解

## 图像

```html
<img src="images/firefox-icon.png" alt="My test image" />
```

## 标记文本

### 标题

```html
<h1>主标题</h1>
<h2>顶层标题</h2>
<h3>子标题</h3>
<h4>次子标题</h4>
```

### 段落

```html
<p>这是一个段落</p>
```

### 列表

1. 无序列表(Unordered Lists)中项目的顺序并不重要，如购物清单。用`<ul>`元素包裹。
2. Ordered lists are for lists where the order of the itmes does matter, such as a recipe. These are wrapped in an `<ol>` element.

For example

```html
<p>At Mozilla, we're a global community of</p>

<ul>
  <li>technologists</li>
  <li>thinkers</li>
  <li>builders</li>
</ul>

<p>working together…</p>
```

### Links

```html
<a href="https://www.mozilla.org/en-US/about/manifesto/">Mozilla Manifesto</a>
```


