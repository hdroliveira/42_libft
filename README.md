# Libft - 👤 Author: hdroliveira

![42 Porto](https://img.shields.io/badge/42-Porto-blue)
![Language](https://img.shields.io/badge/Language-C-orange)
![Score](https://img.shields.io/badge/Score-125%2F100-success)

**Libft** is the very first project at 42. It challenges us to recreate some of the standard C library functions (and some additional ones) to build a personal library. This library will be used in future 42 curriculum projects.

## 📂 Project Structure

### 1. Libc Functions
Standard C library functions re-implemented from scratch.

| Function | Description |
| :--- | :--- |
| `ft_isalpha` | Checks for an alphabetic character. |
| `ft_isdigit` | Checks for a digit (0 through 9). |
| `ft_isalnum` | Checks for an alphanumeric character. |
| `ft_isascii` | Checks whether c fits into the ASCII character set. |
| `ft_isprint` | Checks for any printable character. |
| `ft_strlen` | Calculates the length of a string. |
| `ft_memset` | Fills memory with a constant byte. |
| `ft_bzero` | Zeroes a byte string. |
| `ft_memcpy` | Copies memory area. |
| `ft_memmove` | Copies memory area (safe for overlaps). |
| `ft_strlcpy` | Copies string to a specific size. |
| `ft_strlcat` | Concatenates string to a specific size. |
| `ft_toupper` | Converts char to uppercase. |
| `ft_tolower` | Converts char to lowercase. |
| `ft_strchr` | Locates character in string (first occurrence). |
| `ft_strrchr` | Locates character in string (last occurrence). |
| `ft_strncmp` | Compares two strings. |
| `ft_memchr` | Scans memory for a character. |
| `ft_memcmp` | Compares memory areas. |
| `ft_strnstr` | Locates a substring in a string. |
| `ft_atoi` | Converts a string to an integer. |
| `ft_calloc` | Allocates memory and sets its bytes' values to 0. |
| `ft_strdup` | Creates a duplicate for the string passed as parameter. |

### 2. Additional Functions
Useful functions that are not part of the standard Libc but are often used.

| Function | Description |
| :--- | :--- |
| `ft_substr` | Allocates and returns a substring from the string 's'. |
| `ft_strjoin` | Allocates and returns a new string, result of the concatenation of 's1' and 's2'. |
| `ft_strtrim` | Allocates and returns a copy of 's1' with the characters specified in 'set' removed from the start and end of the string. |
| `ft_split` | Allocates and returns an array of strings obtained by splitting 's' using the character 'c' as a delimiter. |
| `ft_itoa` | Allocates and returns a string representing the integer received as an argument. |
| `ft_strmapi` | Applies the function 'f' to each character of the string 's' to create a new string. |
| `ft_striteri` | Applies the function 'f' to each character of the string 's'. |
| `ft_putchar_fd` | Outputs the character 'c' to the given file descriptor. |
| `ft_putstr_fd` | Outputs the string 's' to the given file descriptor. |
| `ft_putendl_fd` | Outputs the string 's' to the given file descriptor, followed by a newline. |
| `ft_putnbr_fd` | Outputs the integer 'n' to the given file descriptor. |

### 3. Bonus Functions (Linked Lists)
Functions to manipulate linked lists, useful for projects requiring dynamic data structures.

| Function | Description |
| :--- | :--- |
| `ft_lstnew` | Allocates and returns a new node. |
| `ft_lstadd_front` | Adds the node 'new' at the beginning of the list. |
| `ft_lstsize` | Counts the number of elements in a list. |
| `ft_lstlast` | Returns the last node of the list. |
| `ft_lstadd_back` | Adds the node 'new' at the end of the list. |
| `ft_lstdelone` | Takes as a parameter a node and frees the memory of the node’s content. |
| `ft_lstclear` | Deletes and frees the given node and every successor of that node. |
| `ft_lstiter` | Iterates the list and applies the function 'f' to the content of each node. |
| `ft_lstmap` | Iterates the list and applies the function 'f' to the content of each node to create a new list. |

## 🛠️ Usage

### Requirements
The library is written in C language and needs the **`gcc`** compiler.

### Compilation
To compile the library, run:

```bash
make

This will generate a libft.a file.

To compile with the bonus functions (Linked Lists):
make bonus

Using it in your code
To use this library in your code, include the header and link the library during compilation:

#include "libft.h"

int main(void)
{
    ft_putstr_fd("Hello, 42!", 1);
    return (0);
}

Compile your main.c with the library:

gcc main.c -L. -lft -o program