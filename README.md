
**Using Git to implement a new feature/change without affecting the main branch**

This blog indicates how to implement a new feature or change without affecting the main Git branch.

Prerequisites:  

Git installed on your local machine
Access to the remove repository

Steps:
Clone the remote repository
 git clone https://github.com/catalinasmeureanu/git_tutorial

Create a new branch for the feature or change you’d like to implement and switch to the new branch
Change directory (cd) to the local project
$  cd git_tutorial

$ git checkout -b my-feature
Update or add the files as needed
Add the changes to be tracked by Git
To track all changes that have been made and files that have been added:
$ git add .
To track just a single file, we can specify that file in our git add command:

$ git add file.txt

Commit the changes
$ git commit -m “Added file.txt”

Push changes to the remote repository
$ git push origin my-feature

depending on the platform used create a Merge Request or Pull Request

The changes can be merged directly to the main branch without creating a Merge Request with the git merge command.

 switch to the main branch, then run the git merge command.
$ git checkout main
$ git merge my-feature

