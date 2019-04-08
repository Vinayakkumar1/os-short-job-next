# os-short-job-next
Consider a scheduling approach which is non pre-emptive similar to shortest job next in nature. The priority of each job is dependent on its estimated run time, and also the amount of time it has spent waiting. Jobs gain higher priority the longer they wait, which prevents indefinite postponement. The jobs that have spent a long time waiting compete against those estimated to have short run times. The priority can be computed as : Priority = 1+ Waiting time / Estimated run time.
 
 solution :
   code :-
      
      #include<stdio.h>
#include<conio.h>

struct Process
{
	int process_id;
	int burst_time;
};

void sorting(struct Process temp[] ,  int n)
{
	int a;
	int i , j ;
	temp[n].burst_time=9999;
	for(j= 0 ; j < n; j++)
	{
		for(i = 0 ; i<=j ; i++)
		{
			if(temp[i].burst_time > temp[i+1].burst_time)
			{
			a = temp[i+1].burst_time;
			temp[i+1].burst_time = temp[i].burst_time;
			temp[i].burst_time = a;
			}
		}
	}
	
}


     
   

