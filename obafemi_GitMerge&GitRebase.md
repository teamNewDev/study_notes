Git: Understanding Merging And Rebasing

Git Merge
Branches are created at different points of a project lifecycle for different reasons; ranging from bug fixing to program testing to new development etc. These changes needs to be integrated into the master branch, more specifically merging takes the contents of a source branch and integrates them with a target branch, this process results in, changes to the target branch while the source branch history remains unchanged.
Merging is done by using the checkout and merge Git commands;
$ git checkout branch_a

$ git merge master

(or)

$ git merge master branch_a

Git Rebase
Another way of integrating changes from one branch to another branch is by taking the patch of the change that was introduced into a source branch and reapply it on top of the target branch. This is called Rebasing in Git. With the rebase command, you can take all the changes that were committed on one branch and replay them on a different branch.
Rebasing is done by using the checkout and rebase Git commands;
$ git checkout feature

$ git rebase master