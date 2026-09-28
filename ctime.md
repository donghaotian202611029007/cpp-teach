# ctime 头文件
## 概念
`<ctime>`是C++的头文件，主要用来获取系统时间。
常搭配`time()` 函数，用来给随机数设置种子，让每次运行程序得到不一样的随机数字。

## 示例代码
```cpp
#include <iostream>
#include <ctime>
#include <cstdlib>
using namespace std;

int main()
{
    // 设置随机数种子，依靠当前系统时间
    strand((unsigned int)time(NULL));

    //生成 0~9 的随机数
    int num = rand() % 10;
    cout << "随机数字:" << num << endl;
    return 0;
}
```
知识点说明
1. #include <ctime> : 引入事间相关函数
2. time(NULL) ：获取当前系统时间
3. srand（）：设置随机数种子，只需要写一次
4. rand（） % 10 ：生成0到9的随机整数
