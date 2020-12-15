#define _CRT_SECURE_NO_WARNINGS

#include<stdio.h>
int main()
{
	int i, row, col, n, a[15][15] = { 0 };
	printf("输入n:\n");
	scanf("%d", &n);
	row = 0; 
	col = (n - 1) / 2;
	a[row][col] = 1;
	for (i = 2; i <= n * n; i++)
	{
		if (a[(row - 1 + n) % n][(col + 1) % n] == 0)
		{
			row = (row - 1 + n) % n;
			col = (col + 1) % n;
		}
		else
			row = (row + 1) % n;
		a[row][col] = i;
	}
	printf("%d阶魔方阵如下:\n", n);
	for (row = 0; row < n; row++)
	{
		for (col = 0; col < n; col++)
			printf("%4d", a[row][col]);
		printf("\n");
	}
	return 0;
}
