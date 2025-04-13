# PTA_7-11
# 分段计算居民水费
# 为鼓励居民节约用水，自来水公司采取按用水量阶梯式计价的办法，居民应交水费y（元）与月用水量x（吨）相关：当x不超过15吨时，y=4x/3；超过后，y=2.5x−17.5。请编写程序实现水费的计算。

# 输入格式：输入在一行中给出非负实数x。

# 输出格式：在一行输出应交的水费，精确到小数点后2位。
```cpp  
#include<iostream>
#include<iomanip>
using namespace std;
int main() {
	double x;
	float y;
	cin >> x;
	cout << fixed << setprecision(2); //还是一样输出要有两位小数
	if (x >= 15) {
		y = 2.5 * x - 17.5;
		cout << y;
	}
	else {
		y = 4 * x / 3;
		cout << y;
	}
	return 0;
}