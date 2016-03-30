## OS_lab1 实验报告

##### Thinking 1.1

1. ls -1

   该命令表示查看文件的详细信息以及读写权限

2. mv test1.c test2.c

   用来移动文件或者将文件改名（move (rename) files），用来备份文件或者目录。

3. cp test1.c test2.c

   复制文件或目录

4. cd

   进入文件或者文件夹

##### Thinking 1.2

Linux系统中grep命令是一种强大的文本搜索工具，它能使用正则表达式搜索文本，并把匹 配的行打印出来。

[options]主要参数：
－c：只输出匹配行的计数。
－I：不区分大 小写(只适用于单字符)。
－h：查询多文件时不显示文件名。
－l：查询多文件时只输出包含匹配字符的文件名。
－n：显示匹配行及 行号。
－s：不显示不存在或无匹配文本的错误信息。
－v：显示不包含匹配文本的所有行。
pattern正则表达式主要参数：
\： 忽略正则表达式中特殊字符的原有含义。
^：匹配正则表达式的开始行。
$: 匹配正则表达式的结束行。
\<：从匹配正则表达 式的行开始。
\>：到匹配正则表达式的行结束。
[ ]：单个字符，如[A]即A符合要求 。
[ - ]：范围，如[A-Z]，即A、B、C一直到Z都符合要求 。
。：所有的单个字符。
\* ：有字符，长度可以为0。

##### Thinking 1.3

-Werror

Make all warnings into errors.

-Wall

This enables all the warnings about constructions that some users considerquestionable, and that are easy to avoid (or modify to prevent the warning),even in conjunction with macros. This also enables some language-specificwarnings described in C++ Dialect Options and Objective-C and Objective-C++Dialect Options.

-Werror在项目开发中的意义是，当我们在编程遇到warning时，有时候我们可以忽视它且达到想要的结果，但是也会留下风险，-Werror把所有的warning转为error，使得我们不能忽略warning，增加了程序的鲁棒性。

-Wall

提示所有可能的warning，增加程序的鲁棒性。



##### Thinking 2.1

- 使用  `git checkout – printf.c`


- 使用  `git reset –-hard HEAD^`  如果没有commit可以先commit
- 使用  `git rm Tucao.txt`

##### Thinking 2.2

- 正确
- 正确
- 错误 应该是所有版本库
- 正确



##### 实验难点

1. Linux系统的掌握以及Vim编辑器的使用，对于新手都不是很容易上手。
2. 不能很好的理解工程代码的阅读顺序，特别是在填写*printf.c*时无从下手。

##### 体会与感想

​        看到代码时真的是一脸懵逼，太多的不会，很多文件闻所未闻，前期准备的工作量很大，但是代码量却很少。理解之后不是特别难。

##### 指导书反馈

​       希望在指导书中每一个练习之前添加一项建议阅读的文件/代码。因为我发现经常会浪费大量的时间在找某一个宏定义出现在哪。