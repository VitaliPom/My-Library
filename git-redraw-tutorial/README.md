# git-graph-redraw-tutorial 
git tutorial on one of the hottest topics on how to redraw git history (how to redraw git graph history)

Tutorial on how to create nice looking picture in git graph, like this:

<img src="https://raw.githubusercontent.com/VitaliPom/My-Library/main/git-redraw-tutorial/image.jpeg" height="512px" width="512px">


You do `git commit` after you made `git branch`, you continue to work, until you do `git merge` and even `git push`. There are thousands of tutorials like that, but you don't know the upcoming hustle that will be with your git branch, so usually in development of some big products, `git branch` is omitted and corporations don't usually trust novice developers on how to work with the branch, since they don't know how to clean up. 

**In this tutorial we will continue to learn git, assuming you learnt basics from others and since destruction guaranteed, please create a NEW-fresh-copy of your git local repository directory & please start working on it until you learn and master all the basics that are here.**

------
###Let us begin:
#1
So first of all, before you apply the changes and get disappointed from results, be aware you might get a nasty git graph history with TONs of branches, which are easily deleted by just doing `git push -force`, the reason is that git apps are doing fetch every few minutes or even evert few seconds and the later results once you create a local change is an ugly-ugly tree.

#2
###Basics:
When you are working on redrawing git history graph tools view, you might probably want on the first to learn how to detach tail of a branch and re-attach head of a branch, doing un-merge and re-commit it into a new, another branch.

#2.1
###`git rebase` - git rebase --onto \<newparent\> \<oldparent\>
[https://stackoverflow.com/a/39081674/1017216](https://stackoverflow.com/a/39081674/1017216)

In order to make the existing branch which looks messy to be a child of another branch, you pick up the old parenting pointing commit (paste it in \<oldparent\>), choose the new parenting point you wish the branch to start from and paste there the new commit in \<newparent\> & yeas the order IS correct git rebase new old.

```
git rebase --onto <newparent> <oldparent>
```
---------
