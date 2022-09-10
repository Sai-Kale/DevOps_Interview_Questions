# GIT

## Pass a message to git commit ?
- git commit -m "comment"

## If you were to make a change for a commit done 30 days   ago with respect to a machine type used? how would you do this change? Would you directly change it?
- Ex: if there is  terraform file where we need to change the instance type which is updated 30 days ago.
    - Here we need to know the engineering best practice & how to handle git.
    - git blame comes to our advantage here.
    - git clone > git branch(create a new branch) > go to github UI > git blame to check change to the history of the file who made what change for what reason > make changes to your code.

## What is Branch protection in Github?
- Suppose dev is working on a feature branch and he makes commit to the master branch, we have to make sure the master is protected so that code is not accepted with an PR raised for merge request.
- got to settings > branches > branch protection rules > Add rule (required PR before merging)
- IF we dont do the setup then anyone can merge something to the master branch