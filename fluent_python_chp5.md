# 一等函数
__一等函数定义__：  
* 在运行时创建
* 能赋值给变量或数据结构中的元素
* 能作为参数传给函数
* 能作为函数的返回结果

## 5.1 把函数视作对象
```python
def factorial(n):
    '''return n'''
    return 1 if n<2 else n * factorial(n - 1)

factorial(42)
print(factorial.__doc__) # __doc__ 属性能打印函数的注释

fact = factorial() # 将函数赋值给变量，此处体现了一等函数的特性

print(fact(42))

print(map(factorial, range(11)))
# 将函数作为参数进行传递，此处体现了一等函数的特性

```

## 5.2 高阶函数
