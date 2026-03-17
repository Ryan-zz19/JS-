js介绍：
变量 
常量
数据类型
类型转换
算术运算符
实战案例

1.js是什么
a.一种运行在客户端的编程语言，实现人机交互的结果

b.作   用：
  a.网页特效（监听用户的一些行为让网页做出对应的反馈）
  b.表单验证（针对表单数据的合法性进行判断）
  c.数据交互（获取后台数据，渲染到前端）
  d.服务端编程（node.js）
  
c.js的组成（有什么？）
ECMAScript：规定了js基础语法核心知识
比如：变量、分支语句、循环语句、对象等等
web api：
DOM操作文档，比如对页面元素进行移动、大小、添加删除等操作
BOM操作浏览器，比如页面弹窗，检测窗口宽度、存储数据到浏览器等等
一些基础知识可以搜MDN



2.js书写位置
css 位置：1.行内 2.内部 3.外部  样式表
js位置：1.行内 2.内部 3.外部 样式表

js行内部样式表：
写在</body>前面
写在最下面的原因是 按顺序执行 

外部样式表：
<body>
  <script src="my.js"></script>
</body>

行内样式表：
写在表签内部
<button onlick="alter('逗你玩的--')">点击我月薪过万</button> 后面vue会用这种模式

注意事项：
练习：
1.<script src="my.js">   js.   alter('你好，js')
  
</script>

2.<script>
 alter（'你好，js'）
</script>

注释/结束符
单行注释：
符号：//
作用：//右边这一行代码会被忽略

块注释：
符号：/* */
作用：在/* 和 */之间的所有内容都会被忽略

结束符：；要么每局都写 要么每局都不写

总结：js 有单行注释 和多行注释 //和/* */

1.5 js输入输出语法
什么是语法 ：
人和计算机打交道的规则约定
我们要按这个规则去写
比如：你吃了吗
我们操作计算机 需要计算机能够看懂

语法1：document.write（'wshi'）
       document.write(;;shd)
       document.write(<h1></h1>)
作用：向body内输入内容
注意输出的内容写的是标签，也会被解析成网页元素

语法2：alter（‘要出的内容’）
作用：页面弹出警告对话框

语法3:console.log('kankanduibudui1')
作用：控制台输出语法，程序员调试使用

语法4：
prompt（'请输入您的姓名'）
作用：显示一个对话框，对话框中包含一条文字信息，用来提示用户输入文字
练习题：
a.浏览器弹出对话框 alter（'nihao,js'）
b.页面打印输出：document.write('shhdj')
                document.write(<h1>266</h>)
c.页面控制台输出：console.log('ta-sjs')    

js执行代码的顺序：
按html流顺序执行
alter（） 和 prompt（）他们会跳过页面渲染先被执行

字面量：
在计算科学当中 字面量 是计算机中描述 事/物
‘’ 1000 【 】 {} 这些都是字面量

总结输入输出语句：
输入：prompt（）
输出：alter（） document.write（） console.log（）




2.变量：
变量是什么；
变量的基本使用；
变量的本质
变量命名规则与规范

变量是什么？
用户输入的数据我们如何存储起来？
答：变量
白话：变量就是装东西的盒子
通俗：变量是计算机中用来存储数据的容器，它可以让计算机变得有记忆
注意：变量不是数据本身，它仅仅是一个用于存储数值的容器。可以理解为一个哥用来装东西的纸箱子

变量是怎么理解的：
装数据的容器 变量是容器不是数值

基本使用：
1.声明变量：
let 变量名
关键字 变量名
变量赋值 =
变量=字面量
申明变量的时候直接完成赋值操作，这种操作也被称为1 变量初始化
=赋值运算符 

变量的基本使用：
目标：1.掌握变量的更新 2.声明多变量的写法
更新变量：
变量赋值之后 还可以接着赋值来更新它
eg：let age = 18；
age=19；
console。log（age） 19

let age = 19
let uname =18
console.log(age,uname)

用户输入：
prompt（）
内部处理保存数据
let 。。。
打印输出
document.write（）

