# Markdown
Markdown是JOHN GRUBER开发的一种轻量级标记语言，它可以轻松的插入代码、图片、链接、公式、表格等等，并且很容易转化为HTML、PDF、电子书适用的格式。

# Markdown标题
Markdown标题有两种方法，第一种使用\#，可以支持1-6级标题；第二级使用=和-，仅支持两级标题。  
样例如下:  
***************************
# H1
## H2 
### H3
#### H4
##### H5
###### H6
***************************
H1  
===========================
H2  
---------------------------

# Markdown段落、区块与字体
## Markdown段落
Markdown段落划分通过文本间空行实现，文本换行有两种实现方式。第一种两个空格仅仅实现换行；第二种两段文本间插入一个空行实现换行，
此时两段文本之间隔着一个空行。样例如下：

两个空格换行，第一行  
两个空格换行，第二行  
***************************
插入空行换行，第一行

插入空行换行，第二行  
## Markdown区块
Markdown可以使用区块强调文本，并且区块可以嵌套。  
样例如下：  
标记一个区块  
>这是一个高亮文本  

标记多个嵌套区块  
>第一层
>>第二层  

## Markdown字体
Markdown通过文本两端1/2/3个\*/\_实现斜体、粗体、粗体斜体三种字体，处于简洁的目的，Markdown不支持其它字体格式  
*斜体字体*  
_斜体字体_  
**粗体字体**  
__粗体字体__  
***粗斜体字体***  
___粗斜体字体___   

# Markdown分隔线、删除线、下划线与脚注
## Markdown分隔线
Markdown使用三个及以上\*或_表示分隔线且允许中间存在空格，样例如下：
***
* * * 
*******
___
_ _ _
________________________________________

## Markdown删除线
Markdown使用左右两个~~表示删除线，样例如下：
这是一条删除线  
~~这是一条删除线~~  

## Markdown下划线
Markdown使用HTML的\<u>\</u>表示下划线，样例如下：
这是一条下划线  
<u>这是一条下划线</u>

## Markdown脚注
Markdown使用[^脚注]记号表示一条注释，样例如下：  
这是一条脚注[^Markdown脚注]  
[^Markdown脚注]: 这一条注释

# Markdown列表
Markdown支持有序列表和无序列表两种，有序列表采用数字.的形式；无序列表使用*、+、-来表示。列表支持列表间嵌套、列表与区块嵌套。
## 有序列表
1. 第一项
2. 第二项
3. 第三项

## 无序列表
* 苹果
* 梨子
* 香蕉

+ 苹果
+ 梨子
+ 香蕉

- 苹果
- 梨子
- 香蕉

## 列表嵌套列表
列表嵌套列表时子列表前面需要加入两个、四个空格或一个制表符  
1. 第一项
    * 第一项的第一项
    * 第一项的第二项
    * 第一项的第三项
2. 第二项
    * 第二项的第一项
    * 第二项的第二项
    * 第二项的第三项

* 第一项
    1. 第一项的第一项
    2. 第一项的第二项
    3. 第一项的第三项
* 第二项
    1. 第二项的第一项
    2. 第二项的第二项
    3. 第二项的第三项

## 列表嵌套区块
列表嵌套区块时需要区块>标签前加入四个空格或一个制表符  
1. 第一项
    > 第一项的区块  
2. 第二项
    > 第二项的区块  

## 区块嵌套列表
区块嵌套列表时仅需在列表标签前加入>
> 第一个区块
> * 苹果
> * 梨子
> * 香蕉  

> 第二个区块  
> 1. 第一项
> 2. 第二项
> 3. 第三项

# Markdown插入代码
## 插入一行代码
Markdown使用一个反引号表示插入一行代码，可以单独成行也可以表示行内代码。样例如下：  
这是一行行内代码`print("Hello World!")` 

## 插入一个代码块
插入代码快有两种方式，第一种使用四个空格或一个制表符；第二种使用左右三个反引号。样例如下：  
第一种  
    def add(x, y):  
         return x + y  

第二种  
```python
def add(x, y):
    return x + y
```
如果注释语言类别，可以获得高亮显示。  

# Markdown插入链接与图片
## 插入链接
Markdown有三种方式使用链接，如下所示：  
1. 链接名称  [链接名称]\(链接地址)  
2. 链接地址  \<链接地址>  
3. 变量作为链接，地址位于脚注部分(仅链接图片，不显示)  
[链接名称]\[变量]  
[变量]: 链接地址  

样例说明  
[百度一下](http://baidu.com)  
<http://baidu.com>  
这是一个变量链接: 百度一下[baidu]  
[baidu]: http://baidu.com  

## 插入图片
Markdown图片插入方式与连接极为相似，如下所示：  
1. 无标题 ![alt 属性文本]\(图片链接)
2. 有标题 ![alt 属性文本]\(图片链接 "可选标题")
3. 变量链接 ![alt 属性文本]\[变量]
[变量]:图片链接

Markdown使用本地图片时，链接可以是绝对路径或相对路径。样例如下：  
![dog](./1001851.jpg)  
![RUNOOB图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")  
![RUNOOB图标][runoob]  
[runoob]:http://static.runoob.com/images/runoob-logo.png  

Markdown无法指定图片大小，此时可使用HTML的img标签替代。样例如下：  
<img src="http://static.runoob.com/images/runoob-logo.png" width="50%">  

# Markdown插入表格
## 插入方法
Markdown使用 | 分割单元格，使用 - 分割表头与单元格，样例如下：
| 表头一 | 表头二 | 表头三 |
| ----- | ------ | ------ |
|单元格  | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |

## 对齐方式
Markdown支持左对齐、右对齐、居中对齐三种方式，语法如下：  
:-  单元格字体居左对齐  
-:  单元格字体居右对齐  
:-: 单元格字体居中对齐  

| 居左对齐 | 居右对齐 | 居中对齐 |
| :------ |  ------: | :-----: |
|  单元格  |  单元格  |  单元格  |  
|  单元格  |  单元格  |  单元格  |  
|  单元格  |  单元格  |  单元格  |  


# Markdown插入公式
Markdown支持Latex语法插入公式，插入语法如下所示：  
行内/行间公式： $...$ 或 (...)  
块内/块间公式： $$...$$ 或 [...] 或 \```math  

$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$

# Markdown其它技巧
## 转义字符  
Markdown也使用 \ 表示不可打印字符或将用于表示语法的字符转换为原意。  

\*\* 正常显示星号 \*\*  

>\    反斜线  
>\`   反引号  
>\*   星号  
>_    下划线  
>{}   花括号  
>[]   方括号  
>()   小括号  
>\#   井字号  
>\+   加号  
>\-   减号  
>.    英文句点  
>!    感叹号  

## 嵌入HTML标签 
Markdown支持嵌入部分HTML标签。
