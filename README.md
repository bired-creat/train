# train
尝试，留念
#include <stdio.h>
int main()
{
	int a, b, c;
	scanf_s("%d%d%d", &a, &b, &c);
	int i;int h;
	if (a < b)
	{
		i = a;a = b;b = i;
	}if (a < c)
	{
		a = a + c;c = a - c;a = a - c;
	}if (b < c)
	{
		h = b;b = c;c = h;
	}
	if ((b + c) > a)
	{
		if (a == b && b == c)
		{
			printf("1");
			return 0;
		}
			if (a == b || a == c || b == c)
			{
				printf("2");
				return 0;
			}
		if (b * b + c * c == a * a)
		{
			printf("3");
			return 0;
		}
		else
			printf("0");
	}
	else
		printf("error!");
	return 0;
}
