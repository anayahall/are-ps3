# ARE 212 Problem Set #3

#### MARCH 2018

## What is it
The THIRD problem set for ARE 212.

## How do I use it
Clone the repo from github.com and open in R-studio. This can be done via the command line or directly in R-studio with the url from github.com (big green button above). 

## Basic workflow for version control

In your local directory, **check for updates** in remote repository using:

	git fetch

If changes have been commited by others, then your local repo will be behind. 

To **update your local master** use:

	git pull

before beginning to work on the code. 

When you've finished working for the day and want to commit your changes use:

	git status

to see which files have been changed. Note: you can also use `git diff` to see exactly what has changed in those files.

Then **add** all those files: 

	git add .

or if you just want to add a specific file to be committed use

	git add <filename>

Then **commit** with a message explaining progress

	git commit -m "your message here"

Finally, **push your local commits** to the remote repository on github

	git push origin master

Here, *origin* is the default nickname for the remote repo on github.com, and *master* is the name of the main branch we're working on. More on branches below!

**Note:** *RStudio integrates beautifully with git, so pretty much all of the above can also be done in the RStudio GUI. Whenever you're working with a local directory that contains a .git file (meaning the directory has been initialized as a git repository), you will see a "Git" window in the "Environment/History" pane. You can do adding, commiting, pushing and pulling all from here. I tend to use the command line, which is why I focus on that workflow- I also think you get a better sense of what git is actually doing and how it interacts with github.com that way.*

### Branch stuff

Mostly we'll be working on the main branch, called 'master'. Sometimes though, we may want to experiment with some code and save that to a separate branch before commiting and merging that with the main 'master' code. 

To check which branch you're on use:

	git branch

To switch to a new branch use:

	git checkout -b newbranch

where 'newbranch' is the name of the new branch. 

**Note:** `git checkout -b` will create a new branch with the supplied name if none exists yet. You can also use `git checkout` to switch to an existing branch, like master. 


*more information on commiting changes in branches to come!*




