Git Branching
=============

Goal
----

Become comfortable with Git's killer feature. Create new branches, 
switch to new branches, do some work, commit work. Integrate feature
branches into `master`, remove branches which are not needed any more.
Perform fast-forward or the three-way merges. Do some rebasing.

Tasks
-----

* Initialize an empty repository
* Create README.md file and put some contents inside
* Commit the README.md file
* Create CONTRIBUTING.md file and put some contents inside
* Commit the CONTRIBUTING.md file
* Checkout the `experimental` branch
* Update the README.md file
* Commit the changes
* Switch back to the `master` branch
* Checkout the `hotfix` branch
* Do some hotfixing on README.md
* Commit the changes
* Do a fast-forward merge of `hotfix` branch into `master`
* List all the available branches
* List only merged branches
* List branches that were not merged yet
* Remove the `hotfix` branch
* Switch to the `experimental` branch
* Update the CONTRIBUTING.md file
* Commit the changes
* Switch back to the `master` branch
* Do a three-way merge into master (resolve conflicts if there are any)


Solution
--------

* `git init`
* `touch README.md && echo "#Hi all" >> README.md`
* `git add README.md`
* `git commit`
* `touch CONTRIBUTING.md && echo "#Hi all" >> CONTRIBUTING.md`
* `git add CONTRIBUTING.md`
* `git commit`
* `git checkout -b experimental`
* `echo "#Hi all from experimental" >> README.md`
* `git add README.md`
* `git commit`
* `git checkout master`
* `git checkout -b hotfix`
* `echo "#Hi all from hotfix" >> README.md`
* `git add README.md`
* `git commit`
* `git checkout master`
* `git branch -v`
* `git branch --merged`
* `git branch --no-merged`
* `git branch -d hotfix`
* `git checkout experimental`
* `echo "#Hi all from experimental" >> CONTRIBUTING.md`
* `git add CONTRIBUTING.md`
* `git commit`
* `git checkout master`
* `git merge experimental`


