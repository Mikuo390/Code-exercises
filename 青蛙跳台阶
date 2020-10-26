#include<stdio.h>
int Math(int n)
{
	int a = 1;
	int b = 1;
	int c = 1;
	while (n>1)
	{
		c = a + b;
		a = b;
		b = c;
		n--;
	}
	return c;
}
int main()
{
	int n = 0;
	int t = 0;

	printf("台阶的层数为:");
	scanf("%d", &n);

	t = Math(n);
	printf("青蛙有%d钟跳法\n", t);

	return 0;
}
