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
2. 待续，请完成小作业，less环境的搭建及变量的使用。