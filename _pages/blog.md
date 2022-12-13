---
permalink: /blog/
layout: single
title: Blog
---

# Getting started using Github

1. Setup SSH key for git

Adding an SSH key means that each time you make a commit to github, you don't need to put in your github login information each time.

Follow the instructions [here](https://help.github.com/articles/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent/).

You only need to perform this step once

2. Create new repository on your organization's (i.e. company or academic lab) repository on Github
* Click “new”
* Create a name
* Select a license

3. On Github, fork the new repository to your personal repository

4. Clone the repository to your local machine
* On forked branch click “clone & download”
* In your local terminal run the command:
`$ git clone git@github.com:<user name>/<repository name>`

(Local repo) Create upstream branch
$ git remote add upstream <repository git@github.com:greenelab/Pseudomonas_latent_spaces.git>
(Local repo) Create a new branch and where to push changes to
$ git checkout -b <branch name>
$ git push -u <origin or upstream> <branch name>
This allows you to sync local repo with forked repo (your github) and eventually Greenelab
Origin (your github), upstream (Greenelab)
Warning: Do not touch “master” or “upstream/master” branch
(Local repo) Update branch
Convert jupyter notebooks to python script:
$ jupyter nbconvert --to=script --FilesWriter.build_directory=nbconverted*.ipynb
Perform the following steps each time you have a change you want to add to your personal github
$ git add <file name>
$ git commit -m “message/description”
$ git push
(Github) Create pull request (PR)
You have made significant changes to your personal github and you would like to add them to Greenelab.
Click “Compare and PR”
Add reviewer on the right bar
Add comment
Click “Create PR”
Once is approved
On github PR click “squash and merge”
On github PR click “delete branch”
At this point, Greenelab master branch is at the same level as my github branch and my local repository branch
(Local repo) Update master branch
Now we need to update my local master AND with my personal github master to include the new changes that were on my branch
So we switch to my local master
$git checkout master
Grab the changes from the Greenelab master
$git fetch upstream 
Merge changes in Greenelab master with our local master
$git merge upstream/master
So now our local master is up to date
Push those changes to our github master
$git push
So now our personal github master is up to date
Remove local branch
git branch -d <branch name>
Back to #6 and repeat
To update if made changes on another machine:  $ git pull
