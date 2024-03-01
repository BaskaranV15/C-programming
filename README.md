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
## first and second largest element in array
```c
#include <stdio.h>
int main() {
    int n,i;
    printf("Enter the size of the array: ");
    scanf("%d", &n);
    if (n <= 0) {        printf("Error: Invalid array size. enter a positive integer.\n");
        return 1; }
    int arr[n]; 
    printf("Enter %d elements for the array:\n", n);
    for (int i = 0; i < n; ++i) {
        scanf("%d", &arr[i]);}
    printf("The entered elements are: ");
    for (int i = 0; i < n; ++i) {
        printf("%d ", arr[i]);}
    printf("\n");
    int largest,seclargest;
    largest=arr[0];seclargest=arr[1];
    for(i=0;i<n;i++)
    {if(arr[i]>largest)
        {        largest=arr[i];
        }
        else if(arr[i]>seclargest && arr[i]!=largest)
        {  seclargest=arr[i];        }
    }
    printf("first largest:%d\n",largest);
    printf("second largest:%d",seclargest);
    return 0;
}

```
