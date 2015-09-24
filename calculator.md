# SDC-PROJECT
simply assignments
#include <stdio.h>

int main()
{
 /*defining my variables and initializing them*/
 float number1,number2;
 float result;
 int choice;
 
 /* just to print my name on the screen*/
 printf("\nWELCOME TO THE CALCULATOR PROGRAM v1.0 BY ADUKWU CYPRAIN\n");

printf("\nENTER NUMBER1\n");
scanf("%f",&number1);
printf(" ENTER NUMBER2\n");
scanf("%f",&number2);
 
 /* option to select the operation the user wants, to aid his choice*/
  
printf("\nENTER 1 FOR MULTIPLICATION\n");
printf("ENTER 2 FOR DIVISION\n");
printf("ENTER 3 FOR ADDITION\n");
printf("ENTER 4 FOR SUBTRACTION\n");
printf("\nPLEASE MAKE YOUR CHOICE:");
choice:
scanf("%d",&choice);


/* using switch case to calculate selected operation of inputs and also display the result*/ 
switch (choice)
{
case 1:
    result=(number1*number2);
    printf("\n%f * %f=%f\n\n",number1,number2,result);
    break;
case 2:
    result=(number1/number2);
    printf("\n%f / %f=%f\n\n",number1,number2,result);
   
    break; 
             
case 3:
    result=(number1+number2);
    printf("\n%f + %f=%f\n\n",number1,number2,result);
     if (number2=0)
    printf("\n%f / %f=%f",number1, number2,result);
    break;
    
case 4:
    result=(number1-number2);
    printf("\n%f - %f=%f\n\n",number1,number2,result);
    break;         
    
    default:
        printf("\nplease enter 1,2,3, 0r 4:\n");
        goto choice;        
}      
        
  system("PAUSE");	
  return 0;
}
