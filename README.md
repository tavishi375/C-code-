# C-code-
Using this code we can determine the number of upper case, lower case, special case and number of digits in the entered string................hope u like it and learn from it



#include<stdio.h>
int main()
{
	char a[60];
	int i=0,len,p=0,x=0,y=0,z=0,sp=0;
	printf("Enter a string: ");
	gets(a);
	len=strlen(a);
	for(i=0;i<len;i++)
	{
		if(a[i]>64&&a[i]<91)
		{
			x++;
		}
		else if(a[i]>96&&a[i]<123)
		{
			y++;
		}
		else if(a[i]>47&&a[i]<58)
		{
			z++;
		}
			else
		{
			sp++;
		}
	}
	printf("No of upper case: %d\n",x);
	printf("No of lower case: %d\n",y);
	printf("No of digits: %d\n",z);
	printf("No of special characters: %d\n",sp);
	return 0;
}	
