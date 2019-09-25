# Intro 2 Linux & Version Control

### Objectives
* Learn what is a versioning system
* Why use git
* Create a repository and do your first commit
* Collaborate using git
* Understand what licensing is

### What is a versioning system and why git
* Version control systems are a category of software tools that help a software team manage changes to code over time
* A few famous examples are: git, subversion, mercurial, CVS, Perforce and Clear Case
* Some of the main features are:
  * Full history of all changes
  * Traceability of all changes with user and time
  * Ability to revert changes
  * Availability of Branches that allow team members to work concurrently on same code
  * Availability of Tags that allow for management of software releases
  * Availability of Code revision 
  * Automation of build chains

* How do you currently collaborate in your work? What's the versioning system used there?

### Why git
* [Git Reference](https://git-scm.com/docs): A reference to all git commands
* [Basic "Git Everyday" Walkthrough](https://git-scm.com/docs/giteveryday): A reference to basic git commands used on everyday coding

* Git is a *distributed* versioning system created by Linus Torvalds, the creator of Linux
* Small and lightweight
* Free and open source
* Has all the features mentioned above: [About Git](https://git-scm.com/about/)

### Creating a repository and doing your first commit
* We'll now learn how to deal with git locally
* In order to use git we'll need to initialize a repository, add files to it and commit them
* To understand what's happening, we'll use the `status` and `log` commands 
* Finally we'll see how the checkout command allows us to navigate across commits

1. Create a directory called `my-first-repo`. 
2. Navigate to it and initialize a git repository with `git init`. Check it with `git status` 
3. Create the files `cleaner.py`, `processor.py`, `submit.py`, `data.csv`, write a few lines in each. Check the `git status` 
4. Add one of those files to your staging area using `git add <filename>`. Check the `git status` 
5. Commit that file to git using `git commit -m "My commit message"`. Check the `git status`
6. Add a second of those files to your staging area. Commit that file to git with a different message. Check the `git status` 
7. Add the remaining files and commit with a different message. Check the `git status`
8. Use `git log` to visualize all we did
9. Use the command `git checkout <commit id>` on the previous commits. Check what happened to the files
10. Use the command `git checkout master` . Check what happened to the files

### Collaborate using git
* Git allows for collaboration through the use of remote repositories
* Remote repositories are accessible by multiple users that can synchronize to through the use of the pull and push commands
* Here are a some of the existing [Distributed Workflows](https://git-scm.com/book/en/v2/Distributed-Git-Distributed-Workflows) possible with git
* [GitHub](https://github.com/) is one of the most used git servers, allowing users not only to have shared repositories but to also collaborate using other tools like wikis, issue trackers and others
* We'll now learn how to synchronize our work with GitHub which will be our main point of collaboration for this course
 
1. Create a repository `class2-notebook` in GitHub and clone it.
2. In the cloned repository you must create, add and commit a file called `README.MD`.
2. Push your changes to GitHub in order to ensure the changes are stored in your `remote`
3. Use GitHub UI in your browser to modify the file and commit it.
4. Pull all the changes that happened remotely to your local git repository.
5. Add your class notes to this notebook, commit and push it again.

### Understand what licensing is
* [Licensing a Repository](https://help.github.com/en/articles/licensing-a-repository): A GitHub guide on how to license a repository
* [Choose a license](https://choosealicense.com/): A GitHub Page to help you decide which is the right license for your project

1. Create a LICENSE file in your previously created repository. Add the MIT license in it, commit and push.

### Final notes on Linux and Shell
* Let's review what we've learned today
* Other ways to use git

### Additional Exercises Material
* [Extra exercises](./2-git-exercises.md): Additional exercises to practice Git

### Recommended References
* [Git CheatSheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet) All git commands in a single cheatsheet
* [Git UI Tools](https://git-scm.com/downloads/guis/): A list of UI tools for git
* [Git Documentation](https://git-scm.com/doc): The Official documentation for using git

### Advanced exercises material
* [Git Branching](https://learngitbranching.js.org/): Learn what git does visually with 
* [Official Pro Git Book](https://git-scm.com/book/en/v2): The Official Pro Git Book