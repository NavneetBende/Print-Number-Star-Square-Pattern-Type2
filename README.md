PRINTING PATTERN:
13*14*15*16

9*10*11*12

5*6*7*8

1*2*3*4

PREREQUISITE:
Basic knowledge of C language and use of loops.

ALGORITHM:
Take the number of rows/columns as input from the user and store it in any variable.(‘l‘ in this case).
Run a loop ‘l’ number of times to iterate through each of the rows. From i=0 to i<l. The loop should be structured as for( i=0 ; i<l : i++).
Inside this loop run another nested loop to iterate through the columns. From j=0 to j<l. The loop should be structured as for(j=0 ; j<l ; j++).
And increment count to get the max number required.
Run a loop ‘l’ number of times to iterate through each of the rows. From i=0 to i<l. The loop should be structured as for( i=0 ; i<l : i++).
Inside this loop run another nested loop to iterate through the columns. From j=0 to j<l. The loop should be structured as for(j=0 ; j<l ; j++).
increment count and run an if condition if(j==l-1).
if true then print count else print count and a star after it.
outside the nested loop reinitialize count=count-2*l then print a newline
CODE IN C:
#include<stdio.h>
int main()
{
int i,j,l,count=0; //declaring integers i,j for loops and l for number of rows
printf("Enter the number of rows/columns\n"); //Asking user for input
scanf("%d",&l); //Taking the input for number of rows
for(int i=0;i<l;i++) //Outer loop for number of rows
  {
    for(j=0;j<l-1;j++)
      {
        count++;
      }
  }
    for(i=0;i<l;i++)
      {
        for(j=0;j<l;j++)
          {
            count++;
            if(j==l-1)
              {  
                printf("%d",count);
              }
            else
              {
                printf("%d*",count);
              }

          }
    count=count-2*l;
    printf("\n");
  } 

}
TAKING INPUT:DISPLAYING OUTPUT:
