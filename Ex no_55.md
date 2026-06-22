# EX 55 write a program to check whether the given date is valid or not using function with return type with arguments?
## DATE:
## AIM:
To write a C program to check whether the given date is valid or not using function with return type with arguments?
## Algorithm
Start
Define a function findSquare(num) that takes an integer argument.
Inside the function, compute num * num and display the result.
In the main() function:
Accept an integer input from the user.
Call findSquare(number) with the input value.
End
## Program:
```
/*C program to validate date (Check date is valid or not).*/
 
#include <stdio.h>
 
int main()
{
    int dd,mm,yy;
    scanf("%d/%d/%d",&dd,&mm,&yy);
     
    //check year
    if(yy>=1900 && yy<=9999)
    {
        //check month
        if(mm>=1 && mm<=12)
        {
            //check days
            if((dd>=1 && dd<=31) && (mm==1 || mm==3 || mm==5 || mm==7 || mm==8 || mm==10 || mm==12))
                printf("Date is valid.\n");
            else if((dd>=1 && dd<=30) && (mm==4 || mm==6 || mm==9 || mm==11))
                printf("Year is valid.\n");
            else if((dd>=1 && dd<=28) && (mm==2))
                printf("Year is valid.\n");
            else if(dd==29 && mm==2 && (yy%400==0 ||(yy%4==0 && yy%100!=0)))
                printf("Year is valid.\n");
            else
                printf("Day is invalid.\n");
        }
        else
        {
            printf("Month is not valid.\n");
        }
    }
    else
    {
        printf("Year is not valid.\n");
    }
 
    return 0;    
}

```

## Output:
<img width="996" height="285" alt="image" src="https://github.com/user-attachments/assets/6d137bc9-4155-4ee1-b9fd-cc7ba27f6713" />



## Result:
Thus the program was executed and the output was verified successfully.
