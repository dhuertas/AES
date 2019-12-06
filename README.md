AES
===

AES algorithm implementation using C. Check out [this other repo](https://github.com/dhuertas/block-cipher-modes.git) on how to use it with different modes of operation.

# Example

Compile the source code (e.g. using GCC): 

`gcc gmult.c aes.c main.c -o aes`

And run:

```bash
./aes
Plaintext message:
00 11 22 33 44 55 66 77 88 99 aa bb cc dd ee ff
Ciphered message:
8e a2 b7 ca 51 67 45 bf ea fc 49 90 4b 49 60 89
Original message (after inv cipher):
00 11 22 33 44 55 66 77 88 99 aa bb cc dd ee ff
```
