---
title: Getting started with github
toc: true
toc_label: "github"
---

1. Setup SSH key for git

Adding an SSH key means that each time you make a commit to github, you don't need to put in your github login information each time.

Follow the instructions [here](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/).

You only need to perform this step once

2. (On Github) Create new repository on your organization's (i.e. company or academic lab) repository
* Click “new”
* Create a name
* Select a license

3. (On Github) Fork the new repository to your personal repository

4. (On Github) Clone the repository to your local machine
* On forked branch click “clone & download”
* In your local terminal run the command:
```
$ git clone git@github.com:<user name>/<repository name>
```

5. (Local repository) Create upstream branch,
```
$ git remote add upstream <repository git@github.com:<organization repository name>/<repository name>.git
```

6. (Local repository) Create a new branch and where to push changes to
```
$ git checkout -b <branch name>
$ git push -u <origin or upstream> <branch name>
```
This allows you to sync your local repository with the forked repo (your personal Github) and eventually the organization's repository. 

If you call `$ git remote -v` you will see that origin is your personal Github and upstream is your organization's Github.
**Warning:** Do not touch “master” or “upstream/master” branch

7. (Local repository) Make changes on your branch

Perform the following steps each time you have a change you want to add to your personal github
```
$ git add <file name>
$ git commit -m “message/description”
$ git push
```

8. (On Github) Create a pull request (PR)
At this point you have made significant changes to your personal Github and you would like to add them to the organization's Github.
* Click “Compare and PR”
* Add reviewer on the right bar
* Add comment
* Click “Create PR”

9. Merge PR
When your PR is approved:
* On github PR click “squash and merge”
* On github PR click “delete branch”
At this point, the organization's master branch is at the same level as your personal Github branch and your local repository branch

10. (Local repository) Update your local master branch
Now we need to update your local master AND with my personal github master to include the new changes that were on your branch.

* First, we switch to your local master: `$git checkout master`
* Then grab the changes from the organization's master branch: `$git fetch upstream` 
* Then merge the changes in the organization's master with your local master: `$git merge upstream/master`

Now your local master is up to date.
Push those changes to our github master: `$git push`

Now our personal github master is up to date
11. Remove local branch
```
git branch -d <branch name>
```

12. You can continue to make more changes to this repository by going back to #6 and repeat the subsequent steps
