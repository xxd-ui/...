#  Day 01
  
  
##  HTML 骨骼架式
  
  
html 标签:网页的根节点  
head 标签: 辅助浏览器解析页面，并不会在页面中展示。  
body 标签：页面的主体部分，用于存放网页要展示的标签。
  
##  HTML 常用标签：
  
  
注释标签：&lt;!-- 注释语句 --&gt;  
文档类型 <!DOCTYPE> ：声明文档类型，告诉浏览器以 HTML5 的标准去解析页面。  
&lt;meta&gt; 标签：设置网页的元数据，不同的属性会使&lt;meta&gt;标签具备不同的功能。  
&nbsp;&nbsp;&nbsp;1. &lt;meta charset="utf-8" /&gt;指定字符集编码 utf-8 (优化后的全球码)  
&nbsp;&nbsp;&nbsp;2. 用于设置关键字 &lt;meta name="keywords" content="xxx" /&gt;  
&nbsp;&nbsp;&nbsp;3. 用于设置描述信息 &lt;meta name="description" content="xxxx" /&gt;  
标题标签：&lt;hn&gt;标题文本&lt;/hn&gt; h1 最大 h6 最小  
段落标签:&lt;p&gt;文本内容&lt;p&gt;  
分割线标签:&lt;hr/&gt;  
换行标签:&lt;br/&gt;
斜体 &lt;em&gt; &lt;i&gt;  
加粗 &lt;strong&gt;&lt;b&gt;  
上标/下标 &lt;sup&gt;&lt;sub&gt;  
下划线/删除线&lt;ins&gt;&lt;del&gt;
转义字符 空格 &nbsp ; 小于号&lt ; 大于号&gt ;  
图像标签: &lt;img src="" alt=""&gt;  
&nbsp;&nbsp;&nbsp;src 属性用于指定图像文件的路径和文件名.  
&nbsp;&nbsp;&nbsp;alt 属性用于指定图片未找到时，显示的内容.
  
###  路径(相对路径和绝对路径)
  
  
相对路径:相对于当前文件  
&nbsp;&nbsp;&nbsp;同一级目录 直接引用图像文件的名称  
&nbsp;&nbsp;&nbsp;上一级目录 在文件名之前加../ ，如果上两级目录，使用 ../ ../  
&nbsp;&nbsp;&nbsp;下一级目录 输入文件夹名和文件名，之间用/隔开
绝对路径:  
本地绝对路径（不用）  
 网络路径（常用）
  
###  链接标签
  
  
&lt;a href="跳转目标" target="目标窗口的弹出方式">文本或图像</a&gt;  
&nbsp;&nbsp;&nbsp;href：用于指定链接目标的 url 地址.  
&nbsp;&nbsp;&nbsp;target：用于指定链接页面的打开方式。  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\_self 为在当前窗口打开（默认值）。  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\_blank 为在新窗口中打开方式。  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\_top 在顶级窗口打开。（不常用）  
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;\_parent 在父类窗口打开。（不常用）  
 ### 列表标签  
 无序列表ul  
 &lt;ul&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项1&lt;/li&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项2&lt;/li&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项3&lt;/li&gt;  
  &nbsp;&nbsp;&nbsp;.......  
  &lt;ul&gt;   
  有序列表ol  
  &lt;ol&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项1&lt;/li&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项2&lt;/li&gt;  
 &nbsp;&nbsp;&nbsp;&lt;li&gt;列表项3&lt;/li&gt;  
  &nbsp;&nbsp;&nbsp;.......  
  &lt;ol&gt;  
  自定义列表  
  &lt;dl&gt;  
 &nbsp;&nbsp;&nbsp;&lt;dt&gt;名词1&lt;/dt&gt;  
 &nbsp;&nbsp;&nbsp;&lt;dd&gt;名词1解释1&lt;/dd&gt;  
 &nbsp;&nbsp;&nbsp;&lt;dd&gt;名词2解释2&lt;/dd&gt;  
  &nbsp;&nbsp;&nbsp;.......    
  
 &nbsp;&nbsp;&nbsp;&lt;dt&gt;名词2&lt;/dt&gt;  
 &nbsp;&nbsp;&nbsp;&lt;dd&gt;名词2解释1&lt;/dd&gt;  
 &nbsp;&nbsp;&nbsp;&lt;dd&gt;名词2解释2&lt;/dd&gt;  
  &nbsp;&nbsp;&nbsp;.......  
  &lt;dl&gt;  
  # HTML基本规范(语法规范)  
    注释不能嵌套
    标签必须完整
    标签可以嵌套，但要注意语义。
    标签的属性必须加双引号
    标签属性尽量使用小写  
###  表格标签  
  
```
<table>
	 <tr>
	     <th>表头内的文字</th>
	     ...
	 </tr>
	 <tr>
	    <td>单元格内的文字</td>
		...
	 </tr>
	...
</table>         
```    
合并单元格:  
rowspan 单元格所占行  
 colspan   单元格所占列
  
  