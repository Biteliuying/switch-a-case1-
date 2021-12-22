# switch-a-case1-
default:break;
#define _CRT_SECURE_NO_WARNINGS
#include<stdio.h>
int main()
{
	int a = 2;
	int b = 3;
	switch (a)
	{
	case 1:a++;
	case 2:b++;
	case 3:
		switch (a)
		{
		case 1:b++;
		case 2:a++;
		}
	case 4:a++;
		break;
	default:
		break;
	}
	printf("a=%d\nb=%d\n", a, b);
	return 0;
}
