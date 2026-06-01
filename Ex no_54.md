
# EX 54 D program to print all the letters of the English alphabet.
## DATE:
## AIM:
To write a C program to print all the letters of the English alphabet.

## Algorithm:

1. **Start**  
2. Initialize a character variable `ch` with `'A'`.  
3. Loop from `'A'` to `'Z'`:  
   - Print the character.  
   - Print a space after each character.  
4. End the loop once `'Z'` is printed.  
5. **End**  

 

## Program:
```c program
#include <stdio.h>

int main() {
    char ch;
    
    for (ch = 'A'; ch <= 'Z'; ch++) {
        printf("%c ", ch);
    }
    
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/19dc5de0-1868-49eb-ae01-387170e6b6bc)


## Result:
Thus the program was executed and the output was verified successfully.
