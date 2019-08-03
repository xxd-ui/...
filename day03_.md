# 盒子模型
content(内容) ,padding（内边距）、border（边框）、margin（盒子与盒子的距离）  
### padding   会改变元素的大小。
	padding:10px; 			        上左右下。
	padding:10px 20px; 			上下、左右。
	padding:10px 20px 30px; 		上、左右、下。
	padding:10px 20px 30px 40px;		 上、右、下、左
	padding-top、padding-left、padding-right、padding-bottom 分别用来指定四个方向的内边距。  
 ### margin     (透明 其他是有颜色的)  
   设置方法和padding类似
	margin: xxx auto;可以使块状元素水平居中。  
### 嵌套崩塌： 
两个盒子发生嵌套的时候，给子类设置 margin 会给父类造成一种崩塌现象，子类元素的 margin-top 没有效果，而是直接作用到父类元素。  
  解决方案：
		1. 父类 overflow: hidden;
		2. 父类 设置极小的 padding 或者 border；  
 ### margin重叠：
如果垂直方向上两个块状元素同时设置了 margin-bottom 和 margin-top，那么这两个值将会发生重叠，不会累加，哪个值大用哪个。  
margin-top/margin-bottom 对于行内元素无效。
### border 	会改变元素的大小。
border:1px solid red; 分别指定了边框的宽度、样式和颜色.
	border-style: none (默认) / dashed(虚线) / dotted（点） / solid(实线) / double(双实线)/transparent(透明)
	可以单独设置某一条边框：border-right: 20px solid blue;
	利用border画三角形.  
### 显示和隐藏  
display:none; 	隐藏(消失)元素，不再在文档中占据位置。
	visibility:hidden; 	隐藏元素，隐藏后其在文档中所占的位置会依然保持，不会被其他元素覆盖。  
### hover  
 鼠标悬停时的状态
	显示 display:block;(只要不是none,就会显示)
	        visibility:visible;  
### overflow  
指定标签里面的内容超出了样式的宽度和高度时如何处理。
	visible：默认值
	scroll：添加滚动条
	auto：根据需要添加滚动条
	hidden：隐藏超出盒子的内容  
### 浮动  
 使元素脱离原来的文本流，在父元素中浮动起来。
	float:none 	 不浮动
	float:left 		向左浮动
	float:right 	向右浮动  
### 浮动的表现形式  
- 当一个元素浮动以后，其下方的元素会上移。元素中的内容将会围绕在元素的周围。
- 浮动会使元素完全脱离文本流，也就是不再在文档中在占用位置。
- 元素设置浮动以后，会一直向上漂浮直到遇到父元素的边界或者其他浮动元素。
- 元素浮动以后即完全脱离文档流，这时不会再影响父元素的高度。也就是浮动元素不会撑开父元素。
- 浮动元素默认会变为块元素，即使设置 display:inline 以后其依然是个块元素。
- 块级元素和行内元素都可以浮动，当一个行内元素浮动以后将会自动变为一个块级元素。
- 当一个块级元素浮动以后，宽度会默认被内容撑开，所以当漂浮一个块级元素时我们都会为其指定一个宽度。