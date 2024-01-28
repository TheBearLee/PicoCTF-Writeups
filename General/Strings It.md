This challenge focuses on the `strings` tool. The `strings` tool finds the human-readable text within a binary file and outputs it for future use.

1. Download the file from picoCTF

You will receive the file called "strings".

2. Use the `strings` command on the file

Trying to just use `cat` on the file prints out a bunch of digits and impossible-to-read jargon. This is where `strings` comes in.

We can use `strings` to find the text that we can actually read! Use the format-
```
strings [filepath]
```

This will give you all the text within the file. You can pipe `grep` to find the specific text you are looking for.

Submit the flag once you find it!