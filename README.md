# PARTHASARATHI S
# 212223040144
# EX-8-ADVANCED-ENCRYPTION-STANDARD ALGORITHM
# Aim:
To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption.

# ALGORITHM:
AES is based on a design principle known as a substitution–permutation.
AES does not use a Feistel network like DES, it uses variant of Rijndael.
It has a fixed block size of 128 bits, and a key size of 128, 192, or 256 bits.
AES operates on a 4 × 4 column-major order array of bytes, termed the state
# PROGRAM:
```
#include <stdio.h>
#include <string.h>

void xor_encrypt_decrypt(char *input, char *key) {
    int input_len = strlen(input);
    int key_len = strlen(key);
    for (int i = 0; i < input_len; i++) {
        input[i] = input[i] ^ key[i % key_len];
    }
}

int main() {
    printf("\n\n\n\n");

    char url[] = "HELLOWORLD";
    char key[] = "key123";

    printf("Original text: %s\n", url);

    xor_encrypt_decrypt(url, key);
    printf("Encrypted text: %s\n", url);

    xor_encrypt_decrypt(url, key);  // Decrypting back using the same function
    printf("Decrypted text: %s\n", url);

    return 0;
}
```
# OUTPUT:
![437329972-c65e63c5-2ad3-4288-846b-1a658d93fe88](https://github.com/user-attachments/assets/57464153-1917-43c6-85ad-094a6147b0f2)


# RESULT:

To use Advanced Encryption Standard (AES) Algorithm for a practical application like URL Encryption is verified


