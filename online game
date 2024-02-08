/*Description

You are playing an online game. In the game, a list of N numbers is given. The player has to arrange the numbers so that all the odd numbers on the list come after the even numbers. Write an algorithm to arrange the given list such that all the odd numbers of the list come after the even numbers.



Input Format

The first line of the input consists of an integer num, representing the size of the list(N). The second line of the input consists of N space-separated integers representing the values of the list.



Output Format

Print N space-separated integers such that all the odd numbers of the list comes after the even numbers



Sample Input 

8

10 98 3 33 12 22 21 11



Sample Output 

Array after Segregation

10 98 22 12 33 3 21 11*/

#include <stdio.h>
void swap(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
}
void segregate(int arr[], int n) {
    int left = 0, right = n - 1;
    while (left < right) {
        while (arr[left] % 2 == 0 && left < right) {
            left++;
        }
        while (arr[right] % 2 != 0 && left < right) {
            right--;
        }
        if (left < right) {
            swap(&arr[left], &arr[right]);
            left++;
            right--;
        }
    }
}
int main() {
    int n;
    scanf("%d", &n);
    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    segregate(arr, n);
    printf("Array after Segregation\n");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }
    printf("\n");
    return 0;
}
