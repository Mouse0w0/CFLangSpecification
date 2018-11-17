# CFaster语言设计规范
CFaster语言是一门基于C语言的高级语言，旨在方便初学者学习编程。

## 语言特性

### 1. 连续判断
示例代码：
```c
if(month == 1 || 3 || 5 || 7 || 8 || 10 || 12) 
{
    day = 31;
}
```

### 2. 连续判断
示例代码：
```c
if(1<=month<=6) 
{
    day = 31;
}
```

### 3. 百分数
示例代码：
```c
float f = 1%; // 0.01
```

### 4. 字符串比较
示例代码：
```c
if(str1 == str2) {
    // do something
}
```

### 5. for语句逗号支持
示例代码：
```c
for(i = 0, i < 100, i++) {

}
```

### 6. 分号可省略
示例代码：
```c
printf("hello world.")
printf("There have not ';'.")
```

### 7. 高级的函数调用
示例代码：
```c
double d = pow(double x, double y);
```

### 8. 除法运算统一为浮点运算
示例代码：
```c
double d = 10 / 3; // 3.3333333333333
```

### 9. 分数类型
示例代码：
```c
fraction f = 10 / 3; // 十分之三，可做为浮点数运算
```

### 10. 除号支持
示例代码：
```c
double d = 10 ÷ 3;
``` 

### 11. 乘号支持
示例代码：
```c
double d = 10 × 3;
```

### 12. 指针方法参数自动取指针
示例代码：
```c
int i;
scanf("%d", i);
```

### 13. 隐式类型转换
示例代码：
```c
int i = 1.0;
```

### 14. if和else if不用打大括号
示例代码:
```c
if(i == 0) 
    printf("Hello world.");
    printf("This is number 0.");
else if(i == 1)
    printf("Hello world."); printf("This is number 1.");
else
{
    printf("Hello world.");
    printf("This is unknown number");
}
```

### 15. 多余参数不输入
示例代码：
```c
scanf("%d%d%d%d", &i, &j, &k);
```

### 16. scanf换行支持
示例代码：
```c
scanf("%d%d%d\n", &i, &j, &k);
```

### 17. 变量定义数组长度
示例代码：
```c
int array[i];
```

### 18. 无边界数组
示例代码：
```c
int array[10]; // 长度是什么？能吃吗？或：int array[];
int i = array[0x7fffffff];
```

### 19. void类型支持
示例代码：
```c
void i = 1;
```

### 20. main方法可以不写return 0;
示例代码：
```c
int main() {
    printf("Hello world");
}
```

### 21. main方法可以不写int返回类型
示例代码：
```c
main() {
    printf("Hello world");
    return 0;
}
```

### 22. main方法可以不写
示例代码：
```c
printf("Hello world");
```

### 23. 连等赋值
代码示例：
```c
int i = j = k = 0;
```

### 24. 指数运算符
代码示例：
```c
double d = 2^3; // 2*2*2
```

### 25. 汉字标点符号支持
代码示例：
```c
#include《stdio。h》
int main（）{
    printf（“Hello World”）；
    return 0；
}
```
