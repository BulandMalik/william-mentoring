# Basic Introduction of Git

## Installing Git
> You must install git to use and create an account on Github. Check out this intro guide [here](https://docs.gitlab.com/ee/gitlab-basics/start-using-git.html).

## Key Terminologies

### Repository
Git at its core work on ```Repositories```. A Git repository tracks and saves the history of all changes made to the files in a Git project. It saves this data in a directory called `.git` , also known as the repository folder. 


### Branch
A branch in Git is simply a lightweight movable pointer to one of the commits. The default branch name in Git is `master` or `main`. As you start making commits, you’re given a master/main branch that points to the last commit you made. Every time you commit, the master branch pointer moves forward automatically.

![](../images/git-branch-cheatsheet.png)

### Git Branching Strategy

### Different Git Stages

Git has three main states that your files can reside in: modified, staged, and committed:

    1. Modified means that you have changed the file but have not committed it to your database yet.
    
    2. Staged means that you have marked a modified file in its current version to go into your next commit snapshot.

    3. Committed means that the data is safely stored in your local database.

This leads us to the three main sections of a Git project: the working tree, the staging area, and the Git directory.

![](../images/git-stages-5.png)
![](../images/git-stages-1.png)
![](../images/git-stages-3.png)
![](../images/git-stages-4.png)

### Git Cloning

    ```git clone [REPOSITORY_URL]```

### Git Init

### Git Fork

Forking is getting a copy of an upstream repository for you. So you can do your own changes freely without affecting the original repository. You can fork a repository as below in the upstream repo.

Once you forked a repository you will have an individual copy of it in your GitHub account.

![](../images/git-stages-2.webp)


### Git Add
    ```
        git add [FILE_NAME]
        git add .
        git add *.txt
        git add docs/
    ```

### Git Commit

### Git Push

### Git Pull

### Git Fetch

### Resolving Conflicts

### Ignoring Files with Git
You may use ```.gitignore``` if you want to hide any file when uploading online. Just simply create a ```.gitignore``` file, and write all the files names you want to ignore.

### Git Cheat Sheet
![](../images/git-cheat-sheet.png)

### Useful Links
1. [Google Free Git Course](https://www.coursera.org/learn/introduction-git-github)
2. [ Interactive Guide to Git Branching](https://learngitbranching.js.org/)
3. [Git For Windows](https://www.udemy.com/courses/search/?src=ukw&q=Command+Line+Essentials%3A+Git+Bash+for+Windows)
4. https://kmtsandeepanie.medium.com/understanding-git-basics-5bd1163dc828
5. https://javarevisited.blogspot.com/2019/05/10-free-websites-to-learn-git-online.html#axzz7sOieMTQx
