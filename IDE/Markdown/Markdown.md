> #### 版权所有转载请注明出处:*[https://github.com/LiHengofChina/java-notes](https://github.com/LiHengofChina/java-notes)*
> #### 本文内容均来自*[http://daringfireball.net/projects/markdown](http://daringfireball.net/projects/markdown)*
> #### 关于作者QQ:375461826

#Markdown简介
######Markdown 是一种轻量级的(优雅的)「标记语言」它目前被越来越多的写作爱好者、撰稿者、程序员所使用。
######Markdown 的语法十分简单，它用简洁的语法代替排版。
######而不像一般我们用的字处理软件 Word 或 Pages 有大量的排版、字体设置。
######它使我们专心于码字，用「标记」语法，来代替常见的排版格式。
######使用Markdown语言所编辑的文件后缀名为.md

#Markdown官网 
######*[http://daringfireball.net/projects/markdown/basics](http://daringfireball.net/projects/markdown/basics)*

#工具
######本人学习环境为Windows,
######推荐使用MarkdownPad这款工具
######下载地址:*[http://www.markdownpad.com/](http://www.markdownpad.com/)*
######


#常用语法

 
## 1. 标题
######语法说明:如果一段文字被定义为标题，只要在这段文字前加 # 号即可。
######以此类推，总共六级标题，建议在井号后加一个空格
######另外两级标题会带一条下划线
	        #  This is an H1
			## This is an H2
			###### This is an H6
######效果:
#   	This is an H1
## 		This is an H2
###### This is an H6

###### 一级标题也可以在第二行加入「=」号
	A First Level Header
	=====================
######效果:
A First Level Header
=====================

###### 二级标题也可以在第二行加入「-」号
	A Second Level Header
	----------------------
######效果:
A Second Level Header
----------------------




## 2. 列表 
######语法说明: 
###### 在文字前加上 +、- 或 * 即可变为无序列表
###### 在文字前加 1. 2. 3. 符号即可以变成有序列表

###无序列表
	+ Candy 
	- Gum 
	* Booze 
######无序效果:
+ Candy 
- Gum 
* Booze 


###有序列表
	1. Red
	2. Green
	3. Blue
######有序效果:
1. Red
2. Green
3. Blue



## 3. 引用 
######语法说明: 如果你需要引用一小段别处的句子，那么就要用引用的格式。
	> 我是引用
######效果:
> 我是引用
######引用和标题组合使用
	> 引用
	> > ##我来自火星
	> > > # 我来自火星
######效果:
> 引用
> > ##我来自火星
> > > # 我来自火星




## 4. 链接与图片
######语法说明: 插入链接与插入图片的语法很像，区别在一个 !号 
###### 注意:标记前必须顶格或前面接内容 「"」号内容为连接或图片的标题
	[GITHUB](https://github.com/LiHengofChina  "HHA")
######链接效果:
[GITHUB](https://github.com/LiHengofChina "HHA") 
***
	![Mou icon](http://mouapp.com/Mou_128.png)
######图片效果:
![Mou icon](http://mouapp.com/Mou_128.png "TIP")
 

## 5. 分隔线、加粗与倾斜
######分隔线说明:只需要另起一行，连续输入三个星号 *** 即可。
	***
######效果:
***

######加粗说明:用两个「*」号或「_」号包括一段文字
	Use two asterisks for **strong emphasis**. Or, if you prefer, __use two underscores instead__.
######效果:
Use two asterisks for **strong emphasis**.
Or, if you prefer, __use two underscores instead__.

######倾斜说明:用一个「*」或「_」号包括一段文字
	Some of these words *are emphasized*.Some of these words _are emphasized also_.
######效果:
Some of these words *are emphasized*.
Some of these words _are emphasized also_.

## 6. 代码框
######说明: 用「`」号将代码引起来
	`printf()`
######效果:
`printf()`
	

## 6. 表格   
######说明:  
 
######方法一:Markdown的表格语法
	| Tables        | Are           | Cool  | 
	| ------------- |-------------  | ----- |  
	| col 3 is      | right-aligned | $1600 |  
	| col 2 is      | centered      |   $12 |  
	| zebra stripes | are neat      |    $1 | 
######效果: 注意:在MarkdownPad程序中无法正常显示,但是GITHUB中可以正常显示,这是由于各种软件对于Mardown语法支持的程序不同决定的
| Tables        | Are           | Cool  | 
| ------------- | ------------- | ----- |  
| col 3 is      | right-aligned | $1600 | 
| col 2 is      | centered      |   $12 | 

| zebra stripes | are neat      |    $1 | 
######方法二:Markdown支持html，所以我们可以用html来写表格。
	<table class="table table-bordered table-striped table-condensed" >
	   <tr>
	      <th>John</th>
	      <th>Smith</th>
	      <th>123 Main St.</th>
	      <th>Springfield</th>
	   </tr>
	   <tr> 
	      <td><code>System.out.println("123")</code></td>
	      <td>Jones<I>要设为斜体的内容</I></td>
	      <td></td> 
	      <td>Dover</td> 
	   </tr>
	   <tr>
	      <td>Jim</td>
	      <td>Baker</td>
	      <td>789 Park Ave.</td>
	      <td>Lincoln</td>
	   </tr>
	</table>

######效果: 注意:在MarkdownPad程序中无法正常显示,但是GITHUB中可以正常显示,这是由于各种软件对于Mardown语法支持的程序不同决定的
<table class="table table-bordered table-striped table-condensed" >
   <tr>
      <th>John</th>
      <th>Smith</th>
      <th>123 Main St.</th>
      <th>Springfield</th>
   </tr>
   <tr> 
      <td><code>System.out.println("123")</code></td>
      <td>Jones<I>要设为斜体的内容</I></td>
      <td></td> 
      <td>Dover</td> 
   </tr>
   <tr>
      <td>Jim</td>
      <td>Baker</td>
      <td>789 Park Ave.</td>
      <td>Lincoln</td>
   </tr>
</table>