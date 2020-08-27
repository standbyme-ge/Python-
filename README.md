# Python-基础自学笔记

#1.基础===========================================================

# this is note

#打印
print("hello world")


#1.1.1 函数定义
```
'''
def             :关键字 声明
get_image_path  :函数名：定义函数的名字
picture         :路径
return          :返回值
-------------------------------------------
def get_image(picture_path):
        img = cv2.imread("picture_path")
    return img
'''
```
#1.1.2 函数参数
```
'''
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

============================================

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

'''
```
#1.2.1 python缩进
```
'''
C语言中使用{ }来区分代码块。
Pyhon 使用缩进来区分。

def SayHello():
    print("say: Hello world !")
    
>>>SayHello()
say: Hello world !
'''
```


