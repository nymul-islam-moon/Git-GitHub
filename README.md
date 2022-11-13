
<div align="center">

  #  **`About This Repository`**

  ## This Repository is created for Git and GitHub uses and commands.

</div>

</br>

# Menu

- <h2 id="git-branch-1"> <a href="git-branch-2"> Git Branch </a></h2>

<!-- - <h2>Git Branch</h2> -->


<!-- - ## [Git Branch](#git-branch-1) -->


<br/>

# Git Commands

~~jdsfjhds fdskjh sdfhsdfhdsfkh sdkhdfj~~

## 1. Start Controlling With Git

### There are two ways to control with git or initialize git

- Git Initialize

- Git Clone

<br/>

### 1. <b>Git Initializing </b>

---

<p>For Version Controlling with you have to initialize git in that directory. For Initialize git in any directory follow the steps bellow.</p>

```git
  git int
```
<p>This command will create a folder called (.git) in that directory</p>


<br/>

### 2. <b>Git Clone </b>
<p>The Second methode for version controll with git is to clone any repositoy from github using HTTPS or SSH key</p>

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

<p>After having (.git) folder in your directory git wil start tracking all the changes in that directory.</p>

<br/>
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

<h1 align="center" id="git-branch-2"> <a href="git-branch-1"> Git Branch</h3>

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

<h1 align="center">Git Restore and Git Undo</h3>

##  ***[`git checkout`](##`git-reset`) | `git clean` | `git revert` | `git reset` | `git rm`***

</br>
</br>

## `git reset`

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