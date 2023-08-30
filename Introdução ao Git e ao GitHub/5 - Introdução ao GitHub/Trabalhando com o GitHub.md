#Git #DIO 

# Linking Git to GitHub
First of all, you'll need to create a GitHub repository. When you've created it, you can copy the URL, and type the following command in your local directory:
```bash
git remote add origin url
```

if you want to see the list of remote repositories you can type:
```bash
git remote -v
```

# Push
To push our local commits to our remote repository, we can type the following comanda - Note that you've to certify that the remote repository have been setup as exemplified bellow:
```bash
git push -u origin main 
```

