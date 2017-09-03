---
title: markdown 常用语法
---
## 1. 段落、标题、区块代码
一个以上的空行来划分出不同的段落(看起来像是空行，就被视为空行，空白和 tab均可)。
Markdown 支持两种标题的语法，Setext 和 atx 形式。
Setext 形式是用底线的形式，利用 = （最高阶标题）和 - （第二阶标题）;
Atx 形式在行首插入 1 到 6 个 # ，对应到标题 1 到 6 阶。
区块引用则使用 email 形式的 '>' 角括号。
**示例：**
```
这是一个段落。

这是另一个段落。

Setext写法:
标题一
===
标题二
---
Atx写法：
# 标题一
## 标题二
### 标题三
#### 标题四
##### 标题五
###### 标题六

>这里是区块引用这里是区块引用这里是区块引用这里是区块引用这里是区块引用这里是区
```

**展示：**

这是一个段落。

这是另一个段落。

Setext写法:
标题一
===
标题二
---
Atx写法：
#标题一
##标题二
###标题三
####标题四
#####标题五
######标题六

> 这里是区块引用这里是区块引用这里是区块引用这里是区块引用这里是区块引用这里是区

## 2. 列表

#### 无序列表

无序列表使用星号、加号和减号来做为列表的项目标记，可以嵌套

**示例：**
```
* 列表1
    + 列表11
        - 列表111
+ 列表2
    * 列表22
        - 列表222
- 列表3
    * 列表33
        + 列表333
```

**展示：**

* 列表1
    + 列表11
        - 列表111
+ 列表2
    * 列表22
        - 列表222
- 列表3
    * 列表33
        + 列表333

#### 有序列表
文字前面加上 1. 2. 3. 就可以添加序号

**示例：**

```
1. 列表1
2. 列表2
3. 列表3
```

**展示：**

1. 列表1
2. 列表2
3. 列表3

**注意:符号与文本之间保留一个字符的空格，否则不生效**

## 3. 文本设置
#### 倾斜

首尾加一个星号或下划线都可以

**示例：**

```
*文本*

_文本_
```

**展示：**

*文本*

_文本_

#### 加粗

首尾加一个星号或下划线都可以

**示例：**

```
**文本**

__文本__
```

**展示：**

**文本**

__文本__

## 4. 链接

Markdown 支援两种形式的链接语法： 
行内 和 参考两种形式，两种都是使用角括号来把文字转成链接，还可以选择性的加上 title 属性。

#### 行内形式是直接在后面用括号直接接上链接

**示例：**

```
这是一个有title的[链接](https://www.google.com.hk/)

这是一个无title的[链接](https://www.google.com.hk/ "Google")
```

**展示：**

这是一个有title的[链接](https://www.google.com.hk/)

这是一个无title的[链接](https://www.google.com.hk/ "Google")

#### 参考形式的链接让你可以为链接定一个名称，之后你可以在文件的其他地方定义该链接的内容

**示例：**

```
我是用 [Google][1] 搜索[W3C][2]

[1]: https://www.google.com.hk/ "Google"
[2]: https://www.w3.org/ "W3C"
```

**展示：**

我是用 [Google][1] 搜索[W3C][2]

[1]: https://www.google.com.hk/ "Google"
[2]: https://www.w3.org/ "W3C"

## 5. 图片

图片的语法和链接类似

**示例：**

```
![](https://www.google.com.hk/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google")

![][3] 
![][4] 

[3]: https://www.google.com.hk/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google"
[4]: https://www.w3.org/2008/site/images/logo-w3c-screen-lg "W3C"
```

**展示：**

![](https://www.google.com.hk/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google")

![][3] 
![][4] 

[3]: https://www.google.com.hk/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png "Google"
[4]: https://www.w3.org/2008/site/images/logo-w3c-screen-lg "W3C"

**注意:title 与链接地址之间保持一个空格，否则错误**

## 6. 分割线
**示例：**
```
---
```


**展示：**

---

## 7. 表格

**示例：**
```
First Header | Second Header | Third Header
:----------- | :-----------: | -----------:
Left         | Center        | Right
Left         | Center        | Right
```


**展示：**

First Header | Second Header | Third Header
:----------- | :-----------: | -----------:
Left         | Center        | Right
Left         | Center        | Right


## 8. 代码

#### 使用`包裹含段落文字中的代码区段

**示例：**
```
html的空格符号是`&nbsp`，换行符号是`</br> `，按钮可以这么写`<input type="button" value="" `
```


**展示：**

html的空格符号是`&nbsp`，换行符号是`</br> `，按钮可以这么写`<input type="button" value="" `

#### 使用```包裹代码块

