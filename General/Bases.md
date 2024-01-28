# Bases

This challenge introduces us to basic cryptography, specifically base64

# Identify the type to encryption used

The challenge provides no files and so we are given a string of numbers and characters to start off with. We are tasked with decrypting this in order to submit as a flag.

Although there is not a great way to decipher what type of encryption was used, we can use context clues to help. Based on the ciphertext containing numbers 1-9, and uppercase and lowercase letters in the English alphabet, we can rule out types of encryption such as hex, binary, and ROT13. 

Another common encryption method is base64 which as its name entails, uses a series of 64 characters to encrypt a system. Lets use an online tool to attempt to decrypt this ciphertext using base64.

Using this decoder, we get the flag to submit!

For more information on how base64 works, check out https://www.base64decode.org
