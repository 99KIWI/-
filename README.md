# 校招笔试面试题
分享校招笔试面试题
2019-8-9(多益网络笔试)

一、单选（2道）
var reg = /^[A-Z]+$/;问[reg.test(null), reg.test()]结果；

window的open返回什么（对象？）

二、多选（1）
图片下方出现几像素的空白间隙的解决方法？

三、填空
在数组最后添加、删除数组最后一个元素的方法？

[1<2<3, 3<2<1]结果

脱离文档流的position属性

let a = 10;
let obj = {
  a:5,
  say:function() {
    console.log(this.a)
  }
}
let func = obj.say;
let func2 = obj.say.bind(obj);
func();
func2();

var script = document.createElement('script')
script.src = "XXX"
script.___ = function() { //script加载成功
    if(__.test(script.__)) {   //文件加载成功
      script.onreadystatechange = null;
    }
 }
 script.__ = function() {} //加载失败

四、问答题（8）
XSS攻击预防方法
前端攻击手段
readonly和disabled
onclick和addEventListener
background-color和background-image占据盒子范围
Dom操作：添加、删除、移动、复制、创建、查找节点

五、编程题（1）
找出数组中出现最多的元素，并给出出现过的位置
