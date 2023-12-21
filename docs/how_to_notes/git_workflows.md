# Git Workflows

## What is git
Git is version control software used to enable collaboration between many people on a single project. [This youtube video gives a good synopsis of what git is.](https://www.youtube.com/watch?v=2ReR1YJrNOM)

## Getting started with git

### Making an account
Git is a software technology that is independent of remote repository systems like github, gitlab and bitbucket. However it is almsot used in conjunction with one of these services. This project, and most others, are managed through github. If you don't already, you'll need a github account. [You can make a github account here!](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home)

### SSH keys
In most cases, to start using git on a new computer you need to set up a new SSH key. An SSH (secure shell) key is a method of security control where an ecnrypted key is generated and stored on a client and service. These keys are used when the client trys to connect to the service to verify that both parties are who they say they are.

You'll need an SSH key to clone using SSH rather than https, SSH is genreally considered to be a safer method and is therefore reccomended.

[Follow these directions to generate a new SSH key.](https://github.com/signup?ref_cta=Sign+up&ref_loc=header+logged+out&ref_page=%2F&source=header-home) You can choose to add a passphrase to your SSH key or not. If you do choose to add a passphrase it is recommended that you add the key to an SSH-agent. This will make it so you don't have to type in your passphrase everytime you interact with git. [Follow these instructions to add your key to an SSH agent](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent#adding-your-ssh-key-to-the-ssh-agent)

Now that you've generated an SSH key, [follow these instructions to add your SSH key to your github account](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account#adding-a-new-ssh-key-to-your-account)


## Helpful git commands
[Here is a decent git cheat sheet.](https://about.gitlab.com/images/press/git-cheat-sheet.pdf) This reference covers the basic usage of git. Be aware that the git rabbit hole is deep and things can get complciated fast, so don't be affraid to google specific issues you experience. 


## Basic pull request workflow
Below is outlined a typical workflow for opening pull requests (PR) and participating in code review. This applies when you are working in a shared repo (like this one 😉).
These instructions assume you already have cloned the repo (`git clone <repo address>`) and have made and committed changes (`git add <changed file>` and `git commit -m <commit message>`)

- Before you push your code to open a PR it is a good practice to pull from the main branch to make sure you have the most up-to-date version of the code: On your working branch `git pull origin main`
    - Resolve any merge conflicts
- Push your code to the remote `git push` or if it's your first push on this branch `git push --set-upstream origin <branch name>`
- Open a new pull request. 
    - If you navigate to the repo's page in github shortly after pushing you should see a large green button prompting you to open a PR. 
    - Otherwise you need to click the PR tab, select `New Pull Request` and configure `main <- <your branch>`
- The above steps will open a new PR form, please write a description of your changes. If you are working on an established project it's helfpul to include the steps you used to test your code as well as screen shots. 
- Assign one or more reviewers, or otherwise let folks know you have a PR ready for review
- Once your code has been reviewed there is likely some changes you need to make, you can make changes on your current branch and push them to the remote, the PR will pick up the changes.
    - It's good to make make sure you have the most recent code from `main` before each push back to the PR (`git pull origin main` and then resolve merge conflicts if they exist)
- Once your PR is approved, either you or someone from the project will merge your changes in. This varies from project to project so just ask.