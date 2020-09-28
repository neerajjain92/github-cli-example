# Github CLI Example
 
## Installation
- CLI can be installed using the steps mentioned in [https://cli.github.com/](https://cli.github.com/)

## Command used
1. Authenticate the Github CLI `gh` with your github.com account using `gh auth login`
```
❯ gh auth login

? What account do you want to log into? GitHub.com
- Logging into github.com
? You're already logged into github.com as MovingToWeb. Do you want to re-authenticate? Yes
? How would you like to authenticate? Login with a web browser

! First copy your one-time code: F960-6144
- Press Enter to open github.com in your browser...
✓ Authentication complete. Press Enter to continue...

? Choose default git protocol HTTPS
- gh config set -h github.com git_protocol https
✓ Configured git protocol
✓ Logged in as MovingToWeb
```

2. Create new repo using `gh repo create`. 
```
❯ gh repo create github-cli-example

? Visibility Public
? This will create 'github-cli-example' in your current directory. Continue?  Yes
✓ Created repository github-cli-example on GitHub
? Create a local project directory for github-cli-example? Yes
Initialized empty Git repository in /Users/neeraj/Projects/github/neerajjain92/github-cli-example/.git/
✓ Initialized repository in './github-cli-example/'
```

3. Add a new file in the empty repo, commit it and push it to remote repository (github.com)
```
touch Readme.md
❯ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	Readme.md

nothing added to commit but untracked files present (use "git add" to track)
❯ git add Readme.md
❯ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   Readme.md

❯ git commit -m "Added Readme.md" .
[master (root-commit) 8de23a9] Added Readme.md
 1 file changed, 38 insertions(+)
 create mode 100644 Readme.md
❯ git push origin master
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 921 bytes | 921.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/neerajjain92/github-cli-example.git
 * [new branch]      master -> master
 ```