# 课后练习
## 题目1
写出程序运行结果
```cpp
#include <iostream>
using namespace std;
int main(){
    int a = 3;
    cout << a++ << endl;
    cout << a << endl;
    return 0;
}
```
题目2
用for循环，输出1到10所有数字。
参考代码
```cpp
#inculde <iostream>
using namespace std;
int main()
{
    for(int i = 1; i <= 10; i++)
    {
        cout << i << endl;
    }
    reyurn 0;
}
```
题目3
使用ctime，生成1个1~100之间的随机数。
```cpp
#include <iostream>
#include <ctime>
#include <cstdlib>
using namesace std;
int main()
{   
    srand((unsigned int)time(NULL));
    int num = rand() % 100 + 1;
    cout << num << endl;
    return 0;
}
