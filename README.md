# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 1 and 1.
3.	Use bitwise OR operator.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```

```

## OUTPUT


## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.



# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT
## AIM
Write a C Program to check whether the two numbers are equal or not using simple if statement.


## ALGORITHM
1.	Start the program.
2.	Read remarks for the grade.
3.	If grade is equal to C, display Fair.
4.	If grade is equal to D, display Bad.
5.	Stop the program.

## PROGRAM
```

```

## OUTPUT

           
## RESULT
Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully.

 
## EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
#include <ctype.h>

int main() {
    char str[100];
    scanf("%s", str);
    for (int i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/338550d0-4a9f-4670-8b1e-56a0c43c71f9)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 
## EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <string.h>
#include <ctype.h>
int main() {
    char str[200];
    int i = 0, c = 0;
    int inword = 0;
    fgets(str, sizeof(str), stdin);
    str[strcspn(str, "\n")] = '\0'; 

    if (str[0] != '\0') { 
        do {
            if (!isspace(str[i])) {
                if (inword == 0) {
                    c++;
                    inword = 1;
                }
            } else {
                inword = 0;
            }
            i++;
        } while (str[i] != '\0');
    }

    printf("%d\n", c);
    return 0;
}

}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/e8bafbe0-1ad2-4817-9a28-64fc98816e7d)

## RESULT
Thus the program to count the total number of words in a given string using  While loop has been executed successfully
 
 

## EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
```
Step 1: Start
Step 2: Declare two character arrays str1 and str2 to store the input strings
Step 3: Declare integer variables i (for index) and flag (to indicate mismatch), and initialize i = 0, flag = 0
Step 4: Read two strings from the user using scanf()
Step 5: Repeat the following steps while either str1[i] or str2[i] is not equal to the null character ('\0'):
If str1[i] is not equal to str2[i]:
Set flag = 1
Break out of the loop
Else:
Increment i to move to the next character
Step 6: After the loop, check the value of flag:
If flag == 0, then print "strings are same"
Else, print "strings are not same"
Step 7: End
```

## PROGRAM
```
# include <stdio.h>

int main(){
    char str1[100],str2[100];
    int i=0,flag=0;
    scanf("%s%s",str1,str2);
    while (str1[i] != '\0' || str2[i] != '\0'){
        if(str1[i] != str2[i]) {
            flag=1;
            break;
        }
        i++;
    } 
    if (flag==0)
         printf("strings are same\n");
    else
         printf("strings are not same\n");
         
    return 0;
```

## OUTPUT
![image](https://github.com/user-attachments/assets/1131f85c-ce6f-453d-a2c5-8ac5f85d8a41)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

