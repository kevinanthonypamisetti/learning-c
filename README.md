
#include <stdio.h>

int main(void) {
    int a, b, size = 15;

    // Upper part (A pattern)
    for (a = size / 2; a <= size; a += 2) {
        // Print spaces
        for (b = 1; b <= size - a; b++)
            printf(" ");
        
        // Print first block of A's
        for (b = 1; b <= a; b++)
            printf("A");

        // Print spaces between
        for (b = 1; b <= size - a; b++)
            printf(" ");

        // Print second block of A's
        for (b = 1; b <= a; b++)
            printf("A");

        printf("\n");
    }

    // Lower part (B pattern)
    for (a = size; a >= 1; a--) {
        // Print spaces
        for (b = a; b < size; b++)
            printf(" ");

        // Print B's
        for (b = 1; b <= (a * 2) - 1; b++)
            printf("B");

        printf("\n");
    }

    return 0;
}

