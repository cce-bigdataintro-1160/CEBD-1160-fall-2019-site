### Use External Tools and Gnu Core Tools to enhance your shell skills
1. Print only the lines 3 to 5 of the file?
2. Split the train.csv file in multiple files with 20 lines each.

##### Finding files and contents in files

1. Find the person called `Torborg` in the titanic file `train.csv`
2. Count how many people were male and female in the file
3. Count how many people called `John` are in the file and how many of them are male or female
4. Find all csv files in your home directory. Play with the `-maxdepth` flag to see the difference.
5. Print all the `grep` commands you did today.

##### Write loops to iterate over lists

1. Download the `ultratrail-du-montblanc.zip` file from Slack and unzip it to `/Users/<myusername>/ultratrail`
2. Write a loop that prints the name, dimension and first 2 lines for each of the `.csv` files.
3. Write a loop that copies each of the `.csv` files with the prefix `bkp-` to a folder `/Users/<myusername>/ultratrail/backups`. 

##### Create scripts to automate basic processes

1. Write a script that suggests the data formats: csv, xlsx, pdf, doc and txt. It should allow the user to pick their desired extension then create a file named `selected.<extension selected>`. Use the `read` command to read the user input!
2. Write a script that keeps only the first N number of lines of all files in '/Users/<myusername>/files_to_clean/*.csv'. N should be an argument passed before starting the script! If other people depend on this being done daily, how can we automate it's daily execution at 8:00AM? 
3. Answer what does this script do:
   ```
   #!/bin/bash
   for dir in 0 1 2 S
   do
     mkdir $dir-files
     touch $dir-files/$dir
   done
   ```

