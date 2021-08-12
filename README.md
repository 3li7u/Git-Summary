# Git Test

this is just a local repository for testing GIT & GitHub

# Git Install:

    You can download Git for free from the following website: [https://www.git-scm.com/]

# Git Commands:

    - To check if Git is installed or not:
    $ git --version

    - To set the username and mail:
    $ git config --global user.name "[USERNAME]"
    $ git config --global user.email "[EMAIL]"

    - To Initialize an empty Git repository:
    $ git init

    - To check the status of all files in repo [Untracked, Added/Staged, Changed, Committed]:
    $ git status

    - To add/stage an Untracked file or changed file to be a Staged file:
    $ git add [file.name]
        - New file in repo is [Untracked file] U
        - Modified file in repo is [Changed file] M
        - To save the two types of files above [U & M] we use $ git add to be a [Added or Staged files] A

    - To Commit a staged files:
    $ git commit -m "[MESSAGE]"
        - Committed files are a save point you can go back to if you find a bug

    - To list all commits for a repository:
    $ git log 

    - To create new branch:
    $ git branch [BRANCH-NAME]
    - To list all branches
    $ git branch
    - To moving us from the current branch, to specific one:
    $ git checkout [BRANCH-NAME]
    - To delete a specific branch:
    $ git branch -d [BRANCH-NAME]

    - To merge current branch with specific branch
    $ git merge [BRANCH-NAME]

# GitHub Commands:

    - Go to [https://github.com/] and sign up for an account, Remember to use the same e-mail address you used in the Git config.

    - Create a repo on GitHub

    - To push a local repository to GitHub:
    $ git remote add origin [REPO-URL]
    $ git push --set-upstream origin master

    - Note: Since this is the first time you are connecting to GitHub, you will get some kind of notification you to authenticate this connection.

    - To fetch changes from GitHub: To see what has changed on GitHub in this repo:
    $ git fetch origin

    - To merge our current branch with remote GitHub branch:
    $ git merge origin/[BRANCH-NAME]

    - To Pull [fetch and merge] all changes from a remote repository into the local branch you are working on:
    $ git pull origin

    - To push your changes from local repo to GitHub:
    $ git push origin

    - Branches on GitHub:

    - To list remote branches:
    $ git branch -r

    - To pull Branches:
        - You can create new branch on GitHub and use:
        $ git pull origin : To get it local as remote branch.
        - Then you can switch to local new branch by:
        $ git checkout [NEW-GITHUB-BRANCH] : And work on it locally.

    - To push a local new Branch to GitHub:
        - create a new local branch by:
        $ git checkout -b [BRANCH-NAME]
        - and push that to GitHub
        $ git push origin [BRANCH-NAME]
        - Now you have a pull request on your GitHub repo you can confirm it and merge it with master branch

# GitHub Pages:

    - In your GitHub repo navigate to: [settings] > [pages] then select branch to deploy your project on GitHub pages
    - you will get the link to your as [USERNAME.github.io/YOUR-PROJECT/index.html]
