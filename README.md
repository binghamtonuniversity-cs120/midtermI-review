#### CS 120 - Spring 2019
# Midterm Review - Programming in C
## Due Date: In Lab

### Provided Files
* _Files_
    * N/A


## Review

1. Fill in the code for a C subroutine that adds two integers together, and stores the result in the location indicated by a pointer.
```c
    void addstuff(int a, int b, int *c){
            //Your Code Here
    }
    int main() {
            int x = 10;
            int y = 20;
            int z;
            addstuff(x, y, &z);
            return 0;
    }
```

2. What are the definitions of the “Boolean'' values true and false in C?
3. (tricky question) What would this code print?
```c
    int i;
    for(i = 0; i < 3; i++)
            printf("a\n");
            printf("b\n");
    printf("c\n");
```
4. Using no array syntax, write a C function that takes only a char * as a parameter and removes, in place, all the letter 'A's (UPPER and lower case) from the original string.
    * Try to do it without using any additional arrays.

5. What, if anything, will be output when you execute following c code and why? If the there is an error of any kind, explain the error.

```c
    #include<stdio.h>
    int main(){
    	char str[8];
    	str ="Network";
    	printf("%s", str);
    }

    #include<stdio.h>
    int main(){
    	int value[]={2,4,6,8,10};
    	int expr = (value[1]&value[3]) | (value[2]&value[4]);
    	printf("%d", value[expr]);
    }

    #include<stdio.h>
    int main(){
    	char ptr[] ="cquestion";
    	printf("%c", *(ptr+2));
    }
```

6. A check is a document that represents a specific amount of money from another person. For example, a check for $178.42 can represent, in its largest denominations, the following cash amounts: 1 x $100, 1 x $50, 1 x $20, 1 x $5, 3 x $1, 1 x 25¢, 2 x 10¢, 1 x 5¢, 2 x 1¢. Write two functions that represent the exchange between these these two formats:
    * A function that takes a double as a parameter and returns an array of doubles  in the largest possible denominations using the denominations specified above.
    * A function that will take an array of doubles and a size,  then return the total amount
