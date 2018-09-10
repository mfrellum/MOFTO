https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/

Create a new repository on GitHub. To avoid errors, do not initialize the new repository with README, license, or gitignore files. You can add these files after your project has been pushed to GitHub.

Change the current working directory to your local project.
```
  git remote add origin remote repository URL
  git remote -v
  git push origin master
```
