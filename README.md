#define _CRT_SECURE_NO_WARNINGS 1

#include <stdio.h>

struct stu//构造结构体
{
	char 名字[20];//名字
	int 年龄;
	char 性别[5];
	char 学号[15];

};//分号不能掉，但是可以直接用vs自带的，会自动给分号，不用易出错
int main() {
	//char 名字 = "输入";
	struct stu s = { "史莹超",20,"男","2016260109" };
	//printf("学生信息查询，请输入姓名：\n");
	//scanf("%s",&名字);
	printf("名字 = %s\n 年龄 = %d\n 性别 = %s\n 学号 = %s\n", s.名字, s.年龄, s.性别, s.学号);//s.成员可以找到对应的
	return 0;
}
