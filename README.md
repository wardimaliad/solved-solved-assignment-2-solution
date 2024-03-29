Download Link: https://assignmentchef.com/product/solved-solved-assignment-2-solution
<br>
How C macros, conditional operator (“?”), and bitwise operators; write a C program that can demonstrate the use of “?” and macros (at some good places in your code) that does:

Always try to use read() and write() system calls for I/O (read keyboard and display).

First, prompt a message (write) asking for keyboard input, then have your last name entered (read) into a character array.

Part A.

Display (write) each bit by alphabet ‘0’ or ‘1’ in each byte of your last name, e.g., if “Chang” is entered:

C 0 1 0 0 0 0 1 1h 0 1 1 0 1 0 0 0a 0 1 1 0 0 0 0 1n 0 1 1 0 1 1 1 0g 0 1 1 0 0 1 1 1

Note the format:separate characters with spaces and put each byte on a line. (A double loop is needed, the outer loop goes through each letter of the name, the inner loop each bit in a byte.)

Part B.

Use the first character from the entered name as a mask-in (bitwise OR) mask for other characters and display them out like that in part A.

Part C.

Use the first character from the entered name as a mask-out (bitwise AND) mask for other characters and display them out like that in part A.

————————————————————————Bonus Part 1. (1 extra-credit point)

Left-shift all bits in each byte one at a time, to find the shifted pattern that is the largest (unsigned) value of all possible shifted patterns, and show the shifted byte like that in part A. e.g., from “Chang” we get:

0 1 0 0 0 0 1 1 — 1 1 0 0 0 0 0 00 1 1 0 1 0 0 0 — 1 1 0 1 0 0 0 00 1 1 0 0 0 0 1 — 1 1 0 0 0 0 1 00 1 1 0 1 1 1 0 — 1 1 1 0 0 0 0 00 1 1 0 0 1 1 1 — 1 1 1 0 0 0 0 0

You only need to show the result side (the right side of above).

————————————————————————Bonus Part 2. (another extra-credit point)

Typical programming-contest problems would ask you to find the size of the largest groups of 0’s and 1’s in the name (consecutive 0’s and consecutive 1’s through out the name string).

Can your code answer these questions from the bit sequence in the original last-name input?

You may want to organize your code to have a subroutine that can be called by each part to display bits from a given string.