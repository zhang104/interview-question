#### 1.doctype 的作用是什么？✨

告诉浏览器解析器用 HTML 规范或者 XHTML 规范解析文档

#### 2.标准模式、怪异模式、近乎标准模式有什么区别

1. 标准模式：浏览器 w3c 标准解析执行代码

```
  盒模型：总width = margin + padding + border + width
  行内元素设置宽高不生效
```

2. 怪异模式：浏览器用自己的方式解析执行代码

```
  存在的原因：对非标准的旧网页的兼容
  盒模型：总width = margin + width
```

#### 3.HTML、XHTML、XML 区别

1. HTML: html4.0 之前 --- 超文本标记语言
2. XML: --- 可扩展标记语言
3. XHTML: W3C 为解决 HTML 混乱问题、衍生出后面的 HTML5 --- 可扩展超文本标记语言

#### 4.标签的 data-属性

```javascript
  <div data-text="hh" id="xx"></div>
  <script>
    const elm = document.getElementById("xx")
    const text = elm.data("text")
  </script>
```

#### 5.HTML 语义化 ✨

1. 理解： 用恰当的标签来标记恰当的内容
2. 原因：
   ```
     即使在没有css样式下、能很好的呈现内容结构和代码结构
     有利于代码维护和添加样式
     提升搜索引擎的优化效果
   ```

#### 6.HTML5

1. 文件声明方式<!DOCTYPE HTML>
2. 新增很多标签 video、canvas 等
3. input 新增的 date、email 等属性

#### 7.常用的 meta 标签

```
  <meta charset="UTF-8" >  --- HTML文档的编码形式
  <meta http-equiv="expires" content="Wed, 20 Jun 2019 22:33:00 GMT" /> --- 设置http的缓存过期日期
  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1"> --- 宽度为设备宽度、初始化缩放为1、最大缩放为不缩放
```

#### 8.src 和 href 的区别

1. src: 将指向的资源下载并将内容会嵌入当前标签所在位置 --- 标签：img 、iframe、 js 脚本
2. href: 用来建立和当前元素或文档的连接 --- 标签: a

#### 9.img 中 srcset 的作用

```javascript
  配合sizes使用
  <img src="/files/16864/clock-demo-200px.png"
    alt="Clock"
    srcset="/files/16864/clock-demo-200px.png 200w,
            /files/16797/clock-demo-400px.png 400w,
            /files/16797/clock-demo-600px.png 1x" // 浏览器宽度200px是用/files/16864/clock-demo-200px.png，浏览器宽度400px用/files/16797/clock-demo-400px.png，1x只对固定宽度的img有用
    sizes="(max-width: 600px) 200px, 50vw"  // 最大宽度600px时宽度是200px否则50vw
  />
```

#### 10.cookies、localstorage、sessionstorage、Web SQL、IndexedDB

| hahaha | hehehe | xixixi |
| ------ | :----: | :----: |
| aaa    |  111   |  222   |
| bbb    |  333   |  444   |
| ccc    |  555   |  666   |
