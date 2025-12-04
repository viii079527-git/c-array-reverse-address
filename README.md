# c-array-reverse-address
This project is created for C programming practice. It demonstrates how to input an array, reverse it, and print each element with its memory address. 
#include <stdio.h>

int main() {
    int n, i;
    
    printf("Enter number of elements: ");
    scanf("%d", &n);
    
    int arr[n];
    
    // Reading array elements
    printf("Enter %d elements:\n", n);
    for(i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    
    // Printing in reverse order with addresses
    printf("\nArray elements in reverse order with addresses:\n");
    for(i = n - 1; i >= 0; i--) {
        printf("Value = %d\t Address = %p\n", arr[i], (void*)&arr[i]);
    }
    
    return 0;
}
