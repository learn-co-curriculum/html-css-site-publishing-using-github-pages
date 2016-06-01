# Site Publishing Using Github Pages

## Overview

In this lesson we will look at how to host a website for free on Github using Github Pages.

## Objectives

1. Setting up a Github.io Github Pages hosted site.
2. Using gh-pages branch to host any repo.

## Free Site Hosting. Thanks Github!

<iframe width="640" height="480" src="https://www.youtube.com/embed/0h_GuoH449w?rel=0" frameborder="0" allowfullscreen></iframe>

### Setting Up A Username.Github.io Site

To get started open your browser and head over to Github.com and sign in. Start by creating a new repository by clicking the `+`  plus icon at top right and selecting **New Repository**. For the name let's name our repo specifially u`username.github.io`, where username is replaced with your actual username on Github. Min for example is jongrover.github.io. Then click the Create Repository button. Next copy the clone url as either SSH or HTTPS which ever you prefer. Then type `git clone <paste your clone url here>` pasting in your clone url using Command+v on mac or Ctrl+v on pc, then press return. Now we can cd into that repo: `cd <github-username>.github.io`. Create an index page by typing `touch index.html`. Open up the index page in your favorite code editor and type in,

```txt
Hello World
```

Save and exit, and head beack to Terminal. Next let's stage and commit our changes. Type `git add index.html` and press return. Then type `git commit -m "first commit` and press return. Then push up your changes `git push -u origin master` and press return. Now to test, open your browser and head to: `http://username.github.io.` where username is your Github username. If all went well your "Hello World" text should appear. If you don't see it right away be patient Github Pages sometimes has up to a ten minute delay before content appears.

### Using Gh-Pages Branch To Host A Repo

Another way you can host a site page on Github Pages is by creating a specially named branch. To get started first create a new repo on Github by clicking the `+` plus icon at top right and selecting **New Repository**. For the name feel free to call it anything you want. Then click the Create Repository button. Next copy the clone url as either SSH or HTTPS which ever you prefer. Then type `git clone <paste your clone url here>` pasting in your clone url using Command+v on mac or Ctrl+v on pc, then press return. Now we can cd into that repo: `cd <repository-name>`. Create an index page by typing `touch index.html`. Open up the index page in your favorite code editor and type in,

```txt
Hello World
```
Save and exit, and head beack to Terminal. Next let's stage and commit our changes. Type `git add index.html` and press return. Then type `git commit -m "first commit` and press return. Then push up your changes `git push -u origin master` and press return. 

Now let's create a new branch, type `git checkout -b gh-pages` and press return. It is important to name the branch exactly that in order for Github to serve the website page from this branch. Next, let's push up our new gh-pages branch, type `git push -u origin gh-pages` and press return.

Now to test, open your browser and head to this repository on Github.com. Next click on the gear icon to bring up the settings for this repo. Scroll down to the area that is labled Github Pages. If all went well there should be a link that says your site is being hosted at... Go ahead and click this link. Your "Hello World" text should appear at this location. If you don't see it right away be patient Github Pages sometimes has up to a ten minute delay before content appears.

### Limitations

Github will host static content in the form of HTML, CSS, and JavaScript as GIthub Pages Sites. If you use a special Ruby gem for Jeckyll you can also post a dynamic blog site. Github Pages will not host dynamic PHP, Python, Ruby or Node sites, so for the most part you are limited to a Front-End website only, with the exception of a Ruby based Jeckyll blog. For more details on what is acceptable to be hosted as a webpage check out the documentation from the link in the resources section below.

## Summary

- Github will host webpages for us for free using either username.github.io repository or by creating a gh-pages branch on any repo.

## Resources

- [Github Pages - Doc](https://pages.github.com/)
<p class='util--hide'>View <a href='https://learn.co/lessons/html-css-site-publishing-using-github-pages'>HTML CSS Site Publishing Using Github Pages</a> on Learn.co and start learning to code for free.</p>
