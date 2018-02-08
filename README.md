### Less是什么
less是css的预处理器，将Less语法的文件转换为css文件，供浏览器解析

### 为啥需要less
css过于简单，没有变量函数，无法高质量复用，引入编程机制

### 现在用的多的css预处理器
less(node编写) sass(ruby编写) 一看我们都首选less啦

### 资源地址
[中文文档](http://lesscss.cn/)
[阮一峰sass博客](http://www.ruanyifeng.com/blog/2012/06/sass.html)

### 安装步骤
0. 进入项目目录， cd命令哦
1. 全局安装less指令 npm install less -g
![111](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/install1.png)
2. 编译源文件lessc path/to/source.css path/to/dist.css
![222](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/4.png)
3. 开启live-server<br />
	live-server

#### 预览效果
1. src文件夹里面是源文件，main.less
![333](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/2.png)
2. dist文件夹里面是编译之后的文件，main.css
![333](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/3.png)
3. 页面效果
![555](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/5.png)

#### 常用语法
1. 变量，方便共用啦，也能全局修改，功能不言自明
```
@fontSize16px: 16px;
.font-size-16{
	font-size: @fontSize16px;
}
```
2. 嵌套。相比于下面左图代码，可以用右边的less语法解决，更加简洁，就是嵌套
![777](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/7.png)
![666](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/6.png)
3. 混合mixin。混合就是一段可复用的代码，跟函数比较类似
使用了左边的less语法，就可以实现动态传参o~~
![888](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/8.png)
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/9.png)
4. 函数。带参数的mixin就是函数啦~~<br />
4. 函数实现if else<br />
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/10.png)<br />
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/11.png)<br />
5. 循环。利用了函数的递归，有点绕，能使用就使用吧，用的也不多
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/12.png)
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/13.png)

#### 小结
less是增强本的css，让css拥有了编程能力。
- 用变量可以做到全局替换，改一个地方全部都一起改
- 用嵌套可以避免写很多雷同的父类选择器
- 用mixin可以根据输入条件编程，实现判断，循环等等

#### 题外话
看看bootstrap里面的less应用~  
![999](https://raw.githubusercontent.com/wiki/sodyxiezhen/practice3_less/14.png)

薛傲洁测试下（么么么哒）