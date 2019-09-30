# Python Data Structures and Conditionals

### Agenda
* Intro 2 Python
* The Python Shell
* Writing a Python script
* Reading datasets with Python

### Intro to Python
* Python is a programming language created in 1991 with a design Philosophy emphasizing Code Readability
* Due to its simplicity, it's always been largely used for academic purposes, but it really took off around 2011 due to its compatibility with several popular platforms like PySpark and AWS Lambda. 
* A few characteristics from the Python language are:
  * Free and OpenSource: No vendor lock-in and no hidden service fees, making it safe for small and large companies adoption
  * Portable : Code written on Python can be executed without modification on Windows/Linux and MacOS systems (as long no native calls are made in the code)
  * Large ecosystem and community: Python has one of the oldest libraries ecosystems in the IT industry, rivaled only by other major languages. These extensions simplify a lot of daily work as most things can be just re-used.
  * Interpreted: Python doesn't require slow/complex code compilation, making its deployment easy and simple
  * Tools: There are several quality tools developed to assist Python development, like PyCharm and Jupyter

![infographic](./python-files/infochart2.jpg)   
   
* [Google Trends](https://trends.google.com/trends/explore?date=all&geo=US&q=%2Fm%2F02p97,%2Fm%2F07sbkfb,%2Fm%2F05z1_,%2Fm%2F0jgqg,%2Fm%2F0_lcrx4) comparing it to other popular languages

* Python code is written in files that we'll call scripts and use the `.py` extension
* Python scripts can be executed with a Python Interpreter, which is already installed in this classroom
* The Python Interpreter can be invoked in two ways:
  * We can use a tool called Python Shell by typing `python3` on the terminal. This will provide us with a special shell capable of running any python commands. No script is required for this mode, and it's an excellent tool for quick exercises and evaluations.
  * The other option is to invoke the command `python3 <my_script>.py`. Please notice that this invocation will require a script to have been created beforehand with the code you want to run. 

### The Python Shell
* Let's start the python shell in our terminals by typing `python3`

* Using the Python Shell, do the following exercise in pairs:
1. Check what's the type of the following values:
   * `type(1)`
   * `type(3.14)`
   * `type("Big Data!")` and `type('Big Data!')`
   * `type(True)` and `type(False)`
   * `type([1,2,"intruder",3])`
2. Use the command `help('Big Data!')`. What does the built-in help() method does?
3. Use the command `dir('Big Data!')`. What does the built-in dir() method does?
4. Write an equation that uses multiplication, subtraction and an addition that is equal to 42.5. 
5. Assign the result to the variable `result`. Ex: `result = <my equation formula>` 
6. Print your variable using `print(result)`
7. Given the string `'big data'` use slicing to produce the string `'g da'`


### Writing a Python script
* Let's now look how to write scripts and execute them
* A Python script can be written with any text editor, but we'll be using PyCharm, a powerful IDE to assist us
* Let's start by creating a project `class3-mynotebook` in GitHub and cloning it locally using `git clone <my repo url>` in the Terminal
* Let's open PyCharm and familiarize ourselves with the tool:
  * Create a new empty project pointing to the directory you just cloned from GitHub, this will make sure you'll be able to push your changes to GitHub later
  * Check the left side menu, top menu, terminal panel and version control panel
  * Create your first script that should produce the classic output: `Hello World!`
  * There are two ways to run your scripts: type `python3 <myscript>.py` from the Terminal Panel or right click on the script and click `Run`
  
* On a separate directory (outside `class3-mynotebook` please clone the course code project using `git clone https://github.com/cce-bigdataintro-1160/CEBD-1160-fall-2019-code.git`
* Open this project in PyCharm in a separate window and let's see a few script examples together

* Go back to your previous `class3-mynotebook` project and do the following exercise in pairs:
1. Write a script called `testing_scripts.py` with the following content below, run it using `python3 testing_scripts.py`:

```

mynumber=1
myfloat=3.14
mystring='Hello World!'
myboolean=True
mylist=[1,2,3,4,5]

print(mynumber)
print(myfloat)
print(mystring)
print(myboolean)
print(mylist)

print(f'{type(mynumber)}, {type(myfloat)}, {type(mystring)}, {type(myboolean)}, {type(mylist)}')
```

2. A script called `FizzBuzz.py` that prints the integers from 1 to 100. For multiples of three print "Fizz" instead , and for the multiples of five print "Buzz". For numbers which are multiples of both print "FizzBuzz"
3. Write another script called `hello_script.py`. It should take one number as input. If the number is equal to 42 print `Right answer to everything`. If the number is not 42 print `wrong answer`. If the input is not a number print `Sorry, invalid input, expecting number`.
4. Add, commit and push these three scripts to the `class3-notebook` repository in GitHub!

7. Return all elements between(non-inclusive) 4 and 8 on the list `[1,2,3,4,5,6,7,8,9]`
8. Can you replace `big data` with `BIG DATA` in the list `['a',2,['b',4,5,'big data']]`


* Use the python shell to write simple expressions and small processes
* Write scripts with input arguments, loops and flow control
* Provide file inputs to your scripts for data exploration


### Reading datasets with Python
1. Create a script called `my_csv_reader.py` that's able to read a file(you can use any file here) and that checks if it's a valid file. If it is print `I have a file to process`, otherwise print `Boo, no file for me.`
2. Expand this script to read a csv dataset and print it to the screen line by line. Replace the previous file with any of the toys datasets for this!
3. Expand this script by printing each line as a list of values. Example:
   The line:
   ```
   abc,cde,efg,1,2,3
   ```
   in the source dataset should become:
   ```
   ['abc','cde','efg','1','2','3']
   ```
4. Add, commit and push this script to the `class3-notebook` repository in GitHub!

### Final notes on Learning Python
* Let's review what we've learned today
* Today we learned two ways to execute Python code: the Python Shell and running scripts with the Python interpreter. In the future classes we'll also learn how to use two other tools: PyCharm and Jupyter, that are widely used in the industry.

### Additional Exercises Material
* [Extra exercises](./3-python-exercises.md): Additional exercises to practice each Python topic

### Optional homework(no need to submit, preparation for next class)
* Read the `Part 1: Orientation` and `Part 2: Containers` from [Docker Getting Started](https://docs.docker.com/get-started/)
* Research what is a Python external `library` and what can you do with it.
* Research what are the `numpy` and `argparse` python libraries and what are they used for.

### Recommended Readings
* [Python Basics Reference](https://pythonbasics.org/): Python basics simplified syntax for using Python basics
* [Official Python3 Documentation](https://docs.python.org/3/): Python3 documentation page
* [Python3 Reference](https://docs.python.org/3/library/index.html):  Python3 reference pages containing all base types
* [Python3 for beginners tutorials](https://wiki.python.org/moin/BeginnersGuide/NonProgrammers): Several Python references for studying, all recommended for beginners
* [Python Coding Style Guidelines](https://www.python.org/dev/peps/pep-0008/): Coding style guidelines for Python if you want to make your code look good
* [Python Docstring Conventions](https://www.python.org/dev/peps/pep-0257/): Rules for properly documenting your functions
* [Software Carpentry Python Lesson](http://swcarpentry.github.io/python-novice-inflammation/index.html): Software Carpentry Lesson on Python basics for data manipulation (Modules )

[Back To Main Page](./index.md)