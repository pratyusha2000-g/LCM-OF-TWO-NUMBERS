#include<studio.h>
void lcm(int a,int b,int p,int i);
void main()
{
  int a,b;
  printf("Enter two numbers \n');
  scanf("%d,%d",&a,&b);
  lcm(a,b,a*b,1);
}

void lcm(int a,int b,int p,int i)
{
  if(i<=p)
   {
     if(i%a==0 && i%b==0)
       printf("LCM of %d and %d = %d",a,b,i);
     else
      {
         i++;
         lcm(a,b,a*b,i);
      }
    }
   else
     exit 0;
}
