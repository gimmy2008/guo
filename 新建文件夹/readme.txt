============测试结构体================
	struct jingchen_type neicun[20];
    int shumu=0,iguaqi=0,flag=0;
	for(int j=0;j<20;j++)
	{
		neicun[j].pid =j;
		printf("/n  pid=%d",neicun[j].pid);

	}
============================================


	printf("\n 输入新进程pid: \n");
				scanf("%d",&(neicun[i].pid));

				for(int j=0;j<20;j++)
				{
					if(neicun[i].pid==neicun[j].pid)
					{
						printf("\n 进程已存在 \n");
						return;
			
					}
					printf("\n 输入新进程优先级: \n");
					scanf("%d",&(neicun[i].youxian));
					printf("\n 输入新进程大小: \n");
					scanf("%d",&(neicun[i].daxiao));
					printf("\n 输入新进程内容: \n");
					scanf("%d",&(neicun[i].info));
					neicun[i].zhuangtai=1;
					shumu++;
				}


					for(int i=0;i<20;i++)
		{
			if(neicun[i].zhuangtai==0) //找到不在内存中的进程，可以创建
			{
			  return;
			}
		}
		==============================
		void create_jingchen()
{
	if(shumu>=20) printf("\n 内存已满，请杀死进程 \n" );
	else
	{
		printf("/n 结束 /n");
	
	
	}

============================================
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

struct jingchen_type{
	int pid;
	int youxian;
	int daxiao;
	int zhuangtai;//0不在内存，1在内存，2挂起
	char info[10];
};

	struct jingchen_type neicun[3];
    int shumu=0,iguaqi=0,flag=0;


void create_jingchen()
{
	if(shumu>=3) printf("\n 内存已满，请杀死进程 \n" );
	else
	{
		for(int i=0;i<3;i++)
		{
			if(neicun[i].zhuangtai==0) //找到不在内存中的进程，可以创建
			{
			  
				printf("\n 输入新进程pid: \n");
				scanf("%d",&(neicun[i].pid));

				for(int j=0;j<i;j++)
				{
					if(neicun[i].pid==neicun[j].pid)
					{
						printf("\n 进程已存在 \n");
						return;
			
					}
					printf("\n 输入新进程优先级: \n");
					scanf("%d",&(neicun[i].youxian));
					printf("\n 输入新进程大小: \n");
					scanf("%d",&(neicun[i].daxiao));
					printf("\n 输入新进程内容: \n");
					scanf("%d",&(neicun[i].info));
					neicun[i].zhuangtai=1;
					shumu++;
				}

			}
		}
	
	
	
	}

}

void main()
{

	create_jingchen();
	//if(shumu>=20) printf()


	//int num;
	//printf("\n*      进程演示系统    *");
	//scanf("%d",&num);


}}