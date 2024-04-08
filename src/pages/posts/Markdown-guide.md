---
layout: "../../layouts/MarkdownPost.astro"
title: "Markdown 语法指南"
pubDate: 2024-04-07
description: "忘记的时候来看看"
author: "Kaemon"
cover:
  url: "https://jsd.cdn.zzko.cn/gh/AEDELSTAN/picx-images-hosting@master/Pictures/Cover/markdown.86tffktmty.webp"
  square: "https://jsd.cdn.zzko.cn/gh/AEDELSTAN/picx-images-hosting@master/Pictures/Cover/markdown.86tffktmty.webp"
  alt: "cover"
tags: ["代码", "Markdown"]
theme: "dark"
featured: false
---

## 快速跳转

[#标题](#使用号标记标题)&emsp;
[#字体](#字体)&emsp;
[#分隔线](#分隔线)&emsp;
[#删除线](#删除线)&emsp;
[#下划线](#下划线)&emsp;
[#删除线](#删除线)&emsp;
[#脚注](#脚注)&emsp;

<hr>

## 使用#号标记标题

使用 # 号可表示 1-6 级标题

```markdown
# 一级标题

## 二级标题

### 三级标题

#### 四级标题

##### 五级标题

###### 六级标题
```

<hr>

## 字体

Markdown 可以使用以下几种字体：

> _斜体文本_ > **粗体文本** > **_粗斜体文本_**

```markdown
_斜体文本_
_斜体文本_

**粗体文本**
**粗体文本**

**_粗斜体文本_**
**_粗斜体文本_**
```

<hr>

## 分隔线

使用三个或更多个 `*`、`-` 或 `_` 可以创建分隔线

> ---
>
> 大
>
> ---
>
> 家
>
> ---
>
> 好
>
> ---

```markdown
---
---

---

---

---
```

<hr>

## 删除线

使用两个波浪线 `~~` 可以创建删除线

> RUNOOB.COM
> GOOGLE.COM
> ~~BAIDU.COM~~

```markdown
RUNOOB.COM
GOOGLE.COM
~~BAIDU.COM~~
```

<hr>

## 下划线

下划线可以通过 HTML 的`<u>`标签来实现：

> <u>带下划线文本</u>

```html
<u>带下划线文本</u>
```

<hr>

## 脚注

脚注是对文本的补充说明。Markdown 脚注的格式如下:

```markdown
[^要注明的文本]
```

&emsp;  
标注完后一定要记得在其他位置进行解释:

```markdown
[^被标记的文本]：解释内容
```

&emsp;  
实例：  
该博客教程由 Kaemon[^Kaemon]编写

<hr>

## Markdown 列表

Markdown 支持有序列表和无序列表。<br>无序列表使用星号(\*)、加号(+)或是减号(-)作为列表标记：

> - 第一项
> - 第二项
> - 第三项

```markdown
- 第一项

* 第二项

- 第三项
```

##### 或者...

> 1.  第一项
> 2.  第二项
> 3.  第三项

```markdown
1. 第一项
2. 第二项
3. 第三项
```

[^Kaemon]: 作者原英文名是 Kevin，但是有点常见了，所以改成 Kaemon
