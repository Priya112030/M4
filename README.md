# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main(){
    int a=44;
    a=a<<3;
    printf("After Left Shift Operation value of a is:%d",a);
}
```

## OUTPUT
![WhatsApp Image 2025-04-27 at 15 24 04_37c40b2d](https://github.com/user-attachments/assets/f0698316-3bd1-4b5e-b7c0-06769988aea0)

## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.



# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT
## AIM
Write a C Program to check whether the two numbers are equal or not using simple if statement.


## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.


## PROGRAM
```
#include<stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if(a==b)
    {
        printf("X is equal to Y");
    }
    else
    {
        printf("X is NOT equal to Y");
    }
    return 0;
}
```

## OUTPUT
![Screenshot 2025-04-27 151357](https://github.com/user-attachments/assets/6d8f7a05-b84b-4964-bb3d-80d09438cb86)
           
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

int main() {
    char a[100];
    int l = 0;
    fgets(a, sizeof(a), stdin);
    a[strcspn(a, "\n")] = '\0';

    
    if (a[0] != '\0') {
        do {
            l++;
        } while (a[l] != '\0');
    }

    printf("%d\n", l);
    return 0;
}


## OUTPUT
![Screenshot 2025-04-27 151533](https://github.com/user-attachments/assets/9a3e9933-6eb7-493c-ad3f-22ca658d6ad0)

## RESULT
Thus the program to count the total number of words in a given string using do  While loop has been executed successfully
 
 

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

