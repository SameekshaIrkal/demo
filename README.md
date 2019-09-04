//Maximum element in list
#include <iostream>
using namespace std;
class Maximum
{
public:
	void max(int[], int);
};

void Maximum::max(int list[], int size)
{
	int big, index;
	big = list[0];
	for (index = 1; index < size; index++)
	{
		if (list[index] > big)
		{
			big = list[index];
		}
	}
	cout << "maximum element is : " << big;
}

int main()
{
	int size, element[5];
	Maximum m1;
	cout << "enter the size of array";
	cin >> size;
	cout << "enter array elements";
	for (int start = 0; start < size; start++)
	{
		cin >> element[start];
	}
	m1.max(element, size);
	return 0;
}
