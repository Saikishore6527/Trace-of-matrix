# Trace-of-matrix
This is my first repository
#include<stdio.h>
int main()
{
int a,b;
int i,j,sum=0;
printf("enter the number of rows and columns \n");
scanf("%d %d ",&a,&b);
if (a==b)
{
int A[a][b];
printf("enter the elements into 3*4 matrix \n");
for (i=0;i<a;i++)
{
for (j=0;j<b;j++)
{
scanf("%d",&A[i][j]);
}
}
printf("given matrix is \n ");
for (i=0;i<a;i++)
{
for (j=0;j<b;j++)
{
printf(" %d ",A[i][j]);
}
printf("\n");
}
//finding trace
for (i=0;i<a;i++)
{
for (j=0;j<b;j++)
{
if (i==j)
sum =sum + A[i][j];
}
}
printf("%d",sum);
}
else
printf("trace not possible for rectangular matrix");
return 0;
}
   
