# EX 53  
Complete the calculate_the_maximum function in the editor below.

calculate_the_maximum has the following parameters:

int n: the highest number to consider
int k: the result of a comparison must be lower than this number to be considered
Prints

Print the maximum values for the and, or and xor comparisons, each on a separate line.

## DATE:
## AIM:
To write a C program to remove duplicates in an array.

## Algorithm
   
Start
Input the number of elements n.
Input n elements into the array.
Create an empty temporary array temp to store unique elements.
Initialize an index variable index = 0.
Loop through each element in the original array:
Check if the element already exists in temp.
If the element is not a duplicate, add it to temp and increment index.
Copy the elements from temp back to the original array.
Update n to the new size of the array.
Print the modified array without duplicates.
End
## Program:
```
#include <stdio.h>
int main(){
    int a,b;
    scanf("%d %d",&a,&b);
    
    int and=0,or=0,xor=0;
    for(int i=1;i<=a;i++){
        for(int j=i+1;j<=a;j++){
            if((i&j)>and && (i&j)<b){
                and=i&j;
            }
            if((i|j)>or && (i|j)<b){
                or=i|j;
            }
            if((i^j)>xor && (i^j)<b){
                xor=i^j;
            }
        }
    }
    printf("%d\n%d\n%d",and,or,xor);
}
```

## Output:

<img width="876" height="383" alt="image" src="https://github.com/user-attachments/assets/18744411-b2b0-44d5-9281-ec0739827030" />


## Result:
Thus the program was executed and the output was verified successfully.
