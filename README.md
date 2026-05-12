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

    #include <stdio.h>
    #include <stdlib.h>
    #include <time.h>

    int main() 
    {
    int count, min, max;
    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);
    
    printf("Enter the minimum value: ");
    
    scanf("%d", &min);
    printf("Enter the maximum value: ");
    
    scanf("%d", &max);
    
    srand(time(NULL));
    
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }return 0;
    
    }
    
# OUTPUT:

<img width="795" height="781" alt="image" src="https://github.com/user-attachments/assets/6653a94e-74cf-42f9-80a7-13e9cc0d9998" />

<img width="889" height="407" alt="image" src="https://github.com/user-attachments/assets/b4ea8003-f365-4e7d-a535-8a7d307533eb" />


# RESULT:

The program for Pseudorandom Number Generation is executed successfully.
