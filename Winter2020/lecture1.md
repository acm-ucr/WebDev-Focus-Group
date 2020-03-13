http://codejeet.github.io/
http://ajeet.codes/

# How to get set up on Github Pages

## Prerequisite: have git and know how to use it

### For windows: 

The easiest way to get github up and running is with the [github GUI](https://desktop.github.com/). If you'd rather use the command line to learn, download standalone git [here](https://git-scm.com/download/win). If you'd like an emulated version of the linux Bash command line, download git bash [here](https://github.com/git-for-windows/git/releases/tag/v2.25.0.windows.1) 

### For linux/macos:

If you're on mac/linux, you probably already have git installed. If you don't, come to me for help.

## Step one: make a repository on Github

Log in, click the plus on the top right, and make a new repository. *You should name it the name of the domain that you're hosting it on, eg [your username].github.io*

## Step two: enable Github Pages

Go to the settings tab on your repository page, and enable github pages, choosing the master branch as your source.

## Step three (optional): link to your custom domain

On the same settings tab, scroll down to "Custom domain", and input the domain you purchased. Now, on your domain registrar (google domains, godaddy, etc) set a `CNAME` record pointing to `[your github username].github.io`

## Step four: fill your repo with content!


```
# Clone your repository to your local machine

git clone repository_name

# Should create a folder with the same title of your repository.
Move to this directory, and move your html file here.

cd repository_name

# If you want the page to be visible at the root, name it index.html 
# Now, we tell git to track this new html file

git add index.html

# Commit our new changes and push to remote branch

git commit -m "New githhub pages site"

git push

# Git will probably ask you for your usename and password at this point, enter it.
```
