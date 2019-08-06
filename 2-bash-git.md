# Intro 2 Linux & Version Control

### Agenda
* Homework Check
* Intro to Shell
* Intro to Git
* Homework

### A brief introduction to Linux
* [The Linux Ancestry](https://en.wikipedia.org/wiki/Unix#/media/File:Unix_history-simple.svg): An image describing where Linux comes from
* [Linux list of distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions): A description of existing Linux distributions

### The Shell
* [The shell](./bash-git-files/shell.png): An image depicting the utility of the shell, interfacing inputs and outputs towards the kernel(core) of Linux
* [Bash, the Unix Shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)): A wikipedia page on the most popular Linux shell

##### Goals
Establish the foundation for our data analysis by understanding how the Linux shell works:
* [Gnu Core Utils](http://www.gnu.org/software/coreutils/manual/html_node/): A list of all shell commands
* [The man command - manual](http://www.linfo.org/man.html): The utility to read the manual for any shell command
* [Software Carpentry Unix](https://swcarpentry.github.io/shell-novice/): A Software Carpentry lesson for Shell

##### Be able to Navigate through the file system:
* [Filesystem Hierarchy Standard - Linux Standard Directories](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard): The basic file system organization in Linux

1. Find out what's your username. Find your home folder and list its contents.
2. Navigate to `/` and list the contents of this directory. Why is this a special directory?
3. Navigate to `/var/log` and list its files. What do we have here?
4. From the previous dir `/var/log` type `cd ../../Users/<myusername>`, why is the new current directory special?
5. Test the following commands: `cd .`, `cd ..`, `cd /` and  `cd ~`. Can you explain what each of those symbols mean?
6. From your home directory test both commands below and explain the difference:
    `cd Desktop`
    `cd /Desktop`
7. What command can give you the most recently modified file in your home directory?
8. Download the file titanic.zip from Slack and locate it through the Terminal by listing it

##### Work with Files and Directories

1. Create a directory called `learning-shell` in your home directory.
2. Download the file `random-datasets` from Slack. Copy it from your `~/Downloads` directory into your `learning-shell` directory and unzip it using `unzip random-datasets.zip`. Do not use the UI for these steps!
3. The files are highly unorganized! Lets organize this by first moving all files that start with `total-public-construction-spending` into the directory `total-public-construction-spending-data`. Second, move all the remaining files that have a `.json` extension into `country-data`. Third, move the `Iris.csv` file into `iris-species`.
4. This looks much better, but now rename the file `master.csv` to `suicides_dataset.csv`
5. Delete the duplicated `iris-species copy` directory.
6. Create three new directories: `csv`, `json` and `mixed`
7. Move `country-data` directory to `json` directory, move the `total-public-construction-spending-data` into the `mixed` directory and finally move all the remaining files and directories in `csv`
8. Let's backup our whole directory `learning-shell` by copying it to the `~/Desktop` directory, name it as `learning-shell-bkp`
9. Look at those files contents by printing some files in your directories using `cat` or `less`. Experiment with `absolute` and `relative` paths.
10. Create a file (using `vi` or `nano` editors) called `a_dataset.csv` in your home directory, write a few `csv` lines in it and save it.
11. Check all of your changes using the MacOS UI

##### Use External Tools and Gnu Core Tools to enhance your shell skills. Compose them using pipes and filters.

1. Unzip (using the terminal) our `titanic.zip` file to `titanic`, 
2. Provide the shape/dimensions of the file `train.csv`?
3. List the first 5 rows of the file. Now list the last 5.
4. Print this file in your screen using `cat` now use the `less` command.
5. Can you print only the names of all people in the file?
6. Print this file last 5 lines save the output to train_tail.csv
7. Print only the lines 3 to 5 of the file?
8. Can you explain the command `du -a . | sort -n -r | head -n 20` and why would you use it? 
9. Split the train.csv file in multiple files with 20 lines each. 

##### Write loops to iterate over lists

1. Download the `ultratrail-du-montblanc.zip` file from Slack and unzip it to `/Users/<myusername>/ultratrail`
2. Write a loop that prints the name, dimension and first 2 lines for each of the `.csv` files.
3. Write a loop that copies each of the `.csv` files with the prefix `bkp-` to a folder `/Users/<myusername>/ultratrail/backups`. 

##### Create scripts to automate basic processes

1. Write a script that suggests the data formats: csv, xlsx, pdf, doc and txt. It should allow the user to pick their desired extension then create a file named `selected.<extension selected>`. Use the `read` command to read the user input!
2. Write a script that keeps only the first N number of lines of all files in '/Users/<myusername>/files_to_clean/*.csv'. N should be an argument passed before starting the script! If other people depend on this being done daily, how can we automate it's daily execution at 8:00AM? 

##### Finding files and contents in files

1. Find the person called `Torborg` in the titanic file `train.csv`
2. Count how many people were male and female in the file
3. Count how many people called `John` are in the file and how many of them are male or female
4. Find all csv files in your home directory. Play with the `-maxdepth` flag to see the difference.
5. Print all the `grep` commands you did today.

### Intro to Git
* [About Git](https://git-scm.com/about/): Information on why to use git
* [Git Reference](https://git-scm.com/docs): A reference to all git commands
* [Basic "Git Everyday" Walkthrough](https://git-scm.com/docs/giteveryday): A reference to basic git commands used on everyday coding

##### Goals
Learn the basics of a versioning control system to enable work organization and collaboration

##### Understanding the necessity for a versioning system
How do you currently collaborate in your work? What's the versioning system used there?

##### Creating a repository and doing your first commit.
1. Create a directory called `my-first-repo`. Navigate to it and initialize a `git` repository. Check it's `git status`
2. Add the files `cleaner.py`, `processor.py`, `submit.py`, `data.csv`, write a few lines in each. Check the `git status` again.
3. Add one of those files to your staging area. Check the `git status`
4. Commit that file to git. Check the `git status`
5. Add a second of those files to your staging area. Commit that file to git. Check the `git status` 
6. See the history of your actions and see what are the changes in each commit
7. Use just one more commit for the remaining files. Check the `git status` 
8. Use `git log` to visualize what happened
9. Check the files using `ls`, then checkout your second commit, check what happened to the files now
10. Checkout your master branch, check what happened to the files

##### Undoing things
1. Undo a non-staged change in one of the files
2. Undo a staged change in one of the files
3. Undo a commited change in one of the files
4. Reset your master branch to an older commit (your changes will be lost, add a new fake commit if you don't want to lose it!)

##### Create a branch to split your development
1. Create a branch called `new-data` and add a commit to it with a new file called `data2.csv`.
2. Checkout your `master` and check the files that you see. 
3. Create another branch from `master` and check the files that you see. Add two commits to it in any files.
3. Checkout your master again and checking the files at each step, merge both branches into it.
4. Visualize with `git log --graph --oneline --decorate --all` what happened.

##### Collaborate using git
1. Create a repository `class2-notebook` in GitHub and clone it.
2. In the cloned repository you must create, add and commit a file called `README.MD`.
2. Push your changes to GitHub in order to ensure the changes are stored in your `remote`
3. Use GitHub UI in your browser to modify the file and commit it.
4. Pull all the changes that happened remotely to your local git repository.
5. Add your class notes to this notebook, commit and push it again.

##### Understand what licensing is
* [Licensing a Repository](https://help.github.com/en/articles/licensing-a-repository): A GitHub guide on how to license a repository
* [Choose a license](https://choosealicense.com/): A GitHub Page to help you decide which is the right license for your project

1. Create a LICENSE file in your previously created repository. Add the MIT license in it, commit and push.

### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Make sure you have your a `shell` (like `bash`) installed, and then choose a text editor you like to use at home! Any text editor should do. A few recommendations are: Visual Studio Code, Atom, Komodo! If you want to practice your Shell skills, you can stick to `vim` or `nano`, but beware the learning curve!
2. Install `python`, recommended steps can be found here: [Python Setup](http://swcarpentry.github.io/python-novice-inflammation/setup/). For Windows, I’d strongly recommend Option 3 (via Installing it through [Anaconda](https://www.anaconda.com/distribution/)) as it will make future steps much easier due to Windows lack of support for the Shell.
3. Complete the [Software Carpentry Unix](https://swcarpentry.github.io/shell-novice/) lesson
4. Send me what these command do: 
   `wc -l * | head -n 3 | sort -n`
5. Send me what does this script do:
   ```
   #!/bin/bash
   for dir in 0 1 2 S
   do
     mkdir $dir-files
     touch $dir-files/$dir
   done
   ```
   
##### Advanced
1. Complete Software Carpentry Git lesson as best as you can: [Git Novice](http://swcarpentry.github.io/git-novice/)
  
##### Reach
1. Be a `git` master! That is, do the following *from scratch*:
  * create a new repository on Github, with a license and a readme
  * clone it locally
  * create a new text file that contains at least 1 line of text
  * add your file to the repository
  * commit your changes
  * edit the README file that came in the repo in some way
  * commit your changes
  * push your changes to Github
  * send me the url for your Github repository

### Optional homework(no need to submit)
* What shell commands we learned are useful for data exploration and why?
* Do a quick research explaining what are the main pros and cons of the Python language.

### Recommended References
* [Shell Cheat Sheet](https://learncodethehardway.org/unix/bash_cheat_sheet.pdf): All shell commands in a single cheatsheet
* [Shell Interactive Manual](https://explainshell.com/): A web version of the man and the help of all shell commands

* [Git CheatSheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet) All git commands in a single cheatsheet
* [Git UI Tools](https://git-scm.com/downloads/guis/): A list of UI tools for git
* [Git Documentation](https://git-scm.com/doc): The Official documentation for using git

### Advanced exercises material
* [cmdchallenge](https://cmdchallenge.com/): Can you complete these challenges from 
* [Git Branching](https://learngitbranching.js.org/): Learn what git does visually with 
* [Oh My Zsh](https://ohmyz.sh/): Extension to use the shell like a boss
* [Official Pro Git Book](https://git-scm.com/book/en/v2): The Official Pro Git Book