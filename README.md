#define _CRT_SECURE_NO_WARNINGS 
#include<stdio.h>
#include<cstring>
//struct为结构体，描述复杂对象，创建一本书
struct Book
{
	char name[20];//C语言
	short price;//55
 };//此分号不可缺少，结束类型定义

int main()
{
	struct Book b1 = { "C语言",55};
	struct Book* pd = &b1;
	//printf（“%s\n”， pd->name）;
	//printf(" % d\n", pd->price);
  b1.price = 20;
	strcpy(b1.name, "C++");
	printf("%s\n", pd->name);
	printf(" % d\n", pd->price);
	return 0;
}
