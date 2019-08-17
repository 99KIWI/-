# 校招笔试面试题
分享校招笔试面试题<br>
---------------
2019-8-9(多益网络笔试)
---------------
一、单选（2道）<br>
---------------
#### var reg = /^[a-z]+$/;So[reg.test(null), reg.test()]结果? [true, false]<br>
<br>
一般来说,正则是只匹配字符串的，正则在执行test的时候，会优先调用toString方法，于是null-> 'null'<br>

#### window的open返回什么（对象？）<br>
Window {postMessage: ƒ, blur: ƒ, focus: ƒ, close: ƒ, parent: Window, …}<br>

二、多选（1）
---------------
#### 图片下方出现几像素的空白间隙的解决方法？<br>
这个是浏览器的一个设计问题。img本来是行内元素，却可以用width 和height,当父元素没有设置高度的时候，<br>
用子元素们的高度计算出的高度给父元素的时候就会出现3px空隙这类的问题。<br>
之所以图片下方会出现几个像素空白的间隙, 是因为 img默认是按照基线(baseline)对齐的<br>
解决这问题有3个方案，一是设置img为块状元素，二给img设置vertical-algin,三设置line-height和font-size <br>
方法1：img{display:block;}<br>
方法2：img{vertical-align:top;}<br>
除了top值，还可以设置为text-top | middle | bottom | text-bottom<br>
方法3：给 img的父级 添加:font-size: 0; line-height: 0;<br>

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
script.___ = function() { //script加载成功  onload
    if(__.test(script.__)) {   //文件加载成功
      script.onreadystatechange = null;
    }
 }
 script.__ = function() {} //加载失败   onerror
 
<script>元素有一个readyState 属性，它的值随着下载外部文件的过程而改变。readyState 有五种取值：
    “uninitialized”：默认状态
    “loading”：下载开始
    “loaded”：下载完成
    “interactive”：下载完成但尚不可用
    “complete”：所有数据已经准备好
```
四、问答题（8）
---------------
XSS攻击预防方法<br>
前端攻击手段<br>
readonly和disabled
<br>
onclick和addEventListener<br>
#### background-color和background-image占据盒子范围<br>
background-color背景颜色是包含边框border，边框如果不设置颜色，默认会采用文本颜色，而文本颜色默认是黑色。<br>
background-image背景图片占据了元素的全部尺寸，包括内边距padding和边框border，但不包括外边距margin。默认背景图片位于元素的左上角，并且在水平和垂直方向重复。<br>

#### Dom操作：添加、删除、移动、复制、创建、查找节点<br>
创建新节点<br>
createDocumentFragment() //创建一个DOM片段<br>
createElement() //创建一个具体的元素<br>
createTextNode() //创建一个文本节点<br>
添加、移除、替换、插入<br>
appendChild() //添加<br>
removeChild() //移除<br>
replaceChild() //替换<br>
insertBefore() //插入<br>
查找<br>
getElementsByTagName() //通过标签名称<br>
getElementsByName() //通过元素的Name属性的值<br>
getElementById() //通过元素Id，唯一性<br>

五、编程题（1）
---------------
#### 找出数组中出现最多的元素，并给出出现过的位置<br>
<br><br><br><br>

美团点评提前批2019-08-16（一面电话面一小时）
---------------
项目经验<br>

盒模型<br>

选择器优先级<br>

margin padding 百分比 包含块 BFC<br>

inline block <br>

重绘重排<br>

怎样才能减少重绘重排<br>

数据类型判断typeof instanceof<br> 

基本数据类型和引用类型区别<br>

for of 与for in 区别 （原型链上不可枚举属性）<br>

null == undefined 0 == null 0 ==undefined 双等与三等区别<br>

cookie（问的比较细）option请求方法<br>

cookie localstorage区别<br>

其他缓存机制<br>

http 状态码304<br>

强缓存 协商缓存<br>

http2.0<br>

vue数据绑定 Obeject.defineProperty proxy <br>

vue和react区别<br>

跨域（cors 前端配置）<br>

原型链<br>

继承<br>

数组操作方法map、reduce、splice<br>

页面性能指标(首次渲染时间衡量 onload DOMContentLoaed )<br>

调试、移动端抓包<br>

页面渲染过程<br>

css阻塞、js阻塞、async、defer的应用场景<br>

图片懒加载<br>

webpack打包过程（问我有没有写过插件）<br>

git 命令（git merge)<br>
