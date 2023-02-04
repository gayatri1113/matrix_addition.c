//# matrix_addition.c//
#include<stdio.h>
int main()
{
    int r,c,a[100][100],b[100][100],sum[100][100],i,j;
    printf("Enter the number of rows:");
    scanf("%d",&r);
    printf("Enter the number of colums:");
    scanf("%d",&c);
    printf("enter elements for first matrix:\n");
    for(i = 0 ; i < r ; i++)
    for(j = 0 ; j < c ; j++)
    {
    printf("Enter elements for%d%d:", i + 1, j + 1);
    scanf("%d",&a[i][j]);
    }
    
    printf("Enter elements for second matrix:\n");
    for(i=0;i<r;i++)
    for(j=0;j<c;j++)
    {
    printf("Enter elements for%d%d:",i+1,j+1);
    scanf("%d",&b[i][j]);
    }
    for(i=0;i<r;i++)
    for(j=0;j<c;j++)
    {
        sum[i][j]=a[i][j]+b[i][j];
    }
    printf("sum of two matrices:\n");
    for(i=0;i<r;i++)
    for(j=0;j<c;j++)
    {
        printf("%d  ",sum[i][j]);
        if(j==c-1)
        {
            printf("\n\n");
        }
    }
return 0;
}

