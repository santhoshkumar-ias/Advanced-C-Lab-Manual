EXP NO: 2
C PROGRAM FOR PASSING STRUCTURES AS FUNCTION ARGUMENTS AND RETURNING A STRUCTURE FROM A FUNCTION
Aim:

To write a C program for passing a structure as a function argument and returning a structure from a function.

Algorithm:
1.Define a structure numbers with members a and b.
2.Declare a variable n of type numbers.
3.Prompt the user to enter values for a and b.
4.Read the values using scanf().
5.Call the function add() by passing the structure variable n.
6.In the function, add the values of a and b.
7.Store the result in a structure variable and return it.
8.Display the result in the main() function.
9.Stop the program.
Program:
#include <stdio.h>

struct numbers
{
    int a;
    int b;
};

struct numbers add(struct numbers n)
{
    struct numbers result;
    result.a = n.a + n.b;
    result.b = 0;
    return result;
}

int main()
{
    struct numbers n, sum;

    printf("Enter value of a: ");
    scanf("%d", &n.a);

    printf("Enter value of b: ");
    scanf("%d", &n.b);

    sum = add(n);

    printf("Sum = %d\n", sum.a);

    return 0;
}
Output:
Enter value of a: 10
Enter value of b: 20
Sum = 30
Result:

Thus, the C program for passing a structure as a function argument and returning a structure from a function was executed and verified successfully.
