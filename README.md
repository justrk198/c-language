#include <stdio.h>

int main(void) {
    int a[100];        
    int i, n, sum = 0; 

    printf("Enter the number of elements in the array (max 100): "); 
    scanf("%d", &n);  

    if (n <= 0 || n > 100) { 
        printf("Invalid number of elements. Please enter between 1 and 100.\n");
        return 1;
    }
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &a[i]);
        sum += a[i];          
    }
    printf("Sum of the array elements = %d\n", sum);

    return 0; 
}
