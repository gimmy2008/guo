============���Խṹ��================
	struct jingchen_type neicun[20];
    int shumu=0,iguaqi=0,flag=0;
	for(int j=0;j<20;j++)
	{
		neicun[j].pid =j;
		printf("/n  pid=%d",neicun[j].pid);

	}
============================================


	printf("\n �����½���pid: \n");
				scanf("%d",&(neicun[i].pid));

				for(int j=0;j<20;j++)
				{
					if(neicun[i].pid==neicun[j].pid)
					{
						printf("\n �����Ѵ��� \n");
						return;
			
					}
					printf("\n �����½������ȼ�: \n");
					scanf("%d",&(neicun[i].youxian));
					printf("\n �����½��̴�С: \n");
					scanf("%d",&(neicun[i].daxiao));
					printf("\n �����½�������: \n");
					scanf("%d",&(neicun[i].info));
					neicun[i].zhuangtai=1;
					shumu++;
				}


					for(int i=0;i<20;i++)
		{
			if(neicun[i].zhuangtai==0) //�ҵ������ڴ��еĽ��̣����Դ���
			{
			  return;
			}
		}
		==============================
		void create_jingchen()
{
	if(shumu>=20) printf("\n �ڴ���������ɱ������ \n" );
	else
	{
		printf("/n ���� /n");
	
	
	}

============================================
#include <stdio.h>
#include <stdlib.h>
#include <string.h>

struct jingchen_type{
	int pid;
	int youxian;
	int daxiao;
	int zhuangtai;//0�����ڴ棬1���ڴ棬2����
	char info[10];
};

	struct jingchen_type neicun[3];
    int shumu=0,iguaqi=0,flag=0;


void create_jingchen()
{
	if(shumu>=3) printf("\n �ڴ���������ɱ������ \n" );
	else
	{
		for(int i=0;i<3;i++)
		{
			if(neicun[i].zhuangtai==0) //�ҵ������ڴ��еĽ��̣����Դ���
			{
			  
				printf("\n �����½���pid: \n");
				scanf("%d",&(neicun[i].pid));

				for(int j=0;j<i;j++)
				{
					if(neicun[i].pid==neicun[j].pid)
					{
						printf("\n �����Ѵ��� \n");
						return;
			
					}
					printf("\n �����½������ȼ�: \n");
					scanf("%d",&(neicun[i].youxian));
					printf("\n �����½��̴�С: \n");
					scanf("%d",&(neicun[i].daxiao));
					printf("\n �����½�������: \n");
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
	//printf("\n*      ������ʾϵͳ    *");
	//scanf("%d",&num);


}}