# jQuery大纲 
- ### 说明 
1. 针对中职学生特性，按照传统的教学过程先进行JavaScript教学后，再讲授jQuery是不合适的，学生无法接受JavaScript过于抽象化的面向对象编程知识内容。
2. 根据网页美术设计专业教学进度，二年级后学生经过两年的设计学习。那么他们对于视觉化方面的知识对比于纯理论的知识更加感兴趣。尤其经过CSS的学习，对于所见即所得的这一学习方式更加适应。
3. jQuery虽然依赖于JavaScript，学习jQuery需要有一定的JavaScript基础，但是总的来说，比较简单，并且使用jQuery大多数是面向方法去编程，很少使用面向对象。
4. 据此，可以将jQuery与JavaScript基础知识穿插讲解来进行jQuery教学。在讲授jQuery的时候涉及到JavaScript基础知识的部分，如变量、数据类型、数学运算符、逻辑判断符、等，就进行JavaScript教学。
5. 根据暑假集训的成果来看，教学效果显著。学生通过jQuery与JavaScript的穿插学习，已经对学习JavaScript不再存在畏难情绪。并且对使用jQuery制作网页产生了浓厚的兴趣。

---

- ### 教学规划
- ### 教学主要以案例讲解为主，每个知识点辅助以合适的案例进行教学以及练习。在案例中如果牵扯到JavaScript基础知识，则重点讲解JavaScript基础知识。
- #### 01主要介绍JavaScript与jQuery的各种区别 
1. 讲述JavaScript的编写位置 
>通过<script></script>标签插入在html文档中  
 也可以通过<script src="..."></script>的方式外部引入  
 可以写在html文档的任意位置，但是原则上我们都写在<head></head>标签内部  
2. 讲述两种简单常用的排错方法

```
alert():   //弹窗功能  
console.log();    //打印功能
```  
3. 讲述JavaScript运行机制，解释性语言与编译性语言的区别  
>解释性语言一行一行翻译并执行  
编译性语言全部翻译完毕后再执行  
  
4. 通过讲解语言区别，来引入入口函数写法

```
//原生JavaScript写法
window.onload = function(){
    ......//实现功能
}

//jQuery的写法
$(function(){
    ......//实现功能
})
```
- #### 02主要介绍jQuery各类选择器
1. id选择器
```
$("#id") 
```
2. 类选择器

```
$(".element")
```
3. 标签选择器

```
$("p")
```
4. 多项选择器以及其他各类选择器

```
$("div,span,p.myClass")
```

- ####  03主要介绍各类事件
1. 以点击事件为例逐步讲解

```
$("p").click(function(){
    ......//编写功能
})
```
2. 以鼠标事件为例逐步讲解

```
$("p").mouseenter(function(){
    ......//编写功能
})
```
3. 选择常用事件进行讲解
- #### 04主要讲解行内样式的操作

```
$("p").css({ 
"color": "#ff0011",
"background": "blue"
});
```
- #### 05主要讲解css类的操作

```
addClass();     //添加class类
removeClass();  //移除class类
toggleClass();  //切换class类
```
> 这里讲解最好配合上transition来制作动画.


- #### 06主要讲解各类动画效果

```
show([s,[e],[fn]])    //显示动画
hide([s,[e],[fn]])    //隐藏动画
toggle([s],[e],[fn])  //切换动画

slideDown([s],[e],[fn])   //滑动显示
slideUp([s,[e],[fn]])     //滑动隐藏
slideToggle([s],[e],[fn]) //滑动切换

fadeIn([s],[e],[fn])      //淡入动画
fadeOut([s],[e],[fn])     //淡出动画
fadeTo([[s],o,[e],[fn]])  //淡入到
fadeToggle([s,[e],[fn]])  //淡出到
```
- #### 07主要讲解animate();自定义动画以及回调函数

```
  $("#block").animate({ 
    width: "90%",
    height: "100%", 
    fontSize: "10em", 
    borderWidth: 10
  }, 1000 );
```
- #### 08可以开始讲解各类综合案例，在案例中穿插讲解JavaScript中常用方法刺激学生学习JavaScript。如定时器|延时器的使用。