交换变量的值
num 1 = 10；
num 2= 20；
思路：临时变量 做中间存储
let num1 = 10
let num2 = 20
let temp
//把右边的值给左边
temp = num1；
num1 =num2；
num2 = temp

变量：计算机存储数据的地方 相当于是一个空间
本质：是程序在内存中申请的一块用来存放数据的小空间
let age age就是函数的名字

函数变量名：
规则(法律方面)：不能用特殊的let int啥的
不能用数字 不能用下划线啥的 哦哦还有区分大小写
规范（道德方面）：
小驼峰命名法：第一个单词首字母小写 后面每个单词首字母大写 eg：userName
let uname = prompt（'请输入姓名'）
let age = prompt('请输入年龄')
let gender = prompt（"请输入性别"）
document.write(uname,age,gender)

let 和var 的区别：
var 就是一个bug 不要用它就对了

变量一次能够存几个值 我像保存5个人的姓名怎么办

数组：一种讲一组数据存储在单个变量名下的优雅方式
let arr =[] 数组字面量
let 数组名=[数据1，数据2，数据3]
声明数组 有序 
使用数组：索引号 0123
console.log（arr[0]）
数据的编号也叫索引 或下标
数组可以存储任意类型的数据

数组取值的案例：
let 

术语：
元素：数组中保存的每个数据都叫数组元素
下标：数组中的数据编号
长度：数组中数据的个数，通过数组的length属性获得


常量
1.不允许修改数值
2。声明了必须赋值

数据类型：（给数据分类）
1.基本数据类型 {
number数字型 整数 小数 正数 负数 统称：数字类型
string
boolean
undefined
null
}
2.引用数据类型
js：若数据类型 得赋值才知道是啥数据类型 java强数据类型
算数运算符：
+ = * / % 计算顺序：先乘除 取余 再加减
题：给袁半径出面积
//1.页面弹出对话框
let r = prompt（'qingshuru'）

2.计算面积
  let re = 3.14*r*r
  3.页面输出
  document.wirte（re）
  NaN：计算错误
  粘性

  数据类型：字符串类型（string）
  '' "" ``这些包裹的数据都叫字符串
  let tel = '1234'
  console.log('str') 
  console.log(tel)
  console.log('tel')
  变量不能加引号 加了之后就变成字符串了
  注意：无论是单引号还是双引号 必须成对使用 而且 单双引号必须相互嵌套 不能自己套自己
  单引号会找离自己最近的进行比配
  内双外单 外单内双
  + 数字相加 字符相连
console.log(1+1)
console.log('pink'+'laoshi')
let age = 18
docuemnt.write('我今年18岁')
document.write('我今年'+age+'了')
模板字符串：
`` ${}
作用：拼接字符串与变量
let age 18
document.log（`我今年${age}岁了`）
''"" ``字符串数据 字符串拼接可以用模板字符串
let uName = prompt('亲输入您的姓名：')
let age = prompt（'请输入您的年龄：'）
document.write(`大家好，我叫${uName},我今年贵庚${age}岁了`)

数据类型boolean类型：
表示肯定和否定在计算机中对应的是布尔类型数据
true false 是布尔型的字面量
let isCool = true
console.log（isCool）

数据类型 undefined类型：
未定义类型是一个比较特殊的类型
只有一个值为undefined
通常在变量声明不赋值的情况下会说明
使用场景：
let age
console.log（age）
我们在开发过程中经常声明一个变量 等待传送过来的数据
如果我们不知道 这个数据能否传递过来 此时我们可以通过检测这个变量是不是undefined 就判断用户是否有数据传递过来

数据类型null 空 无 
let obj = null
与undefined区别：
undefined 表示没有赋值
null表示赋值了，但是内容为空
console.log（null+1）1
console.log（undefined+1）false
定义变量没给值就是undefined
如果变量是undefined 就说明值没有传递过来

数据类型检测数据类型
控制台输出语句：
let age = 18
关键字typeof来检测数据类型
let num = 10
console.log（typeof num） 数字结果
let str = 'pink'
console.log（typeof str）
let str1 = '10'
console.log(typeof str1)
let flag = false
console.log(typeof flag)
let un
console.log(typeof un)
let obj = null
console.log(typeof null) object

