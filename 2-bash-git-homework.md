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