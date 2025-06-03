# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```c
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() 
{
    int count, min, max;

    // Input how many random numbers and the range
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    
    printf("Enter the minimum value: ");
    scanf("%d", &min);
    
    printf("Enter the maximum value: ");
    scanf("%d", &max);

    // Seed the random number generator with current time
    srand(time(NULL));

    printf("Pseudorandom numbers:\n");

    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }

    return 0;
}

```
# OUTPUT:

![image](https://github.com/user-attachments/assets/ca4d8953-4f93-4550-aa8d-7ad0f8f42620)


# RESULT:

Thus, the Implementation of Pseudorandom Number Generation Using Standard library is executed sucessfully

