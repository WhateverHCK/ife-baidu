* 诸如<center>标签及align, bgcolor, color属性已被标记为`废弃`，应用`样式(css)`代替。如：

```html
<p style="background-color:red;font-size:20px;text-align:center">
  whatever
</p>
```

* 规范起见，所有标签必须要`闭合`，并且使用小写。属性值加双引号，若本身已有，可以用单引号。

* 注释中的`条件注释`：

```html
<!--[if IE 8]>
    .... some HTML here .... 当浏览器为IE时才会执行这里
<![endif]-->
```

* 标记语言的真正威力在于其收集能力，它可以将收集来的文档组合成一个完整的信息库，并且可以将文档库与世界上的其他文档集合链接起来。
* 一般来说，[http://example/foo] 语义上代表着一个文件，[http://example/foo/] 代表着一个目录，具体可见[stackoverflow](https://stackoverflow.com/questions/5948659/when-should-i-use-a-trailing-slash-in-my-url)
* 响应式设计指的是：
  * RWD 指的是响应式 Web 设计（Responsive Web Design）
  * RWD 能够以可变尺寸传递网页
  * RWD 对于平板和移动设备是必需的
*  标签<base>(在<head>标签中定义)可以为页面上所有链接规定默认地址或默认目标(即src, target)。如：

```html
<head>
<base href="http://www.w3school.com.cn/images/" />
<base target="_blank" />
</head>
```

* URL编码

  * URL 只能使用 [ASCII 字符集](http://www.w3school.com.cn/tags/html_ref_ascii.asp)来通过因特网进行发送。
  * 由于 URL 常常会包含 ASCII 集合之外的字符，URL 必须转换为有效的 ASCII 格式。
  * URL 编码使用 "%" 其后跟随两位的十六进制数来替换非 ASCII 字符。
  * URL 不能包含空格。URL 编码通常使用 + 来替换空格。

* html5中的datalist for input

* 输入标签<input>的一些限制属性：

  * pattern: 规定通过其检查输入值的正则表达式。
  * required: 规定输入字段是必需的（必需填写）。
  
* form属性

  * form 属性规定 <input> 元素所属的一个或多个表单。

    **提示：**如需引用一个以上的表单，请使用空格分隔的表单 id 列表。

    输入字段位于 HTML 表单之外（但仍属表单）：

    ```html
    <form action="action_page.php" id="form1">
       First name: <input type="text" name="fname"><br>
       <input type="submit" value="Submit">
    </form>
    
     Last name: <input type="text" name="lname" form="form1">
    ```

---

* 阅读了[w3school]([http://www.w3school.com.cn/html/index.asp](http://www.w3school.com.cn/html/index.asp)) 里的基础教程及表单，大约3小时
* 写简历任务大约20分钟