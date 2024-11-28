AES
===

AES algorithm implementation using C. Check out [this other repo](https://github.com/dhuertas/block-cipher-modes.git) on how to use it with different modes of operation.

# Disclaimer
This is a proof of concept implementation and **should not be used in a productive environment**! For example a lookup table implementation of the addition in GF2<sup>8</sup> is used which is vulnerable to side channel cache attacks. [See POC](https://github.com/ECLab-ITU/Cache-Side-Channel-Attacks/blob/master/AES%20-%20HalfKey/Flush%2BReload/Readme.md).

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