单选框多选框提示框 默认的变量值1都是字符串 此时就不能直接简单的进行加法运算
js 弱数据类型语言 它只有赋值了才清楚
console.log（'10000'+'2000'）//输出结果100002000
把一种数据类型的变量转换成我们需要的数据类型
1.隐式转换 2.显示转换
某些运算符在执行时，系统内部自动将数据类型进行转换，这种转换称为隐式转换
规则：
+两边只要有一个是字符串 都会把另外一个转成字符串
除了+以外的算数运算符 比如-*/等都会把数据转化成数字类型

注意：+作为正号解析可以转成数字型
//console.log（+12）
//console.log（+'123'）//转为数字型   这些都叫做隐形转换
任何数据和字符串相加结果都是字符串

隐形转换规律不清晰 因此显性转换
：自己写代码告诉系统该转成什么类型
转成数字类型
Number（数据）
let str = '123'
console.log(Number('str')) 123
console.log(Number(''pink))NaN
let num = prompt('请输入年薪')
console.log(Number(num))
or
let num = Number(prompt('请输入年薪'))
console.log(Number(num))
Number(数据)
转成数据 字符串内容里有非数字 转换失败 结果为NaN 
parseint（数据）
只保留整数
parseFloat（数据）
可以保留小数
console.log（parseInt（'12px'）） 12
字符串转化为数字型 同时只保留整数
console.log(parseInt('12.83'))  12
console.log(parseFloat('abd12.23'))NaN
显式转换：Number parseInt parseFloat
1.用户输入
let num1 =prompt（'请输入第一个数字'）
let num2 =prompt（'请输入第二个名字'）
//2.输出
alter(num1 + num2)

let num1 = +prompt（'请输入第一个数：'）
let num2 = +prompt（'请输入第二个数：'）
alter(`两个数相加的和是：${num1 + num2}`)

实战：输入订单用户和地址 还有各种信息  然后打印
<h2>订单确定</h2>
<table>
  <tr>
    <th>商品名称</th>  
     <th>商品价格</th>  
     <th>商品数量</th>  
    <th>总价</th>
    <th>收获地址</th>  
  </tr>
  <tr>
  <td>小米青春版PLUS</td>
  <td>1999元</td>
  <td>10</td>  
  <td>100</td>  
  <td>武汉黑马</td>  
    
  </tr> 
</table>   
<style>
  table {
    border-collapse:collapse;
    height:80px;
    margin:0 auto;
    text-align:center
  }
  th {
    padding:5px 30px;
  }
  table,th,td {
    border:1px solid #000;
  }
</style>

1.用户输入
let price = +prompt('请输入商品价格：')
let num = + prompt('请输入商品数量：')
let address = +prompt('请输入收获地址：')
2。计算总额
let total = price*num
3.页面打印渲染
document.write(`
 <table>
  <tr>
    <th>商品名称</th>  
     <th>商品价格</th>  
     <th>商品数量</th>  
    <th>总价</th>
    <th>收获地址</th>  
  </tr>
  <tr>
  <td>小米青春版PLUS</td>
  <td>1999元</td>
  <td>10</td>  
  <td>100</td>  
  <td>武汉黑马</td>  
    
  </tr> 
</table>   
`)
i++ ++i
赋值运算符 自增运算符 前置运算符 后置运算符
let i= 1
console.log(i++ + ++i +i)  7

比较运算符：
能使用常见的比较运算符进行比较运算
> < >= <= == 两边值是否相等 ===左右两边是否类型和值都相等
console.log（2 =='2'）true
console.log(2 ==='2') false
//以后判断是否相等 请用 ===
console.log(NaN ===NaN) NaN不等于任何人 包括它自己
// 开发过程中判断是否相等 强烈建议===
if(num = 2){

}
这个是赋值 永远也不可能有条件
if（num === 2）{

} //这种可以


字符串比较：
ASCII字符代码表

尽量不比小数 小数含精度的问题
不同类型之间比较会发生隐形转换
最终把数据隐式 转成number类型在比较
所以在开发中 我们都用 === 或者！==

= == ===
比较结果 true false

