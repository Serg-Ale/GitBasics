#Git #DIO 
# First commands with Git
## git init
To initialize a git local repository, first you go to your local folder/directory and type:
```bash
git init
``` 

output:
```txt
Initialized empty Git repository in "path to your folder/direcotory"
```

This command will create a ` .git ` directory to setup git in your directory.

## git first setup
You need to tell git who you're and what's your email address, to do this, you can type:
```bash
git config --global user.name "your name"
git config --global user.email "your email"
```

You can omit the ` --global ` flag if you want to setup the user and email for only the directory what you're working. Passing the flag ` --global ` will tell git globally, in all the system, who're you and what's your email.

## Tracked ou Untracked
To better understand how git "flow" works, see the example in the image bellow
![[Pasted image 20230824065456.png]]

Inside **Tracked**, we have  3 possible states:
- **Unmodified** -> Files that'd not been modified since the last commit;
- **Modified** -> Unmodified files that have been modified;
- **Staged** -> files prepared to make part of another type of grouping.

And we also have **Untracked**, files that our code versioning is not seeing. 

## Repositories
We've the separation of two environments when we talk about repositories:
![[Pasted image 20230824071251.png]]

## git status
Help us to monitor the status of the files:
```bash
git status
```

## git add
To add an not staged specific change to our "Tracked" area, we can type the following command:
```bash
git add <file_name>
```

Note that this command add only the file that we've specified, to add all the not staged changes, you can type:
```bash
git add .
```

## git commit
To commit (make a snapshot of everything we've staged) we can simple type:
```bash
git commit -m "A message that describe the commits/changes"
```


