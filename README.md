#define _CRT_SECURE_NO_WARNINGS

#include<stdio.h>

#include<math.h>

int main()

{

	char ch;
  
	printf("请输入任意字符:\n");
  
	scanf("%c", &ch);
  
	if (ch >= 48 && ch <= 57)
  
	{
  
		printf("该字符为数字字符\n");
    
	}
  
	else if (ch >= 65 && ch <= 90)
  
	{
  
		printf("该字符为大写字符\n");
    
	}
  
	else if (ch >= 97 && ch <= 122)
  
	{
  
		printf("该字符为小写字符\n");
    
	}
  
	else if (ch == 32)
  
	{
  
		printf("该字符为空格字符\n");
    
	}
  
	else
  
	{
  
		printf("该字符为其他字符\n");
    
	}
  


	int year;
  
	int flag;
  
	printf("请输入年份：\n");
  
	scanf("%d", &year);
  
	flag = (year % 4 == 0 && year % 100 != 0 || year % 400 == 0) ? 1 : 0;
  
	if (flag = 1)
  
	{
  
		printf("是闰年\n");
    
	}
  
	else
  
	{
  
		printf("不是闰年\n");
    
	}
  
  

	int year;
  
	int flag;
  
	printf("请输入年份：\n");
  
	scanf("%d", &year);
  
	if (year % 4 ==0 )
  
	{
  
		if (year % 100 == 0)
    
		{
    
			if (year % 400 == 0)
      
				flag = 1;
        
			else
      
				flag = 0;
        
		}
    
		else
    
		{
    
			flag = 1;
      
		}
    
	}
  
	else
  
	{
  
		flag = 0;
    
	}
  
	if (flag)
  
	{
  
		printf("是闰年\n");
    
	}
  
	else
  
	{
  
		printf("不是闰年\n");
    
	}
  

	float money;
  
	int year;
  
	float a;
  
	float b;
  
	printf("请输入存钱的本金和期限\n");
  
	scanf("%f,%d", &money, &year);
  
	switch (year)
  
	{
  
	case 1:
  
		{
    
		a = money * 0.0225;
    
		b = a + money;
    
		printf("b=%f\n", b);
    
		break;
    
		}
    
	case 2:
  
	{
  
		a = money * pow(1.0243,2);
    
		printf("a=%f\n", a);
    
		break;
    
	}
  
	case 3:
  
	{
  
		a = money * pow(1.0270,3);
    
		printf("a=%f\n", a);
    
		break;
    
	}
  
	case 5:
  
	{
  
		a = money * pow(1.0288,5);
    
		printf("a=%f\n", a);
    
		break;
    
	}
  
	case 8:
  
	{
  
		a = money * pow(1.0300,8);
    
		printf("a=%f\n", a);
    
		break;
    
	}
  
	}
  

	int month;
  
	printf("请输入：\n");
  
	scanf("%d", &month);
  
	switch (month)
  
	{
  
	case 1 :
  
	{
  
		printf("1月\n");
    
		break;
    
	}
  
	case 2 :
  
	{
  
		printf("2月\n");
    
		break;
    
	}
  
	case 3:
  
	{
  
		printf("月3\n");
    
		break;
    
	}
  
	default :
  
	{
  
		printf("其他\n");
    
		break;
    
	}
  
	printf("End\n");
  
	}
  

	int a = 0;
  
	printf("请输入分数：\n");
  
  
	if (a < 60)
  
	{
  
		printf("分数：E\n");
    
	}
  
  
	else if (a < 70)
  
	{
  
  
		printf("分数：D\n");
    
	}
  
	else if (a < 80)
  
	{
  
		printf("分数：C\n");
    
	}
	else if (a < 90)
  
	{
  
		printf("分数：B\n");
    
	}
  
	else
  
	{
  
		printf("分数：A\n");
    
	}
  
	return 0;
  
}