逻辑运算符
：判断一个变量是否大于5且小于10
num >5 && num <10
逻辑运算符：
用来判断多种条件
&& 并且 一假则假 
|| 或者 一真则真
！非取反
let num = 2
console.log（num >5 && num >10）

运算符优先级：
运算符：
1.（）
2.++ -- ！
3.算数运算符：先*/ % 后+ —
4.关系运算符：< >= <=
5.相等运算符：== ！= === ！==
6.逻辑运算符：先&& 后||
7.赋值运算符：=
8.逗号运算符：，
&&优先级比||高

表达式和语句：
表达式：应为表达式可被求值 所有它可以写在赋值语句的右侧
语句：而语句不一定有值 所以比如alter（） for 和break 等语句就不能被用于赋值
语句 ：alter（）弹出对话框 console.log（）控制台打印输出


程序三大流行语句：
顺序结构：
分支结构）（有条件）三角
循环结构：一直执行 反复执行

分支语句：
if分支   三元运算符  swich语句
单分支
if（条件）{
  满足条件执行
}

除了0所有的数字都是真
除了‘’所有的字符串都是真
用户输入
let sore = +prompt（‘请输入成绩’）
进行判断
if（score >=700）{
alter('恭喜考入黑马程序员')
}

双分支if语法“
if（条件）{
满足条件执行语句
}
else（条件）{
满足条件执行语句
}

多分支if语法：
适合有多个结果的时候，比如学习成绩分为：优 良 中 差  多选一
if（条件）{
代码1
}
else if（）{
代码2
}
else if（）{
代码3
}
else（）{
代码n
}

用户输入：
let score = +prompt（‘请输入成绩：’）
判断输出
if（score >= 90）{
alert('成绩优秀，宝贝，你是我的骄傲')
}
else if(score >= 70){
alert('成绩良好')
}
else if（score >= 60）{
alert('成绩良好')
}
else{
alert('成绩不及格 完蛋了')
}
if（数字只有0是假的）
if（字符串只有空是假的）

分支语句之三元运算符：
场景：比if双分支更简单的写法 可使用三元表达式
符号：？与：配合使用
语法：
条件？满足条件执行的代码 ： 不满足条件执行的代码（两刀三段）
console.log( 3>5 ? 3:5)
if(3 >5){
alert('假的')
}
else{
alert('真的')
}
3<5 ? alert('真的') ： alert('假的')
一般来取值：
let sum = 3<5 ? 3:5
console.log(sum)
//用户输入两个数 控制台打出最大的数
//1.用户输入
let num1 = +prompt（‘请输入您的第一个数’）
let num2 = +prompt（‘请输入您的第二个数’）
判断输出-三元运算符
num1 >num2 ? alert(`最大值是：${num1}`) : alert(`最大值是：${num2}`)
用户输入一个数如果数据小于10 则前面进行补0
//用户输入：
let num = prompt('请输入第一个数字')
//判断输出-小于10才补0
num < 10 ？ '0' + num : num

分支语句-switch语句
找到跟小括号数据全等的case值 并执行里面的代码
若没有全等 === 则执行default里的代码
switch（数据）{
case值1：
    代码1
    break
case值2：
    代码2
    break
case值3：
     代码3
     break
default：
    代码n
    break
}
如果值跟2全等 则执行代码2

1.switch case语句一般用于等值判断，不适合于区间判断
2.switch case语句一般配合break关键字使用 没有break会造成case穿透
//用户输入数字
let num1 = +prompt（‘请您输入第一个数字：’）
let num2 = +prompt（‘请输入第二个数字’）
let sp = prompt（‘请输入运算符’）
//用户输入不同算数运算符 可以执行不同的运算
switch（sp）{
case ‘+’：
      alert（`两个加法的操作是${num1 + num2}`）
      break
case '-':
      alert(`两个剑法的操作值${num1 - num2}`)
      break
default:
      alert(`你干啥啊 请输入+ -`)
      break
}

