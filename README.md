# Git Test

this is just a local repo for testing GIT

# Git Install:

    You can download Git for free from the following website: [https://www.git-scm.com/]

# Git Command:

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
