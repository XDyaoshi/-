# -
这个是一个打印斐波那契数列的程序，用c语言写的
#include<stdio.h>  
int fun(int x)
{	
	if(x == 1)return 1;	
	if(x == 2) return 1;	
	return fun(x-1) + fun(x-2);
} 

int main()
{ 	int num,i,y;
		printf("输入一个数字: ");
		scanf("%d",&num);
		for(i=1;i<=num;i++)
		{
		y = fun(i);
        printf("Fibonacci(%d)=%d\n",i,y);
		}
		return 0;
}
