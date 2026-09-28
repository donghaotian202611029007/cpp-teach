# count++ 后置自增运算符

## 概念
count++ 叫做**后置自增运算符**
规则：**先使用变量当前的值，执行完这一行语句后，变量才 +1**

### 示例代码
```cpp
#include <iostream>
using namespace std;
int main(){
    int count = 1;
    std::cout << count++ << std::endl;
    std::cout <<count << std::endl;
    return 0;
}
```
### 解释
1. cout << count : 先拿count当前的值1打印，打印完这一行之后，count才变成2。所以这一行输出1
2. 在执行 cout << count : 此时count已经变成2，所以第二行输出2
