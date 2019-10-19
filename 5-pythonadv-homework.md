Hey everyone!! Thanks for the great class, I feel we have a good understanding of Python basics and can move forward to looking into datasets:muscle:
As always, don't forget to fill up the Weekly Journal: https://forms.gle/QAe9Dm54xNwUxZqZA !!!! :rocket::rocket::rocket:

Here's the homework for this week and have an excellent week:

*PREPARATION*
Create a new repository on GitHub called python-homework and clone it locally.
Use this repository to push all the scripts for this week's homework. Send me the link your repository after you are done!

*BASIC*
Write a script called `FizzBuzz.py` that loops over all the integers from 1 to 100.
- For multiples of three print "Fizz"
- For multiples of five print "Buzz"
- For multiples of three and five print "FizzBuzz"
- If the number isn't a multiple of neither three of five, print the number itself


*ADVANCED*
Write a script called `FileReader.py` that opens the boston housing dataset file (name is `housing.data`) and prints every line in the file. I'm sending the boston housing dataset in the next message in this channel.


*REACH*
1) Enhance the `FileReader.py` from the Advanced section: before you print each line, split them into list of values
(i.e. `0.00632  18.00   2.310  0  0.5380  6.5750  65.20  4.0900   1  296.0  15.30 396.90   4.98  24.00`
would become `['0.00632', '18.00', '2.310', '0', '0.5380', '6.5750', '65.20', '4.0900', '1', '296.0', '15.30', '396.90', '4.98', '24.00']`)

2) Write a script called `Desktop.py` that lists all files on your Desktop. For each file checked, print if the file is a file or a directory.
Tip: The path for Desktop should be similar to `C:/Users/<username>/Desktop` on Windows, `/Users/<username>/Desktop` on Mac and `/home/<username>/Desktop` on Ubuntu.
Tip: you can use os.path.isfile and os.path.isdir to help on this task!
Tip: Make sure you have some files and dirs in your Desktop otherwise the script will do nothing!




Don't forget to check at the reference codes we saw in the class to help you do the homework! (https://github.com/cce-bigdataintro-1160/CEBD-1160-fall-2019-code/tree/master/3-python-notebook):book:

And don't hesitate if you have questions! Next class we finally meets pandas!:panda_face:





### Homework
* Don't forget to fill up the Weekly Journal! 

##### Basic
1. Create a python script `dataset-processor.py` in the repo `class5-homework`. Your script should:
  * load the dataset
  * organize the data in a table-like format
  * compute and print summary statistics 
  * Visualize the data, 1-feature (column) at a time, i.e. line or histogram and save the figures to files 
  * Visualize the data, 2-features (columns) at a time i.e. scatter plot and save the figures to files
  * Optional: plot as many charts as you want! Why not to loop over all columns plotting multiple charts?
  * The dataset used should be the same dataset you chose for your final project!!!
2. Add a section at the end of your `README.md` explaining me how to run the file.

##### Advanced
1. Add code for adding header data to your table(dataframe) if necessary

##### Reach
1. Add an additional type of plot other than scatterplot (Google to find plot types of interest) for visualizing 2 or more of the features(columns) at a time. Please clearly express either in comments in the code or in your README.md what's the additional plot you chose.

* Recommendation: for all homework, plan to use `matplotlib` for plotting

* Extra challenge: make your `dataset-processor.py` capable of receiving a file name and a header file name as arguments to make it generic for any dataset, take a look at the class4-homework repository, adv_reach lesson for guidance.