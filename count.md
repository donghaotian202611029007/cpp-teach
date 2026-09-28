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
