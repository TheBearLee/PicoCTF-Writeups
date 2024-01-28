This challenge focuses on the `grep` command line tool. This is used to find specific patterns within an output.

1. Download the file from PicoCTF

The download will include a file named "file".

2. Use the `grep` tool to find a specific pattern

The `cat` command will output all the content from the file that is readable. Using `grep` we can look for the flag. We know that the flag always begins with "picoCTF{" so we can pass this into `grep` using a pipe to make the command-
```
cat file | grep "picoCTF{"
```

Use this to find the flag and submit!