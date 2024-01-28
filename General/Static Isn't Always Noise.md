# Static Isn't Always Noise

Finally a challenge that has multiple solutions! I will cover each down below. 

# Download the files from PicoCTF

From the site, you will receive files `static` and `ltdis.sh` 

# PROCESS 1

## Use the BASH script given to you

When running the Bash script using `./ltdis.sh` you receive a message that you need a file argument.

Once you add this argument, two new files populate- "static.ltdis.strings.txt" and "static.ltdis.x86_64.txt".

## Read from the `strings.txt` file

To do this, you can use `cat` or simply just open the file with any text editor available to you.

From reading the contents manually, you can quickly find the flag within the first several lines and submit!

# PROCESS 2

Once I learned that the flag was simply a string within the contents of the `static` file, I attempted to use the `strings` command

## Use `strings` on the file

`Strings` is a command that strips all the human-readable text from a non-text file (binary files). This is very useful when looking for text within coding programs that may contain non-printable characters.

## Using piping, use the `grep` command to find the flag

Piping is a very important concept within command line. It simply attaches one command to the output of another.

`Grep` is a search command that looks for certain text within a file/output. Since we know that the flag always starts with "picoCTF{" we can use this in the command line to have a final product of-
```
strings static | grep "picoCTF{}"
```

This will find the flag to submit!
