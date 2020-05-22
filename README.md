# shell-guide

Shell的基本命令语法。

## 入门

```
<                  改变标准输入
>                  改变标准输出
>>                 将标准输出附加到文件末尾
|                  建立管道，将多个程序衔接到一起，速度比用临时文件快10倍
chmod +x file      让file拥有执行的权限
var=value1         赋值
var2=$var          取值时在变量前加$符号

```

```
echo命令

echo [options] [arguments...]    输出内容用以提示用户,echo将各个参数打印到标准输出，参数之间以一个空格隔开，并以换行符结束。
-e                               激活转义字符
```

```
tr命令:将对来自标准输入的字符进行替换，压缩和删除。
tr [options] char-list1   char-list2

1. -d       删除标准输入的字符中所有属于char-list1的字符(此时不需要char-list2)   
2. -s       把标准输入的字符中所有属于char-list1的字符连续重复的字符压缩为一个字符(此时不需要char-list2)
3. -c       删除标准输入的字符中所有不属于char-list1的字符(与-d连用 -d -c)(此时不需要char-list2)   
4. 当选项为空时，表示将标准输入的字符中所有属于char-list1的字符转化成char-list2中的字符
```

## 查找与替换
