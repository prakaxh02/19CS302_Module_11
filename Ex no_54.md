## Problem:

Given a sentence, S, print each word of the sentence in a new line.


Input Format

The first and only line contains a sentence, S.


Constraints

1<=len(s)<=1000


Output Format

Print each word of the sentence in a new line.


#include <stdio.h>

#include <stdlib.h>

#include <string.h>


int main()

{

    char *s;

    s = malloc(1024 * sizeof(char));

    scanf("%[^\n]", s);

    s = realloc(s, strlen(s) + 1);

    int len = strlen(s);

    for(int i = 0; i < len; i++) {

        if(s[i] == ' ') {

            printf("\n");

        }

        else {

            printf("%c", s[i]);

        }

    }

    free(s);

    return 0;

}


Sample Input 0

This is C 


Sample Output 0

This

is

C


Explanation 0

In the given string, there are three words ["This", "is", "C"]. We have to print each of these words in a new line.

```
#include <stdio.h>
#include <stdlib.h>
#include <string.h>
int main()
{
    char *s;
    s = malloc(1024 * sizeof(char));
    scanf("%[^\n]", s);
    s = realloc(s, strlen(s) + 1);
    int len = strlen(s);
    for(int i = 0; i < len; i++)
    {
        if(s[i] == ' ')
        {
            printf("\n");
        }

        else
        {
            printf("%c", s[i]);
        }
    }
    free(s);
    return 0;
}
```

Output:

<img width="598" height="297" alt="image" src="https://github.com/user-attachments/assets/0053603d-765e-4e78-a9a9-05a378816520" />

Result:
Thus the program was executed and the output was verified successfully.
