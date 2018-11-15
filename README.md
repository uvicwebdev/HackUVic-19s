# HackUVic-19s

The HackUVic Website - Spring 2018; "What the World Needs Now"

## What Did We Use?

* HTML / CSS / Javascript
* [Bootstrap](https://getbootstrap.com/)
* [FontAwesome](https://fontawesome.com/)
* [Github Pages](https://pages.github.com/)
* [Gulp](https://github.com/gulpjs/gulp)
* [SASS](http://sass-lang.com/)
* [Surge](https://surge.sh/)

## Run this Locally!

### Prerequisites

* [git](https://git-scm.com/)
* [NPM](https://www.npmjs.com/)
* Text Editor
* Terminal

### Obtain Local Copy

Clone the repository to your local computer in the directory you're currently in.

```bash
git clone https://github.com/uvicwebdev/HackUVic-19s.git
cd HackUVic-19s
```

### Contribute to the Repo

#### Review and Approval Process

For code quality and every member to be in the know, a review and approval process is in place:

* Feature branches: (ie. design-add_clouds or sponsors-reformat_layout)
* No merging directly into master unless absolutely needed.
* PRs must have two (2) approvals before being merged.

#### Getting Gulp Ready

Scss files need to be converted to css first. To do that, we run gulp. (Note: css files
will always be overwritten when running gulp.) To install all the dev dependencies for the first time:

```bash
npm install
````

To run gulp, go through an npm command. This command also automagically syncs any html/scss/js changes to the browser:

```bash
npm run build
```

#### Creating a Branch and Making Changes

```bash
// Creating a branch
git checkout -b new-branch-name_solving_issue

// Make changes and see what files differ from master
git status

// Add modified files one at a time
git add {$specific file names}
// OR (Danger, danger! Do this sparingly) add ALL files at once
git add .
```

Once small changes have been made, commit and push them.
```bash
git commit -m "Description of Changes"
git push origin new-branch-name_solving_issue
```

When all changes are made, create a PR and wait for the review/approval process.

#### Merging Code

```bash
# update your origin/* pointers
git fetch
 
# checkout the branch you’re merging in (assumes branch-name points to origin/branch-name)
git checkout branch-name
 
# rebase the whole branch onto master:
git rebase origin/master

# update origin/branch name to the new rebased head
git push --force-with-lease origin branch-name
 
# point your master branch to latest origin/master
git checkout master && git fetch && git reset --hard origin/master
 
# merge in the branch and force a ‘merge commit’
git merge --no-ff branch-name -m "Merge 'your-branch-name'"
 
# push your changes; this will automagically resolve the Github PR
git push origin master
 
# if no issue with merge, you can now delete the branch locally
git branch -d branch-name
 
# put this deleted branch back into origin
git push origin :branch-name
```

## Inspiration

* [nwHacks 2019](https://www.nwhacks.io/)
* [HackUVic 2018](http://18w.hackuvic.com/)
* [HackathingUVic 2017](http://www.hackathinguvic.com/)
* [Gulp For Beginners](https://css-tricks.com/gulp-for-beginners/)
