# Tab, Tab, Attack

This can be a quite annoying challenge if you do it incorrectly! Make sure to use absolute file paths.

# Download the zip file from picoCTF

You will receive a zip file that is unlocked.

# Unzip the file into a directory that you can access

Using the `unzip` command along with the zip file, you can see all the files that it populates. Looking at the very bottom, you can see it creates a file that is 11 directories deep.

# `Strings` and `grep` the file

Rather than `cd` your way through 11 directories, copy the absolute file path and use `strings` on it to find all the printable text within the file.

Pipe `grep` in conjunction with this output because we know that the flag will always start with "picoCTF{" to make a final command of 
```
strings [filepath] | grep "picoCTF{"
```

This will print the line that contains the flag to submit!
