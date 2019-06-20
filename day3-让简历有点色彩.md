* 网页安全字体指的是几乎在所有操作系统中都存在的字体。以下为5个常用的字体：`serif`, `sans-serif`, `monospace`, `cursive`,和 `fantasy`。
* 字体大小的单位：
  * px：绝对单位，保证不变
  * em：与其父元素大小相关，倍数关系
  * rem：与根元素html大小相关，倍数关系，ie8及以下不支持
* 较好实践：网页默认字体大小为16px。所以将基础文档的字体大小设置为10px，然后使用em/rem。如：

```css
html {
  font-size: 10px;
}

h1 {
  font-size: 2.6rem;
}

p {
  font-size: 1.4rem;
  color: red;
  font-family: Helvetica, Arial, sans-serif;
}
```

* css的属性和属性值区分大小写。
* css文件中除了可以写`规则集`外，还可以写`@-规则(At-rules)`，`嵌套语句`，任何其他语句则会被忽略。

```css
@import 'default.css';
/* 该样式只有当页面宽度大于801px时才会被应用 */
@media (min-width: 801px) {
  body {
    margin: 0 auto;
    width: 800px;
  }
}
```

* `存在和值(presence and value)`属性选择器
  * `[attr]`：该选择器选择包含 attr 属性的所有元素，不论 attr 的值为何。
  * `[attr=val]`：该选择器仅选择 attr 属性被赋值为 val 的所有元素。
  * `[attr~=val]`：该选择器仅选择具有 attr 属性的元素，而且要求 `val` 值是 `attr` 值包含的被空格分隔的取值列表里中的一个。
* `子串值(substring value)`属性选择器
  * `[attr|=val]` : 选择attr属性的值是 `val` 或值以 `val-` 开头的元素（注意，这里的 “-” 不是一个错误，这是用来处理语言编码的）。
  * `[attr^=val]` : 选择attr属性的值以 `val` 开头（包括 `val`）的元素。
  * `[attr$=val]` : 选择attr属性的值以 `val` 结尾（包括 `val`）的元素。
  * `[attr*=val]` : 选择attr属性的值中包含子字符串 `val` 的元素（一个子字符串就是一个字符串的一部分而已，例如，”cat“ 是 字符串 ”caterpillar“ 的子字符串）。
* `data-*` 全局属性：是一类被称为**自定义数据属性**的属性，它赋予我们在所有 HTML 元素上嵌入自定义数据属性的能力，并可以通过脚本(一般指JavaScript) 与 HTML之间进行专有数据的交换。所有这些自定义数据属性都可以通过所属元素的 [`HTMLElement`](https://developer.mozilla.org/zh-CN/docs/Web/API/HTMLElement) 接口来访问。  [`HTMLElement.dataset`](https://developer.mozilla.org/zh-CN/docs/Web/API/HTMLElement/dataset) 属性可以访问它们。



----

* 用时大约3小时。
* 对于data-* 全局属性的应用还不了解。
* 查了下，兄弟选择器为 +。
* 任务链接：[codepen](https://codepen.io/whateverhck/pen/mZENeo?editors=1100) 

