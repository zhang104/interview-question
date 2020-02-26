#### 1.doctype的作用是什么？✨
  告诉浏览器解析器用HTML规范或者XHTML规范解析文档
#### 2.标准模式、怪异模式、近乎标准模式有什么区别
  1. 标准模式：浏览器w3c标准解析执行代码
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
  HTML: html4.0之前 --- 超文本标记语言
  XML: --- 可扩展标记语言
  XHTML: W3C为解决HTML混乱问题、衍生出后面的HTML5 --- 可扩展超文本标记语言
#### 4.标签的 data-属性
  ```javascript
    <div data-text="hh" id="xx"></div>
    <script>
      const elm = document.getElementById("xx")
      const text = elm.data("text")
    </script>
  ```



