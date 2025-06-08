#include <iostream>
using namespace std;

bool KTSNT(int x)
{
	if(x < 2)
		return false;
	for(int i = 2; i*i <= x; i++)
		if(x % i == 0)
			return false;
	return true;
}

int main()
{
	unsigned int n;
	cout << "Nhap vao so nguyen duong n: ";
	cin >> n;
	if(KTSNT(n))
		cout << n << " la so nguyen to!";
	else
		cout << n << " khong la so nguyen to!";
	cout << endl;
	return 0;
}
