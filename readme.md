# Git Started


This repository aims to help those who are using git for the first time.

Let's **git started** now haha !


## Configurations

Before getting started, make sure that you have git installed on your computer/laptop
and that it has been already configured.

- To see if git is already installed :

```shell
  git --version
```

- To configure your email :

```shell
  git config --global user.email "email@example.com"
```

- and your username :

```shell
  git config --global user.name "username"
```

## Basics

1) To initialize a repository in the directory you're currently in :

```shell
  git init
```

2) To see which changes have been staged, which haven’t, and which files aren’t being tracked by 
   git you use : 

```shell
  git status
```

3) To tell git that you want to include updates to a particular file in the next commit i.e you 
   want git to track the file :

```shell
  git add file_name
```

4) A commit is the git equivalent of a "save". To do so :

```shell
  git commit -m "commit message"
```
> You run it after tracking one or multiple files with **git add**

5) To see the commit logs :

```shell
  git log
```

6) To link your local repository to your remote repository on GitHub :

```shell
  git remote add origin remote_url
```

7) To upload your local changes to your remote repository :

```shell
  git push -u origin branch_name
```

8) To see all available branches in your repository : 

```shell
  git branch -a
```

> Even remote branches will be displayed

9) To create a new branch :

```shell
  git branch branch_name
```

or if you want to create a new branch and want to switch to it directly :

```shell
  git checkout -b branch_name
```

10) To switch branch : 

```shell
  git checkout branch_name
```

## Advanced

1) To rewind history without changing the contents of your local files :

```shell
  git reset mode commit
```

> mode :
>  - soft
>  - hard 
>  - mixed
> 
> See git documentation for further details

2) To join two or more branches together : 

```shell
  git merge branch_name
```

3) To fetch changes on your remote repository and merge them on your local repository :

```shell
  git pull
```

4) To clone a remote repository into your computer/laptop :

```shell
  git clone remote_url
```

5) If you want to rewrite history :

 - modify your last commit message

```shell
  git commit --amend
```

 - reorder commits 

```shell
  git rebase -i HEAD~parent_of_the_last_commit
```

> then you just move them as you wish.
>> git will give you instructions during the process so don't worry


That's all for now !