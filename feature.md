# How do we create a feature branch and how to work on it.
## Its always work like this
1. We need to create a feature branch from the developer branch only
2. Give the appropriate feature name so it wouldn't be difficult to track the naming of a feature.
3. Push the changes to the remote repository which will help the people to review on the changes and help to make the pipeline which would test the code.
4. Upon successfull evaluation we shall merge the changes to development branch and perform the pipeline for the particular changes and look for the successfull builds.
5. Then merge the changes to the release branch from the master branch.
6. Delete the feature branch if we need we can go back to the commit and checkout from their to fix the issues.
7. git rebase , git reset will help to work.

## The naming conventions to create feature branch are:
### git branch -b feature/<feature-name>
### git push <remote-name> feature/<feature-name>
### git push <remote-name> --delete <feature-branchname>;  will delete the branch from the remote
### git branch -d <branch-name>; will delete branch locally.
## Delete the branch after successful evaluation.

