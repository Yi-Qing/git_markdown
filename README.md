# 标题
两种形式：  
1）使用`=`和`-`标记一级和二级标题.
> 一级标题   
> `=========`   
> 二级标题    
> `---------`

效果：
> 一级标题   
> =========   
> 二级标题
> ---------  

2）使用`#`, 可表示1-6级标题.
> \# 一级标题   
> \## 二级标题   
> \### 三级标题   
> \#### 四级标题   
> \##### 五级标题   
> \###### 六级标题    

效果：
> # 一级标题   
> ## 二级标题   
> ### 三级标题   
> #### 四级标题   
> ##### 五级标题   
> ###### 六级标题

# 2 段落与换行
段落的前后要有空行, 所谓的空行是指没有文字内容. 若想在段内强制换行的方式是使用`两个以上`空格加上回车(引用中换行省略回车), 
	或者使用`<br>`然后回车也可以

# 3 区块引用
在段落的每行或者只在第一行使用符号`>`,还可使用多个嵌套引用, 如：
> \> 区块引用  
> \>> 嵌套引用  

效果：
> 区块引用  
>> 嵌套引用  
> 区块引用(不能在嵌套引用后直接使用上一级的引用, 需要分段(也就是两次换行))

# 4 代码区块
代码区块的建立是在每行加上4个空格或者一个制表符（如同写代码一样）.如    
普通段落：

void main()    
{    
    printf("Hello, Markdown.");    
}    

代码区块：

    void main()
    {
        printf("Hello, Markdown.");
    }

**注意**:需要和普通段落之间存在空行.

# 5 强调
在强调内容两侧分别加上`*`或者`_`, 如:  
> \*斜体\*, \_斜体\_    
> \*\*粗体\*\*, \_\_粗体\_\_

效果：
> *斜体*, _斜体_    
> **粗体**, __粗体__

> **bugs** 在github中, 特殊字体样式与普通字体样式连用并且特殊样式位于行首的时候必须在**样式**后面添加符号分割, 否则设置无效  
> **eg:**无效  
> **eg:**.有效  
> **eg:** 有效

# 6 列表
使用`+`、或`-`标记无序列表, 如：
> \+ 第一项  
> \- 第二项

**注意**：标记后面最少有一个_空格_或_制表符_.若不在引用区块中, 必须和前方段落之间存在空行.

效果：
> + 第一项
> - 第二项

有序列表的标记方式是将上述的符号换成数字,并辅以`.`, 如：
> 1 . 第一项   
> 2 . 第二项    
> 3 . 第三项    

效果：
> 1. 第一项
> 2. 第二项
> 3. 第三项

# 7 分割线
分割线最常使用就是三个或以上`*`, 还可以使用`_`.  
分割分割
********
继续分割
_______
完毕

# 8 链接
链接可以由两种形式生成：**行内式**和**参考式**.    
**行内式**：
> \[链接\]\(https://baike.baidu.com/item/markdown/3245829?fr=aladdin).

效果：
> 我在自说自话
> [链接](https://baike.baidu.com/item/markdown/3245829?fr=aladdin)
> 说完了

**参考式**(这种形式类似论文的参考文献)：
> \[younghz的Markdown库1\]\[1\]: 我是百度  
> \[younghz的Markdown库2\]\[2\]: 我还是百度  
> \[1\]: https://www.baidu.com/  
> \[2\]: https://www.baidu.com/  

效果：
> [参考一][1]: 我是百度  
> [参考二][2]: 我还是百度

[1]: https://www.baidu.com/
[2]: https://www.baidu.com/

**注意**：上述的`[1]: https://www.baidu.com/`不显示出来.

# 9 图片
添加图片的形式和链接相似, 只需在链接的基础上前方加一个`！`.
![仓库图片](https://github.com/Yi-Qing/git_markdown/blob/learn/resource/AaronSwartz.jpg)

> __Tips__ 使用仓库中的图片时大致格式http://github.com/yourname/Repositoryname/blob/branch/path/filename

![网络图片](https://ss0.bdstatic.com/70cFuHSh_Q1YnxGkpoWK1HF6hhy/it/u=4022253116,4028438106&fm=26&gp=0.jpg)

# 10 反斜杠`\`
相当于**反转义**作用.使符号成为普通符号.

# 11 符号'`'
起到标记作用.如：
>\`ctrl+a\`

效果：
>`ctrl+a`    

# 12 列表：
用`|`表示表格纵向边界, 表头和表内容用`-`隔开, 并可用`:`进行对齐设置, 两边都有`:`则表示居中, 若不加`:`则默认居中对齐.(貌似在github中无效)

| 左对齐 | 居中 | 右对齐 | 默认 |
|:-------|:----:|-------:|------|
| 左对齐 | 居中 | 右对齐 | 默认 |
| 左对齐 | 居中 | 右对齐 | 默认 |

| 居中 | 居中 | 居中 | 默认 |
|------|------|------|------|
| 居中 | 居中 | 居中 | 默认 |
| 居中 | 居中 | 居中 | 默认 |

# 13 缩进:
可以使用`&emsp;`来表示空格, 该符号对应一个全角空格, 在使用时等于一个汉字的宽度, `&ensp;`表示半角空格, 需要使用两个才能表示一个汉字的宽度.**注意符号后面的分号**

**效果:**   
&emsp;&emsp;使用两个emsp;  
&ensp;&ensp;使用两个ensp.  
没有使用空格

详细可以参考网页: [markdown空格缩进以及HTML实体空格](https://www.jianshu.com/p/31eade263e7a)

******

**注意**：不同的Markdown解释器或工具对相应语法（扩展语法）的解释效果不尽相同, 具体可参见工具的使用说明.
虽然有人想出面搞一个所谓的标准化的Markdown, [没想到还惹怒了健在的创始人John Gruber](http://blog.codinghorror.com/standard-markdown-is-now-common-markdown).
以上基本是所有traditonal markdown的语法.
