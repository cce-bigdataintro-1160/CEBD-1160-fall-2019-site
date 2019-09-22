# Intro 2 Linux & Version Control

### Agenda
* Homework Check
* A brief introduction to OS and Linux
* The Shell
* Be able to Navigate through the file system
* Work with Files and Directories
* Use External Tools and Gnu Core Tools to enhance your shell skills
* Homework

### A brief introduction to OS and Linux
* [Operating Systems](https://en.wikipedia.org/wiki/Operating_system)
* An operating system provides facilities to interface between applications and hardware using low level libraries and drivers.
* The most important resources it will manage are:
  * Inputs: Mouse, Keyboard, Sensors, Network
  * Outputs: UI, Disk, Network 
  * Processing (or In-Memory) state: Applications, scripts, programs
  * Storage (or Persistent) state: File systems/Disk
  
* Big Data Software will try to leverage these resources to work in a coordinated and distributed way. 
* [Awesome Big Data](https://github.com/onurakpolat/awesome-bigdata): An exhaustive list of Big Data open software. Most of it was built for Linux distributions.
* [The Linux Ancestry](https://en.wikipedia.org/wiki/Unix#/media/File:Unix_history-simple.svg): An image describing where Linux comes from
* [Linux list of distributions](https://en.wikipedia.org/wiki/List_of_Linux_distributions): A description of existing Linux distributions

### The Shell
* Bash is a command processor that typically runs in a text window where the user types commands that cause actions.

* [The shell](./bash-git-files/shell.png): An image depicting the utility of the shell, interfacing inputs and outputs towards the kernel(core) of Linux
* [Bash, the Unix Shell](https://en.wikipedia.org/wiki/Bash_(Unix_shell)): A wikipedia page on the most popular Linux shell

### Be able to Navigate through the file system:
* [Filesystem Hierarchy Standard - Linux Standard Directories](https://en.wikipedia.org/wiki/Filesystem_Hierarchy_Standard): The basic file system organization in Linux
* [Navigation shell commands](https://github.com/cce-bigdataintro-1160/CEBD-1160-fall-2019-code/blob/master/class2-notebook/1-navigation_shell_commands.sh)
* [The man command - manual](http://www.linfo.org/man.html): A utilitary tool to read the manual for any shell command

1. Find out what's your username. Find your home directory and list its contents.
2. Navigate to `/` and list the contents of this directory. Why is this a special directory?
3. Navigate to `/var/log` and list its files. What do we have here?
4. From the previous dir `/var/log` type `cd ../../Users/<myusername>`, why is the new current directory special?
5. Test the following commands: `cd .`, `cd ..`, `cd /` and  `cd ~`. Can you explain what each of those symbols mean?
6. From your home directory test both commands and explain the difference: `cd Desktop` and `cd /Desktop`
7. What command can give you the most recently modified file in your home directory? Hint, use ls --help to find the right tool to use.
8. Download the file titanic.zip from Slack using the UI and locate it through the Terminal by navigating and listing it

### Work with Files and Directories
* [Working with files](https://github.com/cce-bigdataintro-1160/CEBD-1160-fall-2019-code/blob/master/class2-notebook/2-files_dirs_shell_commands.sh)

1. Create a directory called `learning-shell` in your home directory.
2. Download the file `random-datasets` from Slack. 
   * Copy it from your `~/Downloads` directory into your `learning-shell` directory 
   * unzip it using `unzip random-datasets.zip` 
   * Do not use the UI for these steps!

3. The files inside it are highly unorganized! 
   * Lets organize this by first moving all files that start with `total-public-construction-spending` into the directory `total-public-construction-spending-data` 
   * Second, move all the remaining files that have a `.json` extension into `country-data` 
   * Third, move the `Iris.csv` file into `iris-species`

4. This looks much better, but now rename the file `master.csv` to `suicides_dataset.csv`
5. Delete the duplicated `iris-species copy` directory.
6. Create three new directories: `csv`, `json` and `mixed`
7. Move `country-data` directory to `json` directory
8. Move the `total-public-construction-spending-data` into the `mixed` directory and finally move all the remaining files and directories in `csv`
9. Let's backup our whole directory `learning-shell` by copying it to the `~/Desktop` directory, name it as `learning-shell-bkp`
10. Look at those files contents by printing some files in your directories using `cat` or `less`. Experiment with `absolute` and `relative` paths.
11. Create a file (using `vi` or `nano` editors) called `a_dataset.csv` in your home directory, write a few `csv` lines in it and save it.
12. Check all of your changes using the UI

### Use External Tools and Gnu Core Tools to enhance your shell skills. Compose them using pipes and filters
* [A few Gnu Core Tools](https://github.com/cce-bigdataintro-1160/CEBD-1160-fall-2019-code/blob/master/class2-notebook/3-advanced_shell_commands.sh)
* [Gnu Core Utils](http://www.gnu.org/software/coreutils/manual/html_node/): A list of all standard shell commands present on any Unix distribution

1. Unzip (using the terminal) our `titanic.zip` file to `titanic`, 
2. Provide the shape/dimensions of the file `train.csv`?
3. List the first 5 rows of the file. Now list the last 5.
4. Print this file in your screen using `cat` now use the `less` command.
5. Can you print only the names of all people in the file?
6. Print this file last 5 lines save the output to train_tail.csv
7. Print only the lines 3 to 5 of the file?
8. Can you explain the command `du -a . | sort -n -r | head -n 20` and why would you use it? 
9. Split the train.csv file in multiple files with 20 lines each. 

### Additional Exercises Material
* [Extra exercises](./2-bash-exercises.md): Additional exercises to practice Shell

### Recommended References
* [Shell Cheat Sheet](https://learncodethehardway.org/unix/bash_cheat_sheet.pdf): All shell commands in a single cheatsheet
* [Shell Interactive Manual](https://explainshell.com/): A web version of the man and the help of all shell commands
* [Software Carpentry Unix](https://swcarpentry.github.io/shell-novice/): A full lesson teaching how to use the shell from A to Z. We'll be doing this as part of the homework for this week.

### Advanced exercises material
* [cmdchallenge](https://cmdchallenge.com/): Can you complete these challenges from 
* [Oh My Zsh](https://ohmyz.sh/): Extension to use the shell like a boss
