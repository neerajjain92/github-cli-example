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

2. Create new repo using `gh repo create`. `TechPrimers/` denotes the organization under which the repository needs to be created.
```
❯ gh repo create TechPrimers/github-cli-example

? Visibility Public
? This will create 'TechPrimers/github-cli-example' in your current directory. Continue?  Yes
✓ Created repository TechPrimers/github-cli-example on GitHub
? Create a local project directory for TechPrimers/github-cli-example? Yes
Initialized empty Git repository in /Users/ajay/Documents/code/github-cli-example/.git/
✓ Initialized repository in './github-cli-example/'
```

3. Add a new file in the empty repo, commit it and push it to remote repository (github.com)