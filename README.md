## Exp 14 : IMPLEMENTATION OF HASH ALGORITHM


## AIM:

To implement a simple hash algorithm in C to generate a hash value for a given message, demonstrating how hashing can be used for data integrity.


## ALGORITHM:
1.	Accept a message as input from the user.
2.	Remove any newline character from the input message.
3.	Initialize a hash value to zero.
4.	For each character in the message:
a.	Multiply the current hash value by 31 (a prime number).
b.	Add the ASCII value of the current character to the hash.
5.	After processing all characters, the final hash value is produced.
6.	Display the generated hash value as the output.


## PROGRAM:
```
#include <stdio.h>

int main() {
    char message[100];
    unsigned long hash = 0;
    int i;

    printf("Enter a message: ");
    scanf("%s", message);

    for (i = 0; message[i] != '\0'; i++) {
        hash = hash * 31 + message[i];
    }

    printf("\nGenerated Hash Value: %lu\n", hash);
    return 0;
}
```
## OUTPUT:

<img width="983" height="624" alt="Screenshot 2025-11-16 203949" src="https://github.com/user-attachments/assets/8d4b67a2-4774-491c-989c-1fa5aec8c50d" />


## RESULT:

The hash algorithm was implemented successfully, generating a hash value for the input message to demonstrate data integrity verification.
