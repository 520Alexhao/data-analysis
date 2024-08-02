# Markdown 文档使用

### 标题

```txt
# 
## 
### 
```



#表示一级标题，# 后面需要空一格

##表示二级标题，# 后面需要空一格

###表示三级标题，# 后面需要空一格

.......



### 字体

##### 换行：空两格后回车  

##### 加粗：一句话前面两个**   ，后面两个**        **人民**

``` txt
**人民**
```

##### 斜体：一句话前面一个*，   后面一个 *         *人民*

```txt
*人民*
```

##### 斜体并加粗： ***

```txt
***人民***
```

##### 删除线：~~                                    ~~sad~~

```txt
~~sad~~
```

##### 分割线： 三个连续的*号

```txt
***
```



***



### 列表和勾选框

##### 无序列表：单个*或+或-， + 空格 表示的是无序列表

```txt
* 
```

* 这是一个test

##### 有序列表：1. + 空格 表示的是一个有序列表

```txt
1. 
```

1. 这是一个test

##### 列表嵌套：在一个有序列表中嵌套无序列表（在下一行空格四行）

```txt
* 一级列表
	1. 二级列表
```



1. 一级列表
   * 二级列表

**在列表中连续两个回车不首行缩进**



##### 勾选框 * + 空格 + [x] + 表示勾选框

```txt
* [x] 
```



* [x] 勾选框
* [ ] 没有勾选

### 代码块

##### 连续打三个`即可后回车

```python
def outer(fuc):
    def wrapper(*agrs, **kwargs):
        start_time = time.time()
        response = fuc(*agrs, **kwargs)
        end_time = time.time()
        print(end_time - start_time)
        return response
    return wrapper

@outer   # inside = outer(inside)
def inside(group, s, z):
    print('欢迎来到王者荣耀')
    print(f'你出生在{group}阵营')
    print(f'敌军还有{s}秒到达战场')
    time.sleep(3)
    print(f'{z}出击')

# inside('红色',5,'全军')
```

单个函数:两个`, 中间空格

`print()`



### 引用文本

##### 一个大于号即可' > ' + 空格

```txt
> 
```

> 你好这是什么

> 暂时不知道



##### 引用文本中嵌套列表

> * 你是



### 超链接

##### 将文字用[ ]包裹后面接上(), 小括号中写入网址

```txt
[百度一下，你就知道](https://www.baidu.com)
```

请前往[官网](http://baidu.com)

##### 如果有多个链接时

```txt
[百度一下，你就知道][a]打开百度[搜索][b]
[a]:https://www.baidu.com
[b]:https://www.4399.com
```

##### 将文字用[ ]包裹后面接上[ ]，后面中括号里面填的是变量名, 最后给变量名赋值

[想要][a] 是什么等下[xxx][b]不知道是什么[想要][b]

[a]: http://www.baidu.com
[b]: https://itbaima.cn



##### 脚注：一个中括号里面 + 上尖括号 + 空格（空格写在中括号里面）

```txt
[^ 1]
```

你是什么东西[^ 1]

[^ 1]:我是脚注



### 图片的插入

```txt
单张图片的插入： ![ ]( ) 其中[]里面写的图片的描述信息, ()写的是图片的地址， 可以是本地地址，也可以是网络地址
多张图片的插入:  ![ ][ ] 其中第一个[]里面写的图片的描述信息，第二个写的是变量名
[a]:地址
```



**![图片](https://ts1.cn.mm.bing.net/th/id/R-C.57384e4c2dd256a755578f00845e60af?rik=uy9%2bvT4%2b7Rur%2fA&riu=http%3a%2f%2fimg06file.tooopen.com%2fimages%2f20171224%2ftooopen_sy_231021357463.jpg&ehk=whpCWn%2byPBvtGi1%2boY1sEBq%2frEUaP6w2N5bnBQsLWdo%3d&risl=&pid=ImgRaw&r=0)



### 表格的插入

```txt
|name|age| 
```



| name | age  |
| ---- | ---- |
|      |      |
|      |      |



### 高亮文本

```txt
==我是高亮文本==
```

==我是高亮文本==

### 上标与下标

```txt
上标： x^这是x的上标^
下标： x~这是x的下标~
```



x^这是x的上标^

x~这是x的下标~





