# HackUVic-19s

The HackUVic Website - Spring 2018

## What Did We Use?

* HTML / CSS / Javascript
* [Bootstrap](https://getbootstrap.com/)
* [FontAwesome](https://fontawesome.com/)
* [Github Pages](https://pages.github.com/)
* [Gulp](https://github.com/gulpjs/gulp)
* [SASS](http://sass-lang.com/)

## Links

* [Website]()

## Run this Locally!

### Prerequisites

* [git](https://git-scm.com/)
* [NPM](https://www.npmjs.com/)
* Text Editor
* Terminal

### Obtain Local Copy

Clone the repository to your local computer.

```bash
// Change into your working directory
cd working/directory

// Clone the repository
git clone https://github.com/uvicwebdev/HackUVic-19s.git
```

Go into the folder

```bash
cd HackUVic-19s
```

### Contribute to the Repo

#### Getting Gulp Ready

Scss files need to be converted to css first. To do that, we run gulp. (Note: css files
will always be overwritten when running gulp.) To install all the dev dependencies for the first time:

```bash
npm install
````

To run gulp, go through an npm command. This command also automagically syncs any html/scss/js changes to the browser:

```bash
npm run build
````


#### Creating and Committing Branches

```bash
git checkout -b new-branch-name
```


Add changes

```bash
git add .
```

Commit changes

```bash
git commit -m "Description of Changes"
```

Push changes

```bash
git push origin new-branch-name
```

Submit a pull request

## Inspiration

* [nwHacks 2019](https://www.nwhacks.io/)
* [HackUVic 2018](http://18w.hackuvic.com/)
* [HackathingUVic 2017](http://www.hackathinguvic.com/)
* [Gulp For Beginners](https://css-tricks.com/gulp-for-beginners/)
