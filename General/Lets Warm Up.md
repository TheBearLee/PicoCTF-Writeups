This CTF simply tests your cryptography and conversion knowledge.

1. Identify the type of number that is given in the challenge

The challenge gives you the hexadecimal of 0x70 and tells you to change it to ASCII, but how do we know this is hexadecimal?

Hexadecimal almost always starts with "0x" so this is our tip off. Now hexadecimal stands for "base 16" (hexa - 6, decimal - 10). To do this by hand we can check!

In conversions such as this, we read from right to left. So we do 16^0 * 0. This of course is zero.

Then we do 16^1 * 7, which is 112.

2. Convert from decimal to ASCII

We can use a simple ASCII table to map the digit 112 to a letter which happens to be "p".

Submit the flag!