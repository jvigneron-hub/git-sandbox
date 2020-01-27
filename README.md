# git-sandbox
 Github testing and training
 
Removing a folder
git rm -r <folder name>

Ignoring a previously committed file
If you want to ignore a file that you've committed in the past, you'll need to delete the file from your repository and then add a .gitignore rule for it. Using the --cached option with git rm means that the file will be deleted from your repository, but will remain in your working directory as an ignored file.

$ echo debug.log >> .gitignore
$ git rm --cached debug.log
rm 'debug.log'
$ git commit -m "Start ignoring debug.log"

You can omit the --cached option if you want to delete the file from both the repository and your local file system.

https://www.atlassian.com/git/tutorials/saving-changes/gitignore
