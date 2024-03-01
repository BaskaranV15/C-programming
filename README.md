# C-programming
# Transpose of matix
```c
#include <stdio.h>
int main() {
int row,column,i,j;
printf("Enter a row size:");
scanf("%d",&row);
printf("Enter a column size:");
scanf("%d",&column);
int matrix[10][10];
int tranpose[10][10];
for(i=0;i<row;i++)
{
    for(j=0;j<column;j++)
    {
        scanf("%d",&matrix[i][j]);
    }
}
printf("Transepose matrix:\n");
for(i=0;i<row;i++)
{
    for(j=0;j<column;j++)
    {
       tranpose[j][i]=matrix[i][j];
    }
}
for(i=0;i<column;i++)
{
    for(j=0;j<row;j++)
    {
       printf("%d ",tranpose[i][j]);
    }
    printf("\n");
}
printf("orginal matrix\n");
for(i=0;i<row;i++)
{
    for(j=0;j<column;j++)
    {
        printf("%d ",matrix[i][j]);
    }
    printf("\n");
}
    return 0;
}
```
