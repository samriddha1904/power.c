#include<stdio.h>
int Power(int a, int b);
int main()
{
   int a,b;
   printf("enter the values of a and b:\n\n");
   scanf("%d%d",&a,&b);

   printf("the power of %d and %d is:%d",a,b,Power(a,b));

   return 0;
}
int Power(int a, int b)
{
  if (a==0){
   return 0;
  }
  else if (b==0){
   return 1;
 }
 else if (b==1){
  return a;
 }
 else{
  return (a*Power(a,b-1));
 }
}  
