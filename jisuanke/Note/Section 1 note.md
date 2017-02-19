---
date: 2017-02-10 15:19
status: public
title: 计蒜客课程
---

## Section 1: 你好，C++

### First programe

```cpp
# include<iostream> 

int main() {
	using namespace std;
	cout << "Hello world." << endl;
}
```

### Basic data type

+ int
+ float
+ double
+ char



## Session 2: Basic arithmetical operation



### Arithmetical operation

+ +
+ -
+ *
+ /
+ %



### Library: cmath

`#include <cmath>`

+ pow(`<float>`,`<float>`)
+ abs(`<int>`)
+ fabs(`<float>`)
+ ceil(`<double>`)
+ floor(`<double>`)
+ 三角函数(`<double>`)
+ log(`<double>`) //lg
+ log10(`<double>`)
+ sqrt(`<double>`)

### Comment



+ Single line: `//`
+ Multiple lines: `/* … */`

使用多行注释时需要比较小心，避免在同一代码块内使用多好注释，一般而言还是用单行注释比较稳健。

以下是一个使用多行注释出现问题的示例：

```c++
// Pseudocode

/* lalalala

hehehehehe /* xixixixi */

*/
```

我们会发现，`hehehehehe`部分被错误注释掉了。



## Session 3: 从伴随输入到变量地址



## ### 流式输入



```c++
#include <iostream>
using std::cin;

int main() {
  int a;
  int b;
  int c;
  
  cin >> a >> b >> c;
  
  return 0;
}
```



### Simple I/O format operation



```c++
#include <iostream>
#include <iomanip>
using std::cin;
using std::cout;
using std::endl;
using std::hex;

int main(){
    int a=22;
    //在这里输入语句
    cout << hex << a << endl;
    return 0;
}
```



### 地址与取地址



关于地址这个问题不太熟悉，看看后面会不会细讲。



```c++
#include <iostream>
using std::cout;
using std::endl;

int main() {
    int a;
    int *p; // *声明一个用于储存地址的变量
    p = &a; // &获取变量的地址
    cout << p << endl;
    
    return 0;
}
```



## Session 4: 程序中的是与非



### Relational operation



+ ==
+ \<
+ \<
+ \<=
+ \>=
+ &&
+ ||
+ !

### If…else...



```c++
if (condition) {
  <code block>;
}
else if (condition) {
  <code block>;
}
else {
  <code block>;
}
```



### 多路顺序结构



```
switch(<value>) {
  case <value1>: <code block>;break;
  case <value2>: <code block>;
  case <value3>: <code block>;
  default: <code block>;
} 
```

