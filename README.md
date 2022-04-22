# Useful Git Commands for Git & Github

# Git Install:
You can download Git for free from the official Git website: [git-scm.com](https://www.git-scm.com/)

# Git Commands:

After intallation, Check if Git is installed or not:
     
     $ git --version

&nbsp;

Set the username and mail:

    $ git config --global user.name "[USERNAME]"
    $ git config --global user.email "[EMAIL]"

&nbsp;

Initialize an empty Git repository:

    $ git init

&nbsp;

Start a demo project and check the status of all project files in your repo
1. Untracked [U] refers to new files [created after repo initialization] in the repo
2. Changed [M] refers to modified files in the repo
3. Added/Staged [A] refers to saved [Untracked & Changed files after add them with *git add* command] files in the repo.
</a>

    $ git status

&nbsp;

Add/Stage Untracked or Changed files to be a Staged files, `add .` to add all files in one time.

    $ git add [file.name]
    $ git add . 

&nbsp;

Commit a staged files: Committed files are a save point you can go back to if you find a bug

    $ git commit -m "[MESSAGE]"

&nbsp;

List all commits for a repository:

    $ git log 

&nbsp;

Create new branch:

    $ git branch [BRANCH-NAME]

&nbsp;

List all branches

    $ git branch   

&nbsp;

Moving from the current branch, to specific one:

    $ git checkout [BRANCH-NAME]

&nbsp;

Delete a specific branch:

    $ git branch -d [BRANCH-NAME]

&nbsp;

Merge current branch with specific branch
    
    $ git merge [BRANCH-NAME]


# Git Commands for remote GitHub repo:

 Go to [GitHub](https://github.com) and sign up for an account\
 Remember to use the same e-mail address you used in the Git config.

Create a new repo on GitHub\
Push your local repository to GitHub:

    $ git remote add origin [GITHUB_REPO_URL]
    $ git push -u origin master

Note: Since this is the first time you are connecting to GitHub, you will get some kind of notification to authenticate this connection.

&nbsp;

Fetch changes from GitHub repo: To see what has changed on GitHub in this repo:

    $ git fetch origin

&nbsp;

Merge current branch with remote GitHub branch:

    $ git merge origin/[BRANCH-NAME]

&nbsp;

Pull [fetch and merge] all changes from a remote repository into the local branch you are working on:

    $ git pull origin

&nbsp;

Push your changes from local repo to GitHub:

    $ git push origin

&nbsp;

Branches on GitHub:\
List remote branches:

    $ git branch -r

&nbsp;

Pull Branches:\
Create new branch on GitHub and get it local as remote branch:

    $ git pull origin

&nbsp;

Switching to the local new branch and work on it locally:

    $ git checkout [NEW_GITHUB_BRANCH_NAME]

&nbsp;

Push a local new Branch to GitHub:\
Create a new local branch and push it to GitHub:

    $ git checkout -b [BRANCH-NAME]
    $ git push origin [BRANCH-NAME]

&nbsp;

Now you have a pull request on your GitHub repo you can confirm it and merge it with master branch.

# GitHub Pages:

Deploy your website to Github pages:
1. Create new github repo
2. Push your local repo to the remote one that you just created.
3. In your GitHub repo navigate to: [settings] then: [pages]
4. If your repo has more than one branch, Select the one that contains your website to deploy it on GitHub pages.
</a>
you will get the link to your website as [USERNAME.github.io/YOUR_REPO_NAME]

&nbsp;

To deploy on the root [USERNAME.github.io]\
Create a new repo with specific name [USERNAME.github.io]\
then repeat the steps from 2 to 4
