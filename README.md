
# <b> About This Repository
<p> This Repository is created for Git and GitHub uses and commands.</p>

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

