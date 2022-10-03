#include<stdio.h>
int main()
{
	int n,tax,sum;
	printf("Enter income :");
	scanf("%d",&n);
	if(n<1)
	{
		printf("Invalid Input...");
	}
	else if(n<=150000)
	{
		printf("\nNo Tax");
		tax=0;
	}
	else if(n>150000 && n<=300000)
	{
		tax=n*0.1;
	}
	else if(n>300000 && n<=500000)
	{
		tax=n*0.2;
	}
	else
	{
		tax=n*0.3;
	}
	printf("\n2tax = %d",tax);
	return 0;
}
