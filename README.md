
<div align="center">

  #  **`About This Repository`**

  ## This Repository is created for Git and GitHub uses and commands.

</div>

</br>

# Menu

- [About This Repository](#about-this-repository)
- [Git Commands](#git-commands)
- ### [Local](#local)
- [Git Initializing](#git-initializing)
  - [git init](#git-init)
  - [Git Status: Inspecting a Repository](#git-status-inspecting-a-repository)
  - [Git Staging: `git add`](#git-staging-git-add)
      - [Types of `git add` command](#types-of-git-add-command)
  - [Git Commit: `git commit`](#git-commit-git-commit)
      - [Type of `git commit`](#type-of-git-commit)
  - [Git Add and Commit one line: `git commit -am "message"`](#git-add-and-commit-one-line-git-commit-am-message)
- [Git History](#git-history)
  - [Git Log](#git-log)
  - [Git Log with Graph](#git-log-with-graph)
  - [Git Log with Graph and One Line](#git-log-with-graph-and-one-line)
  - [Git Log with Graph and One Line and Decorate](#git-log-with-graph-and-one-line-and-decorate)
  - [Git Log with Graph and One Line and Decorate and All](#git-log-with-graph-and-one-line-and-decorate-and-all)
  - [Git Log with Graph and One Line and Decorate and All and Date](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author and Grep](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author-and-grep)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author and Grep and Ignore Case](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author-and-grep-and-ignore-case)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author and Grep and Ignore Case and Search Word](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author-and-grep-and-ignore-case-and-search-word)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author and Grep and Ignore Case and Search Word and Search Word](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author-and-grep-and-ignore-case-and-search-word-and-search-word)
  - [Git Log with Graph and One Line and Decorate and All and Date and Author and Grep and Ignore Case and Search Word and Search Word and Search Word](#git-log-with-graph-and-one-line-and-decorate-and-all-and-date-and-author-and-grep-and-ignore-case-and-search-word-and-search-word-and-search-word)
- [Git Branch](#git-branch)
    - [Creating Branch](#creating-branch)
    - [Switch to a Branch](#switch-to-a-branch)
    - [Delete Branch](#delete-branch)
    - [Show all Branches List](#show-all-branches-list)
    - [Rename a Branch](#rename-a-branch)
- [Git Restore and Git Undo](#git-restore-and-git-undo)
    - [git reset](#git-reset)
    - [Undo un-stage changes](#undo-un-stage-changes)
- [Git Count Commits | Short Log View](#git-count-commits-short-log-view)
    - [`git shortlog`](#git-shortlog)
    - [`git rev-list --count <branch>`](#git-rev-list---count-branch)
    - [`git rev-list --count --all`](#git-rev-list---count--all)

- ### [Remote](#remote)
  - [Git Connection to Local Project](#git-connect)
    - [Git Remote to Local Connect](#git-remote-to-local-connect)
    - [Git Local to Remote Connect](#git-local-to-remote-connect)
  - [Git Push](#git-push)
  - [Git Pull](#git-pull)
  - [Git Fetch](#git-fetch)
  - [Git Remote](#git-remote)
  - [Git Remote Add](#git-remote-add)
  - [Git Remote Remove](#git-remote-remove)
  - [Git Remote Rename](#git-remote-rename)
  - [Git Remote Show](#git-remote-show)
  - [Git Remote Prune](#git-remote-prune)
  - [Git Remote Set-Url](#git-remote-set-url)
  - [Git Remote Get-Url](#git-remote-get-url)
  - [Git Remote Set-Branches](#git-remote-set-branches)
  - [Git Remote Set-Head](#git-remote-set-head)
  - [Git Remote Set-Branch](#git-remote-set-branch)
  - [Git Remote Set-Url](#git-remote-set-url)


<br/>

## 1. Start Controlling With Git
## [Local](#local)
### [Git Initializing](#git-initializing)
- ### [git init](#git-init)
  - First of all you have to initialize git in that directory. For Initialize git in any directory follow the steps bellow.
    ```git
      git init
    ```
  - After having (.git) folder in your directory git wil start tracking all the changes in that directory.
  - If you want to remove git from that directory then just delete the (.git) folder from that directory.

- ### [Git Status: Inspecting a Repository](#git-status-inspecting-a-repository)
  - The git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git. Status output does not show you any information regarding the committed project history. For this, you need to use git log.
    ```git
      git status
    ```

<br/>

## [Remote](#remote)
### [Git Connection to Local Project](#git-connect)

- ### [Git Remote to Local Connect](#git-remote-to-local-connect)

  - HTPS
    - https://github.com/ repository link
      ```git
        git clone https://github.com/ repository link
      ```
  - SSH
    - git@github.com: repository link
      ```git
        git clone git@github.com: repository link
      ```
  - Specific Branch
    - git@github.com: repository Or https://github.com/ repository link
      ```git
        git clone -b <branch> <remote_repo>
      ```
  - Specific Directory
    - git@github.com: repository Or https://github.com/ repository link
      ```git
        git clone <remote_repo> <directory>
      ```
- ### [Git Local to Remote Connect](#git-local-to-remote-connect)
    - First create a new repository in GitHub with the name of branch is main, Then redirect to your local project and run the following command
      ```git
        git init
        git add .
        git commit -m "message"
        git checkout -b main
        git branch -D master
        git remote add origin <remote_repo>
        git push -u origin main
      ```
      - The following commend will add your project to GitHub repository in main branch and delete your local master branch.
  

<br/>

### 1. <b>Git Initializing </b>

<br/>

<h1 align="center">Git Status : Inspecting a repository</h3>

<p> <i> The git status command displays the state of the working directory and the staging area. It lets you see which changes have been staged, which haven’t, and which files aren’t being tracked by Git. Status output does not show you any information regarding the committed project history. For this, you need to use git log. </i> </p>

```git
    git status
```


<br/>
<br/>

<h1 align="center">Git Staging : git add</h3>

<p> <i> It will add all the untrack files into staging area for commit. </i> </p>

<br/>

```git
    git add [something]
```

<br/>

## Types of  `git add` command

  1. Stage all the untracked files.

      ```git
        git add .
      ```

      ```
        git add -A
      ```


  2. Stage Specific files
      ```git
        git add file_path
      ```

  3. Stage Specific changes from all files
      ```
        git add -p
      ```


<h1 align="center">Git Commit : git commit</h3>

<p> <i> Commit helps to track what changes is done in that file. </i> </p>

<br/>

## Type of `git commit`
1. commit with a single message
   ```git
      git commit -m "message"
   ```
2. comit with title and messages
   ```git
      git commit -m "title" -m "messages"
   ```

<h1 align="center">Git Add and Commit one line : git commit -am "message"</h3>

<p> <i> This command helps to add and commit at a same time one single line </i> </p>

<br/>

1. add and commit with a single message
   ```git
      git commit -am "message"
   ```


<h1 align="center" id="git-branch">Git Branch</h3>

<p> <i> Branch helps to handle projects </i> </p>

<br/>

```git
  git branch
```

<p>Show all the branches</p>

<br/>

### 1. Creating Branch

<br/>

- First one is for creating branch and at the same time switch to tha enew branch which was created locally.

  ```git
    git checkout -b branch_name
  ```

- Second one just create a new branch

  ```git
    git branch branch_name
  ```

- Create branch remote repository

  ```git
    git push -u origin branch_name
  ```

<br/>

### 2. Switch to a branch

- First one is for creating branch and at the same time switch to tha enew branch which was created.

  ```git
    git checkout -b branch_name
  ```

- Second one is fow direct switch to the branch

  ```git
    git checkout branch_name
  ```

<br/>

### 3. Delete branch

- Delete local branch

  - Delete local branch after merge

    ```git
      git branch -d localBranchName
    ```

  - Delete local branch without merge. Force Delete

    ```git
      git branch -D localBranchName
    ```

- Delete remote branch

  - Delete remote branch

    ```git
      git push origin --delete branch_name
    ```

<br/>

### 4. Show all branches list

- Show all branches locally

  ```git
    git branch -a
  ```


### 5. Rename a branch

  - Rename the current branch

    ```git
      git branch -M name
    ```


<br/>

<h1 align="center" id="">Git Restore and Git Undo</h3>

##  ***[`git checkout`] | `git clean` | `git revert` | [`git reset`](##`git-reset`) | `git rm`***

</br>
</br>

<h2 id="git-reset">git reset</h2>

  Undo changes to the last commit

- <p>Undo most recent commit for git local</p>

    ```git
      git reset head~1
    ```

 - <p>Undo the last second commit for git local</p>

    ```git
      git reset head~2
    ```

## 2. Undo un-stage changes
  <p>Undo the un-stage changes</p>

  - For all un-staged files in current working directory use:

    ```git
      git restore .
    ```

  - For a specific file use:

    ```git
      git restore path/file_name
    ```

<h1 align="center" id="git-count-commits-short-log-view">Git Count Commits | Short Log View</h3>

##  ***[`git shortlog`](#git-shortlog) | [`git rev-list --count <revision>`](#) | `git rev-list --count --all`***

</br>
</br>

## `git shortlog`

Show all the logs in one line as assending order 

```git
  git shortlog
```

</br>
</br>

## `git rev-list --count <branch>`

Show all the logs and logs count for specific branch 

```git
  git rev-list --count main
```

</br>
</br>

## `git rev-list --count --all`

Show all the logs count

```git
 git rev-list --count --all
```