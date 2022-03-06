# check the branches
* git branch

# switch to development branch from feature branch
* git checkout develop

# switch to new branch
* git checkout -b <feature_branch_name>

# merge feature to development branch
* git checkout develop
* git merge --no-ff <feature_branch>

# push changes to remote branch
* git push origin develop

# create and switch back to another branch
*git checkout -b <feature_branch2>

# delete a branch
* git branch -d <branch_name>

# Pull the latest changes on the develop branch down
* git pull

# Push the changes up to the remote repository
* git push origin develop
    next step:
    Merge the develop branch into the master branch
    git merge --no-ff develop

    Push the changes up to the remote repository
    git push origin master

# log
* git log
* git checkout version_number_from_log
