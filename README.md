- ===> practicing git commands

- git is a version control system & github is a repository to store/manage codes
- "git init" --> to initialize any folder in local system as a repo on github, this will create a hidden folder ".git"
- initially files will say "U" which means untracked.. to track those files, use git add
- then use "git add README.md" to add readme file
- After adding the file, status will change to "A" means added
- check status using "git status"
- now commit all tracked files to temp staging environment which will be pushed to github repo later using "git commit -m 'adding readme file'"
- rename branch to main --> "git branch -M main" & check branch "git branch"
- add the location of repo where you want to push the staged files to using "git remote add origin https://github.com/iamprashantjain/git_practice.git"
- push staged files in main branch to repo using "git push -u origin main"
- After updating readme file.. send updated file to repo by first adding the file in staged environment, update commit msg & then push to repo.
- file status will say "M" which means modified but not staged.. so to update that file to repo.. add the file in staged ennvironment & push
- create a new file ".gitignore" from web interface of github, but since it is not in our local system as it was added from the web, we can use "git pull origin main" to update our local system folder with all files on github repo
- whats the use of ".gitignore" --> to prevent files to be ignored uploading to github repo, lets say we have a virtualenv "venv" for our project, we should not update the virtualenv to github repo
- we can add this folder in gitignore file to be ignored by just writing "venv/"
- now git status is showing 2 filed modified --> readme & .gitignore
- If we run "git add ." which adds everything to staging, it will ignore venv bcoz we have defined it in gitignore file to be ignored
 
