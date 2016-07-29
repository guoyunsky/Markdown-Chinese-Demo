针对中文,演示Markdown的各种语法
  
大标题
===================================
  大标题一般显示工程名,类似html的\<h1\><br />
  你只要在标题下面跟上=====即可

  
中标题
-----------------------------------
  中标题一般显示重点项,类似html的\<h2\><br />
  你只要在标题下面输入------即可
  
### 小标题
  小标题类似html的\<h3\><br />
  小标题的格式如下 ### 小标题<br />
  注意#和标题字符中间要有空格
### 标题的等级表示法
	关于标题的等级表示法，共分为六个等级，显示的文本大小依次减小。不同等级之间以井号#的个数来标识。一级标题有一个#，二级标题有两个#，以此类推。
		#一级标题
		##二级标题
		###三级标题
		####四级标题
		#####五级标题
		######六级标题
### 注意!!!下面所有语法的提示我都先用小标题提醒了!!! 

### 单行文本框
    这是一个单行的文本框,只要两个Tab再输入文字即可
        
### 多行文本框  
    这是一个有多行的文本框
    你可以写入代码等,每行文字只要输入两个Tab再输入文字即可
    这里你可以输入一段代码

### 比如我们可以在多行文本框里输入一段代码,来一个Java版本的HelloWorld吧
    public class HelloWorld {

      /**
      * @param args
	    */
	    public static void main(String[] args) {
		    System.out.println("HelloWorld!");

	    }

    }

### 链接
1.[点击这里你可以链接到www.google.com](http://www.google.com)<br />
2.[点击这里我你可以链接到我的博客](http://guoyunsky.iteye.com)<br />

###只是显示百度的图片
![baidu-images](http://www.baidu.com/img/bdlogo.png "baidu")  

###只是显示图片，这里用的是相对路径
![github-01.jpg](/images/01.jpg "github-01.jpg")

### 显示图片也可以用原生的html标签
<img src="http://su.bdimg.com/static/superplus/img/logo_white.png" />

###想点击某个图片进入一个网页,比如我想点击github的icorn然后再进入www.github.com
[![image]](http://www.github.com/)
[image]: /images/02.jpg "github-02.jpg"

### 文字被些字符包围
> 文字被些字符包围
>
> 只要再文字前面加上>空格即可
>
> 如果你要换行的话,新起一行,输入>空格即可,后面不接文字
> 但> 只能放在行首才有效

### 文字被些字符包围,多重包围
> 文字被些字符包围开始
>
> > 只要再文字前面加上>空格即可
>
>  > > 如果你要换行的话,新起一行,输入>空格即可,后面不接文字
>
> > > > 但> 只能放在行首才有效

### 部分文字的高亮
如果你想使一段话部分文字高亮显示，来起到突出强调的作用，那么可以把它用\`\`包围起来。
注意这不是单引号，而是Tab键和数字1键左边的按键（注意使用英文输入法）。<br />
	example：
		Thank`You`. Please `Call` Me `Coder`
### 代码片段高亮显示
GitHub的markdown语法还支持部分语言的代码片段高亮显示。只需要在代码的上一行和下一行用\`\`\`标记。
```Java
	public static void main(String[] args){} //Java
```
```c
	int main(int argc,char *argv[]) //C
```
```javascript
	document.getElementById("myH1").innerHTML="Welcome to my Homepage";//javascript
```
```cpp
	string &operator+(const string& A,const string& B) //cpp
```
	
### list列表条目使用
写文章时经常会用到list列表条目。GitHub的markdown语法里也支持使用圆点符。编辑的时候使用的是星号*。
* 国籍：中国
* 城市：北京
* 大学：清华大学 
<br/>注意：星号*后面要有一个空格。否则显示为普通星号。
GitHub还支持多级别的list列表条目：
* 编程语言
	* 脚本语言
		* Python

### 特殊字符处理
有一些特殊字符如<,#等,只要在特殊字符前面加上转义字符\即可<br />
你想换行的话其实可以直接用html标签\<br /\>
    

### 插入表格
在Markdown中插入表格比较麻烦，需要Markdown的扩展语法，但是插入HTML就没有那么麻烦了，因此我们可以通过曲线救国的方式来插入表格。       
在Markdown中，`&`符号和`<`会自动转换成HTML。

	<div>
	    <table border="0">
		  <tr>
		    <th>one</th>
		    <th>two</th>
		  </tr>
		  <tr>
		    <td>Hello</td>
		    <td>你好</td>
		  </tr>
	    </table>
	</div>
	
<div>
        <table border="0">
	  <tr>
	    <th>one</th>
	    <th>two</th>
	  </tr>
	  <tr>
	    <td>Hello</td>
	    <td>你好</td>
	  </tr>
	</table>
</div>
