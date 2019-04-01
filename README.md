# os-short-job-next
Consider a scheduling approach which is non pre-emptive similar to shortest job next in nature. The priority of each job is dependent on its estimated run time, and also the amount of time it has spent waiting. Jobs gain higher priority the longer they wait, which prevents indefinite postponement. The jobs that have spent a long time waiting compete against those estimated to have short run times. The priority can be computed as : Priority = 1+ Waiting time / Estimated run time.
 
 solution :
   code :-
      
      
      #include<stdio.h>  

void main()


{

    


   int bt[20],p[20],wait[20],tat[20],i,j,n,total=0,pos,temp;

   
    float avg_wt,avg_tat;

    
       printf("Enter number of process:");

      //enter no of process by your choice.
     scanf("%d",&n);  

   
       printf("\nEnter Estimated Time:\n");

    //enter estimated time .
}
