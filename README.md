#include<stdio.h>
void decimaltobinary(int num)
{
	if(num>1)
	decimaltobinary(num/2);
	printf("%d",num%2);
}
int main()
{
	int decimal;
	printf("Enter a decimal number:");
	scanf("%d",&decimal);
	printf("binary:");
	if (decimal==0)
	{
		printf("0");
		
	}else{
		decimaltobinary(decimal);
		
	}
	printf("\n");
	printf("Octal: %o\n",decimal);
	printf("Hexadecimal: %X\n",decimal);
	return 0;
}
