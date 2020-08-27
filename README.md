# Python-基础自学笔记
  #python 基础

#微软官方教程-note

#1.基础===========================================================
```
# this is note
```
#1.1 打印
```
print("hello world")
word = input('enter your word')
```
```
tips:
cls :清除屏幕
使用单独的print()或者在语句中添加\n 来进行换行。
```
#1.2 字符串
```
+               :拼接两个字符串
upper()         :全部大写
lower()         :全部小写
capitalize()    :首字符大写
count('目标')   :统计目标出现次数
------------------------------
a_name = 'aaa'
b_name = 'bbb'
>>>print(a_name + b_name)
aaabbb
```
```
sentence = "it's a sentence"
print(sentence.upper())
print(sentence.lower())
print(sentence.capitalize())
print(sentence.count('e'))

IT'S A SENTENCE
it's a sentence
It's a sentence
3
```
===============================
```
format          :格式化字符串
-------------------------------

output = "Hello,{}{}".format(a1,b1)
output = "Hello,{0}{1}".format(a1,b1)
output = f"Hello,{a1}{b1}"
>>>print(output)
Hello,aaabbb
Hello,aaabbb
Hello,aaabbb
```
===============================
```
+               :加法
-               :减法
*               :乘法
/               :除法
**              :指数幂
--------------------------------
days_month = 30     #用str转换数字与字符
>>>print(str(days_month)+' days in June ')
30 days in June
```





#有三AI-NOTE

#1.1.1 函数定义
```
def             :关键字 声明
get_image_path  :函数名：定义函数的名字
picture         :路径
return          :返回值
-------------------------------------------
def get_image(picture_path):
        img = cv2.imread("picture_path")
    return img
```
#1.1.2 函数参数
```
x               :位置参数,先占位，待输入再运算
y               :默认参数，不输入y则用默认值，有输入则改变

                :默认参数必须在位置参数后面，否则会报错
---------------------------------------------
def sum(x,y=2):
    z = x * y
    return z

>>>sum(3)
6
>>>sum(3,3)
9
```
============================================
```
*n              :可变参数。参数前添加*变为可变。个数可变
name,age..      :关键字参数，传入0个或任意个含参数名的参数
**kk            :将参数以字典的形式导入，将aa=1变为{'aa':1}
--------------------------------------------
def sum(*num):
    sum=0
    for n in num:
        sum = sum + n
    return sum

>>> sum(1,2,3)
6

def person(name,age,**kk):
    print("name:",name,"age:",age,"other:",kk)

>>>person("yyo","12",city="CD")
name: yyo age: 12 other: {'city': 'CD'}
```

#1.2.1 python缩进
```
C语言中使用{ }来区分代码块。
Pyhon 使用缩进来区分。

def SayHello():
    print("say: Hello world !")
    
>>>SayHello()
say: Hello world !
```
#2 矩阵库-NumPy
```
NumPy 是python的扩展库，支持数组与矩阵运算，数学函数库
```
```
#2.1 ndarray 对象
```
在NumPy中使用ndarray表示数组
```
```
#2.2 创建数组
```
import numpy as np          #导入numpy这个数据库包
a0 = np.array([1,2,3])      #采用列表形式
a1 = np.array((1,2,3))      #采用元组形式

>>>print(a0)
>>>print(a1)
[1 2 3]
[1 2 3]
```





