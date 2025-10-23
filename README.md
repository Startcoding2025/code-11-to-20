//11. Write a program to input an integer and check whether it is even or odd using if–else.

#include <stdio.h>
int main()
{
    int num;
    printf("Enter an integer :");
    scanf("%d", &num);
    if (num % 2 == 0)
    {
        printf("%d is even .\n", num);
    }
    else
    {
        printf("%d is odd .\n", num);
    }
    return 0;
}



// 12. Write a program to input an integer and check whether it is positive, negative or zero using nested if–else.

#include <stdio.h>
int main()
{
    int num;
    printf("Enter an integer :");
    scanf("%d", &num);

    if (num >= 0)
    {
        if (num == 0)
        {
            printf("The number is zero .\n");
        }
        else
        {
            printf("%d is positive .\n", num);
        }
    }
    else
    {
        printf("%d is negative .\n", num);
    }
    return 0;
}



// 13. Write a program to input a year and check whether it is a leap year or not using conditional statements.

#include <stdio.h>
int main()
{
    int year;
    printf("Enter a year:");
    scanf(" %d ", &year);

    if (year % 2020 == 0)
    {
        printf(" leap year \n");
    }
    else if (year % 1900 == 0)
    {
        printf(" not a leap year \n");
    }
    else
    {
        printf(" leap year \n");
    }
    return 0;
}



// 14. write a program to input a character and check whether it is a vowel or consonant using if- else.

#include <stdio.h>
int main()
{
    char ch;
    printf("Enter a character:");
    scanf(" %c", &ch);

    if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
        ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U')
    {
        printf("%c is  a vowel \n", ch);
    }
    else
    {
        if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z'))
        {
            printf("%c is a consonant \n", ch);
        }
        else
        {
            printf("%c is not an alphabet \n", ch);
        }
    }
    return 0;
}



// 15. Write a program to input a character and check whether it is an uppercase alphabet, lowercase alphabet, digit, or special character.


#include <stdio.h>
int main()
{
    char ch;
    printf("Enter a alphabet :");
    scanf("%c", &ch);
    if (ch >= 'A' && ch <= 'z')
    {
        printf("%c is an upper case alphabet .\n", ch);
    }
    else if (ch >= 'a' && ch <= 'z')
    {
        printf("%c is a lower case alphabet .\n", ch);
    }
    else if (ch >= '0' && ch <= '9')
    {
        printf("%c is a digit .\n", ch);
    }
    else
    {
        printf("%c is a special character .\n", ch);
    }
    return 0;
}




// 16. Write a program to input three numbers and find the largest among them using if-else.
#include <stdio.h>

int main()
{
    int a, b, c;
    printf("Enter three numbers :");
    scanf(" %d %d %d ", &a, &b, &c);
    if (a >= b && a >= c)
    {
        printf("%d is the largest number .\n", a);
    }
    else if (b >= a && b >= c)
    {
        printf("%d is the largest number .\n", b);
    }
    else
    {
        printf("%d is the largest number .\n", c);
    }

    return 0;
}


// 17. Write a program to find the roots of a quadratic equation and categorize them.
#include <stdio.h>
#include <math.h>
int main()
{
    int a, b, c;
    float root 1, root 2, discriminant;
    printf("Enter coefficients a b c :");
    scanf("%d %d %d ", a, b, c);
    discriminant = b * b - 4 * a * c;
    if (discriminant > 0)
    {
        root 1 = (-b + sqrt(discriminant)) / (2 * a);
        root 2 = (-b - sqrt(discriminant)) / (2 * a);
        printf("Roots are real and differnet .\n");
        printf("Root 1 = %.2f\n", root 1);
        printf("Root 2 = %.2f\n", root 2);
    }
    else if (discriminant == 0)
    {
        root 1 = root 2 = -b / (2 * a);
        printf("Roots are real and same .\n");
        printf("Root 1 = Root 2 = %.2f\n", root 1);
    }
    else
    {
        float realPart = -b / (2 * a);
        float imagPart = sqrt(-discriminant) / (2 * a);
        printf("Roots are complex and differnt .\n");
        printf("Root 1 = %.2f + %.2fi\n", realPart, imagPart);
        printf("Root 2 = %.2f - %.2fi\n", realPart, imagPart);
    }

    return 0;
}





// 18.c Write a program that accepts a percentage (0-100) and assigns a grade based on the following criteria.
// 90-100: Grade A ,80-89: Grade B,70-79: Grade C,60-69: Grade D,below 60: Grade F.
#include <stdio.h>
int main()
{
    int percentage;
    printf("Enter the percentage (0-100):");
    scanf("%d", &percentage);
    if (percentage >= 90 && percentage <= 100)
        printf("Grade A\n");
    else if (percentage >= 80 && percentage <= 89)
        printf("Grade B\n");
    else if (percentage >= 70 && percentage <= 79)
        printf("Grade C\n");
    else if (percentage >= 60 && percentage <= 69)
        printf("Grade D\n");
    else if (percentage < 60)
        printf("Grade F\n");

    return 0;
}




// 19. Write a program to classify a triangle as Equilateral, Isosceles, or Scalene based on its side lengths.

#include <stdio.h>
#include <math.h>

int main()
{
    printf("Enter the lengths of the three sides of the triangle :");
    int a, b, c;
    scanf("%d %d %d", &a, &b, &c);
    if (a == b && b == c)
        printf(" The equilateral triangle");
    else if (a == b || b == c || c == a)
        printf("The isosceles triangle");
    else
        printf("The scalene triangle");
    return 0;
}




// 20. Write a program to display the day of the week based on a number (1–7) using switch-case
#include <stdio.h>
int main()
{
    int day;
    printf("Enter a number (1-7) to get the corresponding day of the week:");
    scanf("%d", &day);
    switch (day)
    {
    case 1:
        printf("Monday\n");
        break;
    case 2:
        printf("Tuesday\n");
        break;
    case 3:
        printf("Wednesday\n");
        break;
    case 4:
        printf("Thursday\n");
        break;
    case 5:
        printf("Friday \n");
        break;
    case 6:
        printf("Saturday \n");
        break;
    case 7:
        printf("Sunday \n");
        break;
    default:
        printf("Invalid input! please enter a number between 1 and 7.\n");
        break;
    }
    return 0;
}




