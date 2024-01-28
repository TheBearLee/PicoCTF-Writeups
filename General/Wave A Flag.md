Wave A Flag is about the `chmod` command
```
chmod [arguments] [file]
```

This command changes the file permissions of the file.

1. Download the file from PicoCTF

Following the website, download the file from the PicoCTF

2. Attempt the `cat` command

Upon first glance, I tried using the CAT command to see if the flag was just printed on the file. 

Instead of a flag, I received non human-readable characters which meant the file contents were encrypted in some way. 

So, I needed to find another way-

3. Use the `ls -l [file]` command to check file permissions

This command lists the file permissions of a specific file in the form of 
```
-rwx rwx rwx owner group 
```

R: Read
W: Write
X: Executable

Represents:
 a. File permissions of owner
 b. File permissions of group
 c. File permissions of others
 d. Owner of file
 e. Group that owns file

4. Use `chmod` to change the file permissions to executable

In order for us to access the code inside the file, use the `chmod u=rwx warm` to change the file permissions of the user (owner) to everything

5. Follow the steps of the file

The file suggests that we add the `-h` argument in order to learn more about the file.

The `-h` argument normally gives useful information about how to use a file yet not all files have a help argument setup.

From this we can submit the flag!