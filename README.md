# openssl-wrappers
Encrypt/Decrypt files easily using these two commands: enc dec


## Encrypt a file using enc
(Adds .enc extension)

```bash
enc <FILENAME>
```
Example:
```
$ enc filename.txt
Encrypting file: filename.txt.
Enter a password: <typed_password_is_hidden>
$ ls
filename.txt.enc
```
## Decrypt a file using dec
(removes the .enc extension)

```bash
dec <FILENAME.ENC>
```
Example:
```
$ dec filename.txt.enc
Decrypting filename.txt.enc -> filename.txt
Enter the decrypt password: <typed_password_is_hidden>
$ ls
filename.txt
filename.txt.enc
```
