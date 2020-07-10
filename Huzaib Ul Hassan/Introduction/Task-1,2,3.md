# Task-1

## 1) What do you mean by git and GitHub?

Git is a distributed version control system allowing us to have control over all the previous versions of our files as well as allowing easy collaboration and community tasks.
Git allows us to easily rollback to previous versions and also work at multiple versions simultaneously with the help of branches 
GitHub is a hosting service or website for all our projects and files allowing us the full implementation of git. It is the best way of contributing and learning in the field of open-source.


## 2) Why GitHub is so popular and used in most of the projects?

GitHub is very popular due to its vast community and huge impact on open-source development.
People get help from other people in the form of contributions and hence reveal the real meaning of open source.
It is used in most of the projects nowadays because every project requires to have a version control system as well as contribution from the open source community.

## 3) What is a version control system? How git is a VCS?

A version control system is a system allowing us to have control and record over different versions of our project. Git is a version control system as it allows all the respective functionalities along with features like committing to open source projects. All this is done in a distributed fashion i.e, every project has a server repo and a local repo thus eliminating the chances of loss. Hence it is a really powerful DVCS.

## 4) What are the other platforms similar to GitHub?

* Gitlab
* Bitbucket
* SourceForge
* Apache Allura
* GitKraken

## 5) Why are you interested in learning git and GitHub?

It is essential for every project so as to get help in debugging. Additionally, I want to start contributing in open source and become a part of this vast community. Also, I want to participate in GSOC. Nowadays GitHub has become a portfolio for programmers and I want to create an impressive GitHub profile.

# Task-2

1) Share the link to the GitHub repository you have created?

[Repo](https://github.com/Huzaib/Binary-Search-Using-Divide-And-Conquer)


2) Your README should contain a brief about the project and should be written in markdown language.

[README](https://github.com/Huzaib/Binary-Search-Using-Divide-And-Conquer/blob/master/README.md)


## a) How git workflow works?

It consists of our Workspace, Staging Area, Local Repo and Remote Repo.
Developers start by cloning the remote repository. In their own local copies of the project, they edit files and commit changes however, these new commits are stored locally - they're completely isolated from the remote repository.
To publish changes to the official project, developers "push" their local master branch to the remote repository.


## b) What are the different stages of a git project as commit, add?

init- To initialise a git repository
add- To add our project to staging area
commit- To add all our files in our staging area to our local repo
push- To add our files in the local repo to the remote repo
fetch- To get files to local repo from remote repo
merge- To merge the files to our workspace
pull- fetch+merge


## c) Is it possible to do a commit before git add, if you have made any changes? Explain why?

No, we can commit only the files in the staging area and we have to git add them to get them in the staging area first. Git cannot track the files that are not present in the staging area and hence git commit is not possible before git add. Hence to have the files in the local repo we have to perform git add plus git commit in the same order.


## d) Why is git diff used?

It is a command to see the differences between files in our staging area and our workspace. It can be used to check before committing whether all the changes are added to the staging area before committing to the local repo. Hence helping us to not miss any file or changes within a file before pushing. The files changed  are shown in red. Git log can be used to track all the changes in decreasing order of their occurrences.


## e) Can we leave the commit message blank?

Yes we can. It is just for our convenience to give every commit a commit message. But it is a good practice to add a commit message because it helps us remember the changes we made in each and every commit.


# Task-3

## 1) Share the links of the two PRs?

[PR-1](https://github.com/Huzaib/Git-Series/pull/1)
[PR-2](https://github.com/codewayy/github_series/pull/125)

## a) What is meant by the term fork and clone?
  
Forking allows us to get a copy of someone else's repository on our remote repository so that we can work with it and then suggest certain changes or additions to it.
Any changes to the original repository will be reflected back to our forked repository.
Clone allows to copy the project we forked from our remote repository to our workspace. To add the changes made in our forked repository to the actual repository, we have to create a pull request to the original repository. If the pull request is accepted by the project administrator, the changes will be merged to the original repository.


## b) What are branches in Git?

Git branch is a feature in git used for separating a feature or part of code from master in order not to mess something in our main code
Branches allow us to work over separate parts of the project or code without affecting the master branch (main working code). By default everything is stored in the master branch and when we create a new branch, the same files are copied and we can make changes to it without affecting the files in the master branch. We can add these changes to the master branch or any other branch whenever we want by merging the two branches.


## c)What is PR?

PR or pull request is a feature utilised whenever we want to contribute to someone else's repository. Pull requests let you tell others about changes you've pushed to a GitHub repository. In order to contribute to anyone else's project we create a pull request with the title and the description of the changes we want to make. If the project administrator finds the changes useful, he can accept the PR and merge. Creating a PR is subject to merge conflicts. We can only create a PR if there are no unresolved merge conflicts.


## d) Can we delete the master branch? If not, why?

We cannot delete the master branch as such because master is the default branch for every project we create. In order to delete this, we need to create a separate branch, make this branch the default branch on GitHub, delete this branch on the local repository and then delete this branch on the remote repository.
In the local repository:-
git branch new
git checkout new
git branch -D master
Make GitHub look at new branch:-
git checkout new
git push origin new
Set the default branch to new on. GitHub
Now
git push origin :master
But this way we have just essentially changed our default branch and deleted it and not deleted default master branch.



## e) How can we delete a branch?(Explain a bit about this yourself)

Git does not let us delete the branch we are currently on so we must make sure to checkout to a branch that we are not deleting. For example: git checkout master

To delete a branch locally:
git branch -d localBranchName

To delete a branch remotely:
git push origin --delete remoteBranchName