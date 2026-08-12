## 流程控制语句
### 条件判断
![alt text](19099589c310d15a64291343dabe4780.jpg)  
注意：
1. Python中通过缩进来描述代码归属，，归属于if代码块的语句，需要在前方缩进四个空格。  
2. 同一个代码块下的语句缩进空格数需相同。

![alt text](b2fa99b9aa12e966c6a6638687563c48.jpg)  
![alt text](image.png)  

### 模式匹配
![alt text](16198b2afb4562eed3f9769de96c7eee.jpg)  ，用于维持

注意：
1. case _匹配其他输入  
2. pass为空语句，起占位作用，为了维持语法完整使用  

进阶case+if守卫
```python
data = ("tom", 22)
match data:
    case (name, num) if num > 18 and len(name) >2:
//case 变量|常量 if布尔表达式：只有满足if条件+匹配同时满足才进case
//data是元组，case（name，num）这一步叫做解构（解包）
        print(f"匹配成功：{name},{num}")
    case _:
        print("不匹配")
```

### 循环
#### while循环
![alt text](b0e315016e2a66ff9531f9baf2610a42.jpg)  
条件表达式成立就执行循环语句，执行完毕后再次判断条件表达式是否成立。流程如下  
![alt text](eb96558104c2a71959aace3fd5c2b622.jpg)  
while-else结构：  
![alt text](415ad269df796e1b3f8dc96dbfd529bd.jpg)  
*else部分可有可无*  


