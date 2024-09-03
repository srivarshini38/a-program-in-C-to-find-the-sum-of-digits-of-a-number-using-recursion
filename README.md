# a-program-in-C-to-find-the-sum-of-digits-of-a-number-using-recursion
#include <stdio.h>

// Function to find the sum of digits using recursion
int sum_of_digits(int n) {
    if (n == 0)
        return 0;
    return (n % 10) + sum_of_digits(n / 10);
}

int main() {
    int number;
    
    // Input
    printf("Input number: ");
    scanf("%d", &number);
    
    // Output
    printf("Sum of digits: %d\n", sum_of_digits(number));
    
    return 0;
}
