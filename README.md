This project is to write a C function that produces output according to a format. The function must handle the following conversion specifiers:

* **Non-custom:** d, i, u, o, x, X
* **Custom:** p, f, %

The function must also handle the following flag characters and length modifiers for non-custom conversion specifiers:

* **Flag characters:** #, 0, -
* **Length modifiers:** l, h

The function must use a local buffer of 1024 chars in order to call write as little as possible.

**Additional requirements**

The function must also handle the following:

* Field width for non-custom conversion specifiers
* Precision for non-custom conversion specifiers
* 0 flag character for non-custom conversion specifiers
* - flag character for non-custom conversion specifiers

**Custom conversion specifiers**

The custom conversion specifiers must be implemented in a way that is consistent with the standard C library implementation of printf(). For example, the `p` conversion specifier must print the address of a pointer in hexadecimal format.

**Local buffer**

The function must use a local buffer of 1024 chars in order to call write as little as possible. This will improve the performance of the function, especially when printing large amounts of data.
