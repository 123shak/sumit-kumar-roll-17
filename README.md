# sumit-kumar-roll-17

#include<stdio.h>
#include<conio.h>

void rr(int no,int remt[10],int Cur_t,int arT[10], int bsT[10]);

main()
{
	int Proc_no,j,no,CurT,RemProc,indicator,time_quan,wait,tut,arT[10],bsT[10],remt[10],x=1;
	indicator = 0;
	wait = 0;
	tut = 1;
	printf("Enter number of processes ");
	scanf("%d",&no);
	RemProc = no;

	printf("\nEnter the arrival time and burst time of the processes\n");
	for(Proc_no = 0;Proc_no < no;Proc_no++)
	{
		printf("\nProcess P%d\n",Proc_no+1);
		printf("Arrival time = ");
		scanf("%d",&arT[Proc_no]);
		printf("Burst time = ");
		scanf("%d",&bsT[Proc_no]);
		remt[Proc_no]=bsT[Proc_no];
	}
}
