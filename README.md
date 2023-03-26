# C-Program-for-Fibonacci-Series-using-While-Loop
C Program for Fibonacci Series using While Loop
#include<stdio.h>

int main()
{
    int f1=0,f2=1,f3,i=3,len;
    printf("enter length of the  fibonacci series:");
    scanf("%d",&len);
    printf("%d\t%d",f1,f2); // It prints the starting two values
    while(i<=len)           // checks the condition
    {
        f3=f1+f2;               // performs add operation on previous two  values
        printf("\t%d",f3);      // It prints from third value to given length
        f1=f2;
        f2=f3;
        i=i+1;                  // incrementing the i value by 1
    }
    return 0;
}
