# EX-26-AREA-OF-RECTANGLE-USING- POINTER
## AIM
To write a C Program to find area of rectangle using pointer.

## ALGORITHM
1.	Start the program.
2.	Read two numbers.
3.	Calculate the area of rectangle using the formula area=(x)(*y)
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include<stdio.h>
int main(){
    float a,b;
    scanf("%f %f",&a,&b);
    float *p1=&a;
    float *p2=&b;
    float formula=0.5*(*p1)*(*p2);
    printf("area of the triangle with base %.6f and height%.6f=%.6f",*p1,*p2,formula);
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/42dc8036-cf86-4fa0-ba1c-ead49d6d628f)

		       	


## RESULT
Thus the program to find area of rectangle using pointer has been executed successfully
 
 


# EX-27-DYNAMIC-MEMORY-ALLOCATION
## AIM
Write a C program to print values 101,201,301  using malloc() and free().

## ALGORITHM
1.  Start the program.
2.  Declare a pointer to an integer.
3. Use malloc() to dynamically allocate memory for an integer.
4. Assign the value 101 to the allocated memory and print it.
5. Free the allocated memory using free().
6. Repeat steps 3–5 for values 201 and 301.
7. End the program.

## PROGRAM
```
#include<stdio.h>
#include<stdlib.h>
int main(){
    int *number1=(int*)malloc(2*sizeof(int));
    number1[0]=101;
    number1[1]=201;
    number1[2]=301;
    for(int i=0;i<3;i++){
        
    printf("%d\n",number1[i]);
    }

    free(number1);

}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/e2f898c7-dfb9-4396-bbf9-c5d818258677)



## RESULT
Thus the program to print values 101,201,301  using malloc() and free(). has been executed successfully
 



# EX-28-STUDENT-INFORMATION-USING-STRUCTURE

## AIM

To write a C Program to store the student information and display it using structure.

## ALGORITHM

1.	Start the program.
2.	Create a student structure with name, roll number and marks as members.
3.	Using structure variable read the structure members and print them.
4.	Stop the program.

## PROGRAM
```
#include<stdio.h>
struct student{
    char name[50];
    int roll;
    float marks;
};
int main(){
    struct student s;
    scanf("%s",s.name);
    scanf("%d",&s.roll);
    scanf("%f",&s.marks);
    printf("Displaying Information:\n");
    printf("Name: %s\n",s.name);
    printf("Roll number: %d\n",s.roll);
    printf("Marks: %.1f",s.marks);
    
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/a72c03a2-8863-42ba-845e-6647195086f2)


## RESULT

Thus the program to store the student information and display it using structure has been executed successfully
 
 


# EX-29-EMPLOYEE-STRUCTURE-SALARY-CALCULATION

## AIM

To write a C Program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure.

## ALGORITHM

1.	Start the program.
2.	Create an employee structure with name, id and salary details as members.
3.	Using structure variable read the structure members.
4.	Calculate the gross salary and print the details.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main()
{
    int empno[3];
    char dept[3][20];
    int basic[3];
for(int i=0; i<3; i++)
    {
     scanf("%d %s %d", &empno[i],dept[i], &basic[i]);
    }
printf("Details of the Employee: \n");
for(int i=0; i<3; i++)
    {
       float da=0.10f*basic[i];
       float hra=0.30f*basic[i];
      float gross=basic[i]+da+hra;

  printf("%d    %s           %d    %.0f    %.0f    %.2f\n",empno[i], dept[i], basic[i],da,hra,gross);
}
    return 0;
}

```

 ## OUTPUT
![image](https://github.com/user-attachments/assets/f48a29aa-50af-4ce6-933e-9eb3925e44be)

 

## RESULT

Thus the C program to read and store the data of 3 employees and calculate their Gross Salary using the concept of structure
 




# EX – 30 -FIND CHARACTER IS VOWEL OR NOT

## AIM
Write a C program to find character 'Y' is vowel or consonant using pointer.

## ALGORITHM 

1. Start the program.

2. Declare a character variable a and a character pointer p.

3. Read a character from the user and store it in variable a using scanf().

4. Assign the address of a to pointer p.

5. Use an if condition to check if the character pointed by p is a vowel:

6. Check if *p is equal to 'A', 'E', 'I', 'O', 'U', or

7. Check if *p is equal to 'a', 'e', 'i', 'o', 'u'.

8. If it matches any of the above, print that the character is a vowel.

9. Otherwise, print that the character is a consonant.

10. End the program.



## PROGRAM
```
#include<stdio.h>
int main(){
    char a,*p;
    scanf("%c",&a);
    p=&a;
    if(*p=='A'||*p=='E'||*p=='I'||*p=='O'||*p=='U'){
        printf("%c is vowel",*p);
    }
    else{
        printf("%c is consonant.",*p);
    }
}
```

## OUTPUT

 ![image](https://github.com/user-attachments/assets/ed839d06-2509-4eb4-99f6-a66cb24c0a29)


## RESULT

Thus the C program to Write a C program to find character 'Y' is vowel or consonant using pointer has been executed successfully.
	


