### JavaScript 的组成
- ECMAScript：JavaScript 的语法标准。包括变量、表达式、运算符、函数、if 语句、for 语句等。

- DOM：文档对象模型，操作网页上的元素的 API。比如让盒子移动、变色、轮播图等。

- BOM：浏览器对象模型，操作浏览器部分功能的 API。比如让浏览器自动滚动。  
### JavaScript 的特点  
- 简单易用：可以使用任何文本编辑工具编写，只需要浏览器就可以执行程序。
- 解释型语言：事先不需要被编译为机器码再执行，逐行执行、无需进行严格的变量声明。
- 基于对象：内置大量现成对象，编写少量程序可以完成目标。
- 面向过程。  
### JavaScript 代码的书写位置  
(1)内嵌的方式：在body标签内嵌入script标签,写在所有html标签之后.   
(2)外链式：引入外部 JavaScript 文件（放到 body 标签里，可以和内嵌的 js 代码并列）   
### JavaScript 输出方式  
- alert()：弹出“警告框”。  
- console.log() ：控制台输出。  
- prompt()：用户输入语句. (prompt语句中，用户不管输入什么内容，都是字符串。)   
### 什么是变量 (储存数据的容器)  
在 JavaScript 中，永远都是用 var 来定义变量（在 ES6 之前）  
变量要先定义，才能使用.  
### 变量的命名规范
1.变量命名必须以字母或是下标符号”_”或者”$”为开头。
2.不能以数字开头
3.不能是 js 中的关键字和保留字
4.严格区分大小写
5.建驼峰命名规则
6.见名知意
### 变量的数据类型  
数据类型： 基本数据类型（原始数据类型） 和 引用数据类型（复杂数据类型）
- 基本数据类型：存放在栈内存（stack）中，可以直接访问。（String 字符串、Number 数值、Boolean 布尔值、Null 空值、Undefined 未定义。）  
- 引用数据类型：属性(键值对)的无序集合,描述事物信息特征.存放在堆内存（heap）中，变量在栈内存中实际保存的是一个指针，这个指针指向堆内存当中对应的数据。 (Object 对象 Array 数组 Function 函数)   
var obj = {  
 &nbsp;&nbsp;&nbsp;    属性名1:属性值1,  
   &nbsp;&nbsp;&nbsp; 属性名2:属性值2,  
  &nbsp;&nbsp;&nbsp;  属性名3:属性值3;
}  
var arr = {1,2,4,7,9};  

 function foo() {
 &nbsp;&nbsp;&nbsp; // 函数要执行的代码
}  
 函数的作用是封装代码
### String 字符串  
转义字符  
- \n 表示换行
- \r 表示回车
- \t 表示制表符
- \b 表示空格
- \\ 表示\  

typeof()表示“获取变量的类型”，返回的是小写.  
- typeof 数值的返回结果：number
- typeof 字符串的返回结果：string
- typeof 布尔型的返回结果：boolean
- typeof undefined的返回结果：undefined
- typeof null的返回结果：object  
### Number 数值  
数值范围：如果使用 Number 表示的变量超过了最大值，则会返回 Infinity。  
NaN 和 isNaN()函数：
（1）NaN：是一个特殊的数字，表示 Not a Number，非数值.  
 注意：
 - typeof NaN的返回结果是 number。  
 - Undefined 和任何数值计算的结果为 NaN。NaN 与任何值都不相等，包括 NaN 本身。

 （2）isNaN() :任何不能被转换为数值的值，都会让这个函数返回 true。  
 ### undefined 未定义  
 声明了一个变量，但是没有赋值（例如：var a;），此时它的值就是 undefined。  
 - Undefined 类型的值只有一个，就是 undefind  
 - 使用 type of 检查一个 undefined 时，会返回 undefined. 

 console.log(isNaN("123")); // false  
 ### null 空值  
 专门用来表示一个为空的对象（例如：var a = null）。注意，专门用来表示空对象。  
 - Null 类型的值只有一个，就是 null。比如：var a = null。
- 使用 typeof 检查一个 null 值时，会返回 object。  
### Object 对象  
Object 对象是一组由键-值组成的无序集合  
### 变量的类型转换  
1.转换为String类型  
- 变量+'' 或者 变量+"abc"  
- 调用 toString()方法 
null 和 undefined 没有toString方法
- 使用 String()函数  

2.转换为Number类型  
- 使用 Number()函数    
 console.log(Number(undefined)); // NaN
        console.log(Number(null)); //0
- 使用 parseInt() 

### parseInt()    
转换规则:   
- 从第一个非空白字符（空格、换行、tab）开始转换，直到遇到一个非数字字符为止。
- 不会四舍五入  取整   
- 如果对非 String使用 parseInt()或 parseFloat()，它会先将其转换为 String然后再操作。
console.log(parseInt('123a')); // 123  
 console.log(parseInt('&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 2019abc')); // 2019    



3.转成布尔值 Boolean()  
 NaN 0 undefined  null  '' 这五种转换为false,其余都是true.  
 ### parseFloat()：  
 var d = "123.456.789px";  
 console.log(parseFloat(d)); // 123.456
### 算数运算符  
注意事项:  
（1）当对非 Number 类型的值进行运算（包括+、-、*、/）时，会将这些值转换为 Number 然后再运算。
（2）任何值和 NaN 做运算的结果都是 NaN。  
（3）任何的值和字符串做加法运算，都会先转换为字符串，然后再做拼串操作。  
### 赋值运算符  
可以将符号右侧的值赋值给符号左侧的变量。  
### 自增和自减  
自增分成两种：a++和++a。  
a++ 加号在后,表示先赋值,再自增.
++a 加号在前,表示先自增,再赋值.  
自减 -- 原理同上。  
### 比较运算符  
非数值的比较  
（1）对于非数值进行比较时，会将其转换为数字然后再比较。  
（2）两个字符串比较时，是一位一位进行比较。 相同则比较下一位("123"<"56" )  .
因此：当我们在比较两个字符串型的数字时，一定要先转型，比如 parseInt()。  
（3）任何值和 NaN 做任何比较都是 false。  
### ==符号的强调  
(1)==这个符号并不严谨，会将不同类型的东西，转为相同类型进行比较.  
(2)undefined 衍生自 null，所以这两个值做相等判断时，会返回 true。  
(3)NaN 不和任何值相等，包括他本身。  
### ===全等符号的强调  
如果要保证完全等于，我们就要用三个等号===。全等不会做类型转换。