循环语句：
目标：掌握循环结构，实现一段代码重复执行
学习路径：断点调试
断点调试：
作用：学习时可以帮助更好的理解代码运行，工作时可以更快找到bug
浏览器调试页面：
f12 点source 选择代码文件
while循环
重复执行一些操做 while 在满足条件的期间 重复执行某些代码
路径：
while循环基本语法
while（循环条件）{
     要重复执行的代码（循环体）
}
跟if很像 满足小括号里的条件为true才会进入循环体执行
while大括号里面的代码执行完毕不会跳出 而是继续回到小括号里判断条件是否满足，若满足又执行大括号里的代码，然后回到小括号判断条件 直到括号内条件不满足 即跳出
while循环三要素：
1.变量起始值
2.终止条件
3.变量变化量
let i = 1
while（i<=3）{
    document.write('whui1')
    i++
}

while作用：
重复执行某些代码
while循环三要素：
变量起始值
终止条件
变量变化量（自增 自减）

//1.变量起始值
let i =1
//终止条件
while（i<=3）{
   document.write('我要循环三次')
}
//变量变化量

作业：在页面中打印10句月薪过万
对了 他就执行循环体

作业：能不能改进，让用户输出打印输出的个数
let end= +prompt（'请输入的次数：'）
let i =1
while（i <=end）{
document.write('我要循环几次'）
i++
}

作业：
1.页面输出1-100
//页面输出1-100
  let i = 1
    while(i <=100){
        document.write(`这是第${i}个数字`)
        i++
    }

2.计算从1加到100的总和并输出
 //核心思路：声明累加和的变量sum
             每次把i加到sum里面

let i = 1
let sum = 0
while（i <100）{
      sum +=i
      i++
}
console.log(sum)
             
3.计算1-100之间的所有偶数和
核心思路：声明累加和的变量sum
          首先利用if语句把i里面是偶数筛选出来
          把筛选的i加到sum里面
let i = 1
let sum = 0
while（i<=100）{
     if(i%2 ===0){
        sum +=i
     }
  i++
}
console.log(sum)

循环退出
目标：能说出continue 和break的区别
break：结束本次循环
eg：
let i= 1
while（i <=5）{
   if(i === 3){
   break//突出整个循环
   }
   i++
   console.log(`我要吃第${i}个包子`)
}
continue 退出本次循环 继续下一次循环
let i= 1
while（i <=5）{
      i++//必须放到前面 不然第三次的时候后面的代码都不执行 也就意味着 i++ 不能再加了
      if(i === 3){
      continue//结束本次循环
      }
      console.log（`我要吃第${i}个包子`）
}
continue：退出本次循环，一般用于排除或者跳过某一个选项的时候，可以使用continue
break：退出整个循环，一般用于结果已经得到，后续的循环不需要的时候可以使用

作业：页面弹出对话框，‘你爱我吗’，如果爱 则结束 否则一直弹出对话框
分析：1.循环条件永远为真 一直弹出对话框
      2.循环的时候 重新让用户输入
      3.如果用户输入的是：爱 则退出循环（break）
  while（true）{
      let str = prompt（‘你爱我吗’）
      if（str ===‘爱’）{
       break
      }
  }    

  作业：简易atm取款案例：
        用户可以选择 存钱 取钱 查看余额 和退出功能
        分析：
        1.循环的时候需要反复提示输入框 输入框要写到循环里面
        2.退出条件 是用户输入了4 如果是4 则循环结束 不再弹窗
        3提前准备一个金额预先存储一个1数额
        4.取钱则是减法操作 存钱则是加法操作 查看余额则是直接显示金额
        5.输入不同的值 可以使用switch来执行不同的操作
        //准备一个总的金额
        let money = 100
        while（true）{
             let r = prompt（`
                 请选择您的操作：
                 1.存钱
                 2.取钱
                 3.查看余额
                 4.退出
              `）
              //如果用户输入的是4 那么则退出循环 break
              if（re === ‘4’）{
                     break
              }
              //根据输入做操作：
              switch（re）{
                  case 1：
                  //存钱
                  let cun = +prompt（'请输入存款金额'）
                  money = money +cun
                  break

                  case 2：
                  //取钱
                  let qu = +prompt（'请输入取款金额'）
                  money = money -cun
                  break

                  case 3：
                  alert（`您的银行卡余额是${money}`）
                  
              }
              
        }
        
        
        
      
while更适合在循环的次数不确定时候使用
break 退出

for循环 最常用的循环体
for(初始值；终止值；变量变化量){
//循环体
}

用for循环输出三句话 月薪过万
for(let i = 1;i <=3;i++){
    document.write('月薪过万')
}

遍历数组：
for循环的最大价值就是循环数组

let arr = ['刘德华','刘晓强'，'刘晓庆'，'刘若英']
console.log(arr[0])
console.log(arr[1])
console.log(arr[2])
console.log(arr[3])

for(let i = 0;i<=3;i++){
     console.log(arr[i])
}

for(let i =0;i < arr.length;i++){
    console.log(arr[i])
}
let arr1 = []
console.log

for：
continue break 两个退出循环
for(let i =1;i<=5;i++){
   if(i===3){
      continue //退出本次循环 后面的代码都不执行 继续下一次循环
   }
   console.log(i)
   document.wirte(i)
}
while（true） 构造无线循环 需要 break来跳出循环
for也是一样的
for(;;){
console.log(11)
}
fo循环和while的区别
当明确了循环次数用for循环
当不明确循环次数 用while循环

for循环之嵌套循环
一个循环再套一个循环
  for(外部声明记录循环次数的变量；循环条件；变化值){
  for（内部记录循环次数的变量；循环条件；变化值）{
      循环体
  }
  }
  计算：每天计5个单词 三天后能计算多少单词
  循环嵌套（双重for循环）
  //外层循环打印 第n天
  //里层循环打印 第几个单词
  for（let i=1；i<3;i++）{
  //内层循环打印几个单词
  for(let j =1;j <=5;j++){
     document.write（`记住了第${j}个单词`）
  }
  }
  练习：页面中打印5行5列的星星
  分析：
  1.利用双重for循环来做
  2.外层循环控制打印行 内层控制打印多少个
  //外层循环打印行数
  for（let i = 1;i<=5;i++）{
     //内循环打印几个星星
     for（let j =1；j<=5;j++）{
       document.write('*')
     }
     //进行显示换行
     document.write('<br>')
  }

  //用户输入行数和列数 打印对应的星星
  let row =+prompt('请输入行数')
  let col =+prompt（'请输入列数'）
  for(let j=1;j<=row；j++){
      document.write('*')
 
  for(let k=1'k<=col;k++){
    document.write('*')
  }
  document.write('<br>')
   }

   打印倒三角型星星
   1.利用双重for循环来做
   2.外层循环控制打印行 内层循环控制每行打印几个
   3.内层循环的个数跟第几行是--对应的
   //外层循环控制行数
     for（let i=1；i<=5;i++）{
   //内层循环控制打印几个
     for(let j=1;j<=i;j++){
     document.write('*')
     }
     //换行
     document.write('<br>')
  }

  九九乘法表：
  分析·：
  1.只需要把刚才倒三角型星星做改动
  2.*换成1x1=2格式

  数组：Array是一种可以按顺序保存数据的数据类型
  为什么要数组？
  思考：如果我想保存一个班里所有同学的姓名怎么办？
  场景：如果有多个数据可以用数组保存起来，然后放到一个变量中，管理非常方便

  目标：能够声明数组并且能够获取里面的数据
  let 数组名 = [数据1，数据2，...,数据n]

  1.字面量生成数组
  let arr = [1,2,3,'pink',true]
  2.使用new Array 构造函数声明 了解
  let arr = new Array(1,2,3,4)
  console.log(arr)
  数组是按顺序保存，所以每个数据都有自己的编号
  计算机中的编号从0开始，所以小明的编号为0 小刚编号为1 以此类推
  在数组中 数据的编号也叫索引

  取值语法：
  数组名[下标]
  let names=[1，2，3，4，]
  names[1]

  术语：
  元素：数组中保存的每个数据都叫数组元素
  下标：数组中数据的编号
  长度：数组中数据的个数，通过数组的length属性获得

  let names =['小明'，'小刚'，‘小红’，‘小丽’，‘小米’]
  console.log(names[0]) //小明
  console.log(names[1]) //小刚
  console.log（names.length）//5
  






          























































 




  
  
  
  
  
  

























 




       
       








