#Git #DIO #SSH

# SSH Key
SSH is a form of establish a secure and encrypted connection between two computers. In your case, our computer and GitHub. 

To do that, first we need to create an ssh key:
```bash
ssh-keygen -t ed25519 -C example@email.com
```

Now, we need to add the generated key to GitHub, for this, we can simple open the the file in the directory that we have created the ssh key in the step above.

After that, we need to pass the key to the client. But first we need to initialize the SSH client itself. This can be done by the command:
```bash
eval $(ssh-agent -s)
```

And now, we can pass the key:
```bash
ssh-add id_ed25519
```
