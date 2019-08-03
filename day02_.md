### 表单:  
由表单控件（也称为表单元素）、提示信息和表单域 3 个部分构成.
表单控件:包含了具体的表单功能项，如单行文本输入框、密码输入框、复选框、提交按钮、重置按钮等。  
 提示信息：一个表单中通常还需要包含一些说明性的文字，提示用户进行填写和操作。  
 表单域：相当于一个容器，用来容纳所有的表单控件和提示信息，可以通过他定义处理表单数据所用程序的 url 地址，以及数据提交到服务器的方法。如果不定义表单域，表单中的数据就无法传送到后台服务器。

### input 标签

type 值:

- text 单行文本输入框
- password 密码输入框
- radio 单选按钮 (需要设置 name 一样)
- checkbox 复选框
- button 普通按钮
- submit 提交按钮
- reset 重置按钮
- img 图像形式的提交按钮
- file 文件域

name:由用户自定义 控件的名称  
 value:由用户自定义 input 控件中的默认文本值.

### lable 标签:

用于绑定一个表单元素, 当点击 label 标签的时候, 被绑定的表单元素就会获得输入焦点。

### textarea 文本域: 创建多行文本输入框

```
<textarea cols="每行中的字符数" rows="显示的行数">
 	 文本内容
</textarea>
```

### 下拉菜单:

```
<select>
	<option>选项1</option>
	<option>选项2</option>
	<option>选项3</option>
	...
</select>
```

### 表单域:

```
<form action="url地址" method="提交方式" name="表单名称">
	各种表单控件
</form>
```

&lt;fieldset&gt;&lt;legend&gt;可以实现表单的分组。
get 提交 post 提交  
disabled 禁用  
readonly 只读  
multiple 多文件上传  
checked 单选框的默认选中  
selected 下拉框的默认选中
autofocus 自动或者光标  
placeholder 默认显示的内容

### 标签的常见属性:

id 这个标签的唯一标识,页面内不能重复  
 class 类 类名可以重复,可以有多个  
 title 鼠标悬停时显示的属性

# CSS

### 书写位置:

```
行内样式 <p style="color: red; font-size: 24px;">这是一个p标签</p>
内部样式 <style>p{color: red;font-size: 24px;}</style>
外部引入 <link rel="stylesheet" href="style.css">
```

### 区别:

行内样式：严重耦合，用的很少。  
内部样式：测试使用，当前页面的样式只能当前页面使用。  
外部样式：上线使用，多个页面可以复用样式。

### \*CSS 选择器

简单选择器:

- 标签选择器 p{}
- id 选择器 #p1{}
- class 选择器 .user{}  
  复杂选择器:
- 后代选择器 (常用 空格隔开)
- 交集选择器 (没有空格)
- 并集选择器 (同时选中多个标签,逗号隔开)
- 通配符

### CSS 继承性的总结: www.cnblogs.com/thislbq/p/5882105.html

CSS 层叠性: 样式冲突,必然只有一个样式生效  
CSS 权重问题: 行内样式 1000> id 选择器 100> class 选择器 100 >标签选择器 10>通配符/继承属性 0
CSS  
常见单位:

- px 像素单位
- 百分比
- em 基于当前字体的倍数
- 颜色  
  预定义颜色  
   十六进制  
   rgb: rgb(0,0,255) ==> 绿色。  
   rgba: rgba(0,0,255,0.5)。a 是透明度：0~1

### CSS 常用属性:

 ![](img/001.png)

### 标签的表现形式:

块状标签:独占一行，宽高有效。比如：div p h1~h6 form table hr br ul>li ol>li dl>dt/dd  
 行内块标签：可以同一行显示，宽高有效。比如: input select img button  
 行内标签：可以同一行显示，但是宽高无效。比如：a span strong del ins em i b  
 转换的必要性：比如可以把 a 标签转换为块状元素，设置宽高，使用户可点击的区域增大，进而实现一个按钮的样式。

### 背景图片属性:
 ![](img/002.png)
