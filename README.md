# C-programming-problem
Write a C code to check weather a number is divisible by 5 or 10 or 15 using switch case statement.



#include<stdio.h>
int main()
{
    int num;
    printf("Enter the number you want to check the divisibility of :\n");
    scanf("%d",&num);
    switch(num%5){
        case(0):
            switch(num%10){
                case(0):
                    printf("The number you entered is divisible by 10.\n");
                    break;
            }
            switch(num%15){
                        case(0):
                             printf("The number you entered is divisible by 15.\n");
                            break;
            }
            printf("The number you entered is divisible by 5.\n");
            break;
        default:
            printf("The number you entered is not divisible by 5.\n");
    }
    return 0;
}
