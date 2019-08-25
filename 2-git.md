# Intro 2 Linux & Version Control

### Agenda
* Homework Check
* Intro to Git
* Homework

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

### Additional Exercises Material
* [Extra exercises](./2-git-exercises.md): Additional exercises to practice Git

### Recommended References
* [Git CheatSheet](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet) All git commands in a single cheatsheet
* [Git UI Tools](https://git-scm.com/downloads/guis/): A list of UI tools for git
* [Git Documentation](https://git-scm.com/doc): The Official documentation for using git

### Advanced exercises material
* [Git Branching](https://learngitbranching.js.org/): Learn what git does visually with 
* [Official Pro Git Book](https://git-scm.com/book/en/v2): The Official Pro Git Book