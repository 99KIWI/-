# 校招笔试面试题
分享校招笔试面试题<br>
---------------
2019-8-9(多益网络笔试)
---------------
一、单选（2道）<br>
---------------
var reg = /^[a-z]+$/;So[reg.test(null), reg.test()]结果? [true, false]<br>
<br>
一般来说,正则是只匹配字符串的，正则在执行test的时候，会优先调用toString方法，于是null-> 'null'<br>

window的open返回什么（对象？）<br>
Window {postMessage: ƒ, blur: ƒ, focus: ƒ, close: ƒ, parent: Window, …}<br>

二、多选（1）
---------------
图片下方出现几像素的空白间隙的解决方法？<br>

三、填空（5）
---------------
在数组最后添加、删除数组最后一个元素的方法？push、pop<br>

[1<2<3, 3<2<1]结果[true, true] 考查类型转换<br>

脱离文档流的position属性 fixed、absolute<br>
```
let a = 10;
let obj = {
  a:5,
  say:function() {
    console.log(this.a)
  }
}
let func = obj.say;
let func2 = obj.say.bind(obj);
func();   // undefined  
大家都知道在全局作用域中用var声明的变量，保存在window对象中 但是用ES6的const或者let在全局作用域中声明的变量，却不在window对象中
func2();  // 5
```
```
var script = document.createElement('script')
script.src = "XXX"
script.___ = function() { //script加载成功
    if(__.test(script.__)) {   //文件加载成功
      script.onreadystatechange = null;
    }
 }
 script.__ = function() {} //加载失败
```
四、问答题（8）
---------------
XSS攻击预防方法<br>
前端攻击手段<br>
readonly和disabled
<br>
onclick和addEventListener<br>
background-color和background-image占据盒子范围<br>
background-color背景颜色是包含边框border，边框如果不设置颜色，默认会采用文本颜色，而文本颜色默认是黑色。<br>
background-image背景图片占据了元素的全部尺寸，包括内边距padding和边框border，但不包括外边距margin。默认背景图片位于元素的左上角，并且在水平和垂直方向重复。<br>

Dom操作：添加、删除、移动、复制、创建、查找节点<br>

五、编程题（1）
---------------
找出数组中出现最多的元素，并给出出现过的位置<br>
