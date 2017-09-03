# ajax-demo
上述代码释义：
1、json文件
[
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"}
]
2、执行var xhr = new XMLHttpRequest()后，console.log(xhr.responseText)输出的内容：
[
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"},
{"url":"https://i.loli.net/2017/08/18/5996969b15d77.jpg"}
]
3、let array = JSON.parse(xhr.responseText)//字符串变数组，对象组成的数组集合//
console.log(array)
![image.png](http://upload-images.jianshu.io/upload_images/2132837-c67a536f156d8952.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
//JSON.parse() 方法解析一个JSON字符串，构造由字符串描述的JavaScript值或对象//
4、遍历数组后：
array.forEach(function(item,index)，console.log(item,index)的结果
![image.png](http://upload-images.jianshu.io/upload_images/2132837-0c50fbc24c312561.png?imageMogr2/auto-orient/strip%7CimageView2/2/w/1240)
//forEach() 方法对数组的每个元素执行一次提供的函数。
语法：array.forEach(callback(currentValue, index, array){
    //do something
}, this)
array.forEach(callback[, thisArg])
callback
为数组中每个元素执行的函数，该函数接收三个参数：
currentValue(当前值)
数组中正在处理的当前元素。
index(索引)
数组中正在处理的当前元素的索引。
array
forEach()方法正在操作的数组。
thisArg可选
可选参数。当执行回调 函数时用作this的值(参考对象)。
返回值是undefined

