#include <stdio.h>

#define MAXN 10
typedef float ElementType;

ElementType Median(ElementType A[], int N);

int main()
{
    ElementType A[MAXN];
    int N, i;

    scanf("%d", &N);
    for (i = 0; i < N; i++)
        scanf("%f", &A[i]);
    printf("%.2f\n", Median(A, N));

    return 0;
}

ElementType Median(ElementType A[], int N)
{
    ElementType temp;
    for (int gap = N / 2; gap > 0; gap = gap / 2)//gap是每次排序分组的间隔，每次间隔缩写两倍
    {
        for (int i = gap; i < N; i++)
        {
            for (int j = i - gap; j >= 0 && A[j] > A[j + gap]; j -= gap)
            {
                temp = A[j];
                A[j] = A[j + gap];
                A[j + gap] = temp;
            }
        }
    }
    return A[N / 2];
}
