# HackUVic-19s

The HackUVic Website - Spring 2018; "What the World Needs Now"

## What Did We Use?

* HTML / CSS / Javascript
* [Bootstrap](https://getbootstrap.com/)
* [FontAwesome](https://fontawesome.com/)
* [Github Pages](https://pages.github.com/)
* [Gulp](https://github.com/gulpjs/gulp)
* [SASS](http://sass-lang.com/)

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
git push origin your-branch-name
```

When all changes are made, create a PR and wait for the review/approval process.

#### Merging Code

```bash
// After committing changes, go to master
git checkout master

// Optional: done if someone has merged code between the creation of the branch and your changes, or 
// you haven't been rebasing your branch. These commands updates local master to origin master.
git fetch
git reset --hard origin/master
git checkout your-branch-name
git rebase origin/master         // Takes your changes and puts them on top of any new changes
git push origin your-branch-name // Update local branch if you've need needed to recieve changes
git checkout master              // Back to master to continue the merge

// Merge your branch from master
git merge your-branch-name -m "Merge 'your-branch-name'"
git push origin master

// Optional: clean up your branches by deleting them (on git, then locally)
git push origin :your-branch-name // Double check master is OK before net step
git branch -d your-branch-name
```

## Inspiration

* [nwHacks 2019](https://www.nwhacks.io/)
* [HackUVic 2018](http://18w.hackuvic.com/)
* [HackathingUVic 2017](http://www.hackathinguvic.com/)
* [Gulp For Beginners](https://css-tricks.com/gulp-for-beginners/)
