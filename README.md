# openssl-wrappers
Encrypt/Decrypt files easily using these two commands: enc dec

## Installation
```
sudo cp enc dec /usr/local/bin
sudo chmod +x /usr/local/bin/enc && \
     chmod +x /usr/local/bin/dec
```

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

## TODO 
- [ ] Add way to display help if nothing is entered 
- [ ] Check to see if a filename was entered as a parameter
