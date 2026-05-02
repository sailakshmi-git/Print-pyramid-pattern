# Print-pyramid-pattern
Write a c program to print the pyramid pattern.


**Program**

```
#include <stdio.h>

int main() {
    int start, end, i, j, isPrime;

    printf("Enter two numbers: ");
    scanf("%d %d", &start, &end);

    for(i = start; i <= end; i++) {
        if(i < 2) continue;

        isPrime = 1;
        for(j = 2; j <= i / 2; j++) {
            if(i % j == 0) {
                isPrime = 0;
                break;
            }
        }

        if(isPrime)
            printf("%d ", i);
    }

    return 0;
}
```

**Output**

<img width="1915" height="1149" alt="image" src="https://github.com/user-attachments/assets/e2888d84-d9a6-4fd2-a039-bb75613796f4" />


