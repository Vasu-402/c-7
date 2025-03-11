#include <stdio.h>

int main() {
    int num, sum=0, temp, digit;
    printf("enter the value:");
    scanf("%d",&num);
    temp=num;
    while(temp>0)
    {
        digit=temp%10;
        sum+=digit;
        temp/=10;
    }
    if(num%sum ==0)
    {
        printf("%d is Nivens number.\n",num);
    }
    else 
    {
        printf("%d is not a Nivens number.\n",num);
    }

  return 0;
}
