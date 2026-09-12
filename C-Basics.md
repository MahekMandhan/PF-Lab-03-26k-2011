
# C Programming Basics

This document explains important concepts of the C programming language, including data types, format specifiers, input/output functions, escape sequences, and precision.

## 1. Data Types

| Data Type | Description |
|---|---|
| `int` | Stores whole numbers, such as 10 or -5. |
| `float` | Stores single-precision floating-point numbers. |
| `double` | Stores double-precision floating-point numbers. |
| `char` | Stores a single character, such as 'A'. |
| `bool` | Stores either true or false. In C, it is available through `stdbool.h`. |
| `void` | Represents the absence of a value or type. |

## 2. Format Specifiers

Format specifiers are used with functions such as `printf()` and `scanf()` to specify the type of data being displayed or read.

| Format Specifier | Description |
|---|---|
| `%d` | Displays or reads a signed decimal integer. |
| `%u` | Displays or reads an unsigned decimal integer. |
| `%o` | Displays an integer in octal format. |
| `%x` | Displays an integer in lowercase hexadecimal format. |
| `%X` | Displays an integer in uppercase hexadecimal format. |
| `%f` | Displays a floating-point number in decimal format. |
| `%e` | Displays a floating-point number in scientific notation. |
| `%c` | Displays or reads a single character. |
| `%s` | Displays or reads a string of characters. |
| `%ld` | Displays or reads a long integer. |

## 3. Input/Output Functions

### `scanf()`

The `scanf()` function is used to read formatted input from the user through the keyboard.

Example:

```c
scanf("%d", &age);
```

### `printf()`

The `printf()` function is used to display formatted output on the screen.

Example:

```c
printf("Hello World");
```

### `getchar()`

The `getchar()` function reads a single character from standard input.

Example:

```c
ch = getchar();
```

### `putchar()`

The `putchar()` function displays a single character on the screen.

Example:

```c
putchar(ch);
```

### `fgets()`

The `fgets()` function reads a line of text from an input stream, such as the keyboard.

Example:

```c
fgets(name, sizeof(name), stdin);
```

### `puts()`

The `puts()` function displays a string followed by a newline.

Example:

```c
puts("Hello World");
```

## 4. Escape Sequences

Escape sequences are special character combinations used inside strings and character constants.

| Escape Sequence | Meaning | Example |
|---|---|---|
| `\n` | New line | `printf("Hello\nWorld");` |
| `\t` | Horizontal tab | `printf("Name:\tMahek");` |
| `\\` | Backslash | `printf("\\");` |
| `\"` | Double quotation mark | `printf("\"Hello\"");` |
| `\'` | Single quotation mark | `printf("\'A\'");` |
| `\b` | Backspace | `printf("AB\bC");` |

## 5. Precision

Precision controls the number of digits displayed after the decimal point when printing floating-point values.

In `printf()`, precision is specified using a dot followed by a number between the `%` sign and the conversion specifier.

For example:

```c
printf("%.2f", 12.3456);
```

Output:

```text
12.35
```

Another example:

```c
printf("%.3f", 12.3456);
```

Output:

```text
12.346
```

Here, `.2` displays two digits after the decimal point, while `.3` displays three digits.
