# Git Test

this is just a local repo for testing GIT

# Git Install:

    You can download Git for free from the following website: [https://www.git-scm.com/]

# Git Commands:

    $ git --version : for check if git installed or not

    $ git config --global user.name "[USERNAME]"
    $ git config --global user.email "[EMAIL]"

    $ git init : Initialized empty Git repository

    $ git status : for check the statuse of all file in repo [Untracked, Added or Staged, Changed, Commited]

    $ git add [file.name] : to add [stage] an Untracked file or changed file to be a Staged file
        - Create new file in repo is [Untracked file] U
        - Modifies a file in repo is [Changed file] M
        - to save tow type above we use $ git add to be a [Added or Staged files] A

    $ git commit -m "[MESSAGE]" : to Commit a Stage file
        - Commited files are a save point you can go back to if you find a bug

    $ git log : To view the history of commits for a repo

    $ git branch [BRANCH-NAME] : Create new branch
    $ git branch : view list of branches
    $ git checkout [ANY-BRANCH] : Moving us from the current branch, to specified one
    $ git branch -d [BRANCH-NAME] : delete specified branch

    $ git merge [BRANCH-NAME] : Merge current branch with specified branch

# GitHub Commands:

    - Go to [https://github.com/] and sign up for an account, Remember to use the same e-mail address you used in the Git config.

    - Create a repo on GitHub

    - Push Local Repository to GitHub:
    $ git remote add origin [REPO-URL]
    $ git push --set-upstream origin master

    - Note: Since this is the first time you are connecting to GitHub, you will get some kind of notification you to authenticate this connection.

    - Fetch changes from GitHub:
    $ git fetch origin : to see what has changed on GitHub in this repo

    - Merge our current branch (master) with GitHub branch (origin/master)
    $ git merge origin/master

    - Fetch and Merge. It is used to Pull all changes from a remote repository into the branch you are working on.
    $ git pull origin

    - Push Changes to GitHub
    $ git push origin

    - Branches on GitHub:
    $ git branch -r : list of remote branches

    - Pull Branches:
        - you can create new branch on GitHub and use
        $ git pull origin : to get it in local repo as remote branch
        - then you can switch to local new branch by $ git checkout [NEW-BRANCH] and work on it
    - Push a Branch to GitHub
        - create a new local branch
        $ git checkout -b [BRANCH-NAME]
        - and push that to GitHub
        $ git push origin [BRANCH-NAME]
        - now you have a pull request on your GitHub repo you can confirm it and merge it to master branch as all other branches

# GitHub Pages:
    - in your GitHub repo navigate to settings then > pages then select branch to deploy your project on GitHub pages
    - you will get the link to your project [USERNAME.github.io/YOUR-PROJECT/index.html]
