---
layout: page
title: Homework
---

## Lab Exercises & Homework
### Quiz (Monday, 2/10, Week 6 Lab)
 - [Quiz Details]({{ site.url }}assets/homework-files/python-quiz-week-6-02-10-2020.pdf)
 - [Quiz Details]({{ site.url }}assets/homework-files/python-quiz-week-6-02-10-2020.md)

### Lab Homework (Week 5):
See [https://shawntylerschwartz.github.io/eeb-c177-w20/2020/02/03/lab-week-5/](https://shawntylerschwartz.github.io/eeb-c177-w20/2020/02/03/lab-week-5/)
 - Due on Github Sunday (2/9) by 11:59pm

### Lab Homework (Week 4):
See [https://shawntylerschwartz.github.io/eeb-c177-w20/2020/01/27/lab-week-4/](https://shawntylerschwartz.github.io/eeb-c177-w20/2020/01/27/lab-week-4/).
 - 2 Parts
  - Part 1: Due on GitHub Friday (1/31) by noon (12pm)
  - Part 2: Due on GitHub Saturday (2/1) by 11:59pm

### No Lab Homework Week 3!

### Lab Homework (Week 2):
See [https://shawntylerschwartz.github.io/eeb-c177-w20/2020/01/13/lab-week-2/](https://shawntylerschwartz.github.io/eeb-c177-w20/2020/01/13/lab-week-2/).
 - 2 Parts
  - Part 1: Due on GitHub Tuesday (1/14) by 9am
  - Part 2: Due on GitHub Sunday (1/19) by 11:59pm

### Lab Homework (Week 1):
- You will keep a food log/journal for the next 5 days (starting this afternoon) using this file
- You must make **10 commits** separated by **at least 6 hours** (i.e., 2 commits per day) M-F this week
- Each time you update the food log, make a add, commit, and push changes to GitHub
- Each commit is worth 10% of your grade for lab homework this week
- I will be checking each of your GitHub repository's commit logs to grade you (remember, they are all timestamped), so I should see a total of 10 commits over the next 5 days (two per day) starting today
- Update the `food-log.txt` file using the vim commands we practiced

<hr />

## Lecture Exercises & Homework
### Lecture Homework #7 (Due Friday, 2/14 by 12pm)
 - Final Project Assignment (8% of final project grade)
 1. Create a new repository on GitHub for your final project called `eeb-c177-project` and clone to your `~/Developer/repos/` directory.
 2. Create a directory within your `eeb-c177-project` repo called `analyses`.
 3. Create a Jupyter Notebook within `analyses` with the name `functions-analyses-week-6`.
 4. Goal: Write code to open up your data file and extract 2 or more columns of data, perform some operations on the extracted data, and then write the results to a new text file.
    - Part 1: You must write a function or multiple functions to do the **extraction**, **analyses**, and **visualization** of your data. Using Numpy or Pandas to accomplish the reading in of the data.
    - Please look at *Section 3.7* from the *Allesina & Wilmes (2019)* textbook for an overview of file input/output in Python.
    - Part 2: Show an alternative way of reading in the data. Take a look at the `csv.DictReader` function [https://docs.python.org/3/library/csv.html](https://docs.python.org/3/library/csv.html) from the `import csv` module. Use this to then examine and manipulate your data in the form of a dictionary. Count the number of occurances and look into other useful functions of the dictionary that can help you organize your data.
    - Chapter 12 in the *Introduction to Python* book is helpful for a perspective on mangaging data.
    - Chapter 14 in the *Introduction to Python* book is helpful for a perspective on file input and output.
    - Part 3: Read this page [https://pyformat.info/](https://pyformat.info/), this page [https://realpython.com/python-string-formatting/](https://realpython.com/python-string-formatting/), and Chapter 5 of the *Introduction to Python* book for information on the _New Style Formatting_ in Python. Using the `.format()` function in Python, create another output file that extracts and modifies the original data and save this data into a text file as output, making use of the `.format()` function to change how the data are output to the file. Make sure to show in your code what you did and why.
    - Use `markdown` headers within your Jupyter Notebook file to clearly separate parts 1, 2, and 3 of this assignment. Points will be taken off if directions are not followed.
    - Push to GitHub before the due date (Friday, 2/14 at 12 noon).
    
### Lecture Homework #6 (Due Sunday, 2/9 by 11:59pm)
1. Create a Jupyter Notebook in your `class-assignments` directory with the name `ch-8-exercises`.
2. Answer questions 8.1 to 8.14 from the Chapter 8 "Things to do" section of the _Introduction to Python_ book.
3. To get full credit for this assignment, you must make 3 commits on 3 separate days (Friday, Saturday, Sunday), where you try to answer at least 3 of the questions each time. _Spacing our your coding practice is an effective strategy to get better._
 - **These exercises will help prepare you for the in-lab quiz on Monday.**

### Lecture Homework #5 (Due Tuesday, 2/4 by 9:30am)
#### Part 1 (Revisiting the Shell)
 - There was a typo in the script we were trying to write in class to learn to pass arguments to a script from the Terminal.
 - When setting variables, there **should not** be a space between the variable name, the `=`, and the value that you want to assign.
 - Here is an updated example of the `dir.sh` script that should work properly on your machine.
 ```bash
#!/bin/bash
INPUTDIR=$1
ls -la $INPUTDIR
echo "Above are the directory listings for this folder"
pwd
echo "right now it is :"
date
 ```
 - Update your `dir.sh` script and push it to your `eeb-c177-scripts` repo on GitHub.
 - Then, let's make our `ExtractBodyM.sh` script dynamic to be able to accept any input file and output the body mass into a csv file with the user's desired filename.
 - The expected input into the terminal should look something like this:
 ```bash
 $ ExtractBodyM.sh inputdatafile.csv outputdatafile.csv
 ```
 **Note: ^these are just examples and placeholders above. The goal is to be able to replace them with anything that would match the format of the script that you wrote to extract the body mass.**

 - In order to test your script, I have prepared two new **input body mass files** that are in the same format as the `Pacifici2013_data.csv` dataset file. You should also test it with the original `Pacifici2013_data.csv` dataset file.
 - You can get these files by using the `wget` command as we've done before.
1. `wget -c http://dev.shawntylerschwartz.com/docs/PanTHERIA_dataset.csv`
2. `wget -c http://dev.shawntylerschwartz.com/docs/other_sources_dataset.csv`

**Push your updated `ExtractedBodyM.sh` script (that can accept two arguments; 1: the input filename, and 2: the output filename) to your `eeb-c177-scripts` repo on GitHub.**

#### Part 2 (Python Practice)
 - Read `Chapter 1` of the _Introducing Python_ Book (Lubanovic, B. (2019). Introducing Python, 2nd Edition: Modern Computing in Simple Packages. O’Reilly Media.)
 - ^ This book is available on the UCLA Network or with the UCLA VPN at [https://proquest.safaribooksonline.com/book/programming/python/9781492051374](https://proquest.safaribooksonline.com/book/programming/python/9781492051374).
 - In your `class-assignments` directory, make a directory called `python-notes`.
 - Inside of `python-notes`, create a Jupyter Notebook that shows that you have worked through the examples inside of `Chapter 2` and `Chapter 3` of the _Introducing Python_ Book. **Create a separate Jupyter Notebook for each chapter, and name them `chapter2` and `chapter3`.**
 - At the end of each chapter, there is a *Things to Do* section. Do the problems there as well within your notebook and make sure to label to sections and headers within your notebook approporiately.

#### Part 3 (Preview to Dictionaries in Python)
Do problems 1-10 on this website [https://www.w3resource.com/python-exercises/dictionary/](https://www.w3resource.com/python-exercises/dictionary/). The solutions are listed, but you won't fully grasp the concepts if you don't work through the problems yourself. As such, please write a comment **directly after** each line of code to explain what is happening. We will be going over this concept in lecture tomorrow, and it's important that you practice it beforehand.

Call it `lecture-hw-5-part3` in your `class-assignments` directory.

### Lecture Homework #4 (Due Sunday, 1/26 by 11:59pm)
#### Part 1 (Making a New Git Repository)
When we made our first Git Repo, `eeb-c177-homework`, we made it on GitHub and then cloned it to our machines. The other way to make a GitHub Repo is to **initialize** a git repo in a directory on your computer and then connect it to a **remote** location (i.e., GitHub). We will therefore make a git repo to store our scripts.
1. In your `repos` directory, make a directory called `eeb-c177-scripts`.
2. `cd` into `eeb-c177-scripts` and type `git init` **IN YOUR SCRIPTS DIRECTORY**.
3. `mv` your `dir.sh` script from class into `eeb-c177-scripts`
4. Do `git add -A`
5. Then commit your script with `git commit -m "added dir.sh script"`
6. Go on **GitHub** and make a new repo using the plus icon with the name `eeb-c177-scripts`
7. **PLEASE READ THIS STEP CAREFULLY: REPLACE _yourusername_ with your own GitHub username.** In terminal, type `git remote add origin https://github.com/yourusername/eeb-c177-scripts.git`
8. Do `git push -u origin master`

#### Part 2 (Making a New Script)
Let's make a shell script of the body mass extraction exercise we did previously.
1. Inside of your `eeb-c177-scripts` git repo directory, `touch ExtractBodyM.sh`
2. Use nano to open and edit your script: `nano ExtractBodyM.sh &` (the "&" character opens the script in the background so you can keep using the terminal)
3. Now, add your terminal command pipeline to the script (the same one you used to create the `BodyM.csv` file).
4. You can use the `#` symbol to write comments in your code file that the computer will pass over when running the script. This is helpful so that you know the purpose of the code when you return to it in the future. **Please comment your script using `#` to explain what each aspect of your code accomplishes.** (See an example comment below.)
5. You can run the script using the `bash` command. `bash ExtractBodyM.sh`
6. With what we learned in class, how could you make this script run automatically from any prompt **without typing bash**? **(Write your answer in the script file as a comment (i.e., following the `#` symbol).)** You will need to change permissions to execute the script. To do this, you need to give the file execute permissions using the following command: `chmod +x ExtractBodyM.sh`
7. Push this script to your new git repo on GitHub. I will be grading it from there.

**Example of comments in a script:**
```bash
# Skip first line of file
```

### Lecture Homework #3 (Due Thursday, 1/23 by 11:59pm)
#### Part 1:
1. Create a directory under your `class-assignments` directory with the name `week-three-hw` and `cd` into it.
2. Download this csv data file using `wget -c` from this address: `http://dev.shawntylerschwartz.com/docs/nobel.csv`.
3. Look at the first few lines to familiarize yourself with these data. 
4. In a **Markdown (.md)** file with this name: `part-1-nobel.md`, place your command followed by the output (answers) to each of the following questions:
    1. Find the number of winners for each Nobel prize (`chemistry`, `economics`, `literature`, `medicine`, `peace`, `physics`).
    2. Find the winners of multiple Nobel prizes.
    3. Find the most common surnames among the winners.
    4. The Nobel prizes have not been awarded every year since 1901. Which one has been awarded the most? Which the least?

#### Part 2:
1. Download this csv data file using `wget -c` from this address: `http://dev.shawntylerschwartz.com/docs/European_Red_List.csv`.
2. Look at the first few lines to familiarize yourself with these data.
```
Species codes:
EX Extinct
RE Regionally Extinct
CR Critically Endangered (= threatened species)
EN Endangered (= threatened species)
VU Vulnerable (= threatened species)
NT Near Threatened
LC Least Concern
DD Data Deficient
NA Not Applicable
```
3. In a **Markdown (.md)** file with this name: `part-2-redlist.md`, place your command followed by the output (answers) to each of the following questions:
    1. Count the number of occurrences for each category (`EX`, `RE`, etc.).
    2. Repeat the previous step, but only consider birds (class `AVES`).
    3. For each order of birds, compute the number of extinct/near extinct (`EX`, `RE` or `CE`) species.

### Lecture Homework #2 (Due Tuesday, 1/21 before lecture by 9:30am)
#### Notes about this assignment:
 - To get full credit for this assignment, you will need to have at least 3 commits spanning 3 different days showing your progress working on this assignment. 
 - You are encouraged to have a separate text file as a log to explain what you are doing and any problems that you may have encountered throughout solving each problem. (Remember, you can use the `history` command as well as use a nicely formatted markdown file (`.md`) to show the commands you are entering and the results that you get. **Feel free to use markdown (.md) for files instead of .txt where appropriate.**
 - You must attempt and try all of these problems for this assignment. If you get stuck, work with others and consult the course discussion forum.
 - Everything that we are doing for this assignment is discussed throughout the first chapter of the textbook, so if you are getting stuck, work through the examples in the first chapter of the book. 
 - If you commit each day (Friday, Saturday, Sunday, Monday) up until Tuesday, you will also get some extra credit for this assignment. 
 - For the optional, extra credit assignments (1.10.3 and 1.10.4), you can only get extra credit if you successfully complete all of the other parts of the assignment (parts 1-5). Do not attempt these assignments until you have finished the other parts (if time permits).
 
#### Part 1:
1. Download this text file using the `wget` command into your `sandbox` directory (within `~/Developers/repos/CSB/unix/sandbox/`): `wget -c http://dev.shawntylerschwartz.com/docs/paragraphs.txt`.
2. Make a new folder in your `class-assignments` directory with the name `homework-two` and move this `paragraphs.txt` file into that location. **Then, do the git add-commit-push workflow again.**
3. Traverse to your `class-assignments/homework-two/` directory and rename the file `easy-question.txt`. **Then, do the git add-commit-push workflow again.**
4. Create a text file titled `hw2-part1-commands.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

#### Part 2
1. Use the `head` command to examine the **first 25 lines** of the `Pacifici2013_data.csv` file in `~/Developers/repos/CSB/unix/data/`. 
2. Now create a new text file with only the **first 25 lines** of that file with the name `Pacifici-25lines.txt` in your `class-assignments/homework-two/` directory.
3. Now create another text file that contains the number of words in the **first 25 lines** of the file with the name `Pacifici-25wordcount.txt` in your `class-assignments/homework-two/` directory.
4. Create a text file titled `hw2-part2-commands-1.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

In *section 1.6.1 of the textbook*, the **pipe |** is introduced. The pipe command allows you to take the output from one command and subsequently use it in the next command. Given this command, find the number of words in the **first 25 lines** as you did above **using the pipe command to avoid making an intermediate text file**.
5. Create a text file titled `hw2-part2-commands-2.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

#### Part 3
Let's use the **pipe** again to count the number of lines in the `~/Developers/repos/CSB/unix/data/` directory (i.e., count the number of lines that are listed when you list the contents of the data directory). 

1. Output the number of lines (in one line of code, using pipe) to a text file named `pipe-data-lines.txt`.
2. Using `cat` and `|` in one line of code, concatentate any 2 *.fasta* files from the `~/Developers/repos/CSB/unix/data/miRNA/` directory and count the **total number of characters** using the word count (`wc`) command. Output this to a text file named `fasta-cat.txt`. **Then, do the git add-commit-push workflow again.**

The `cut` command allows one to extract data columns that are formatted in a `.csv` format (*csv* stands for "comma separated values", although the delimiting (separating) character between values of the file (a.k.a., *the delimiter*) does not necessarily need to be a comma).
3. Examine the `Pacifici2013_data.csv` file using the head command and identify the delimiter. (Write this down in a text file named `Pacifici-delim.txt`.) **Then, do the git add-commit-push workflow again.**
4. Now use the `cut` command on this `Pacifici2013_data.csv` file to extract the family of the **first 10 records** *(hint: you will need to use pipe and the `head` command and also specify the delimiter using `-d` with the `cut` command)*.

Similar to the `head` command, the `tail` command allows you to look at the end of a file.
5. Look at the **last 5 records** in the `Pacifici2013_data.csv` file using the `tail` command.

The `tail` command can be used to skip the first few lines of a file with the `+` command (it will therefore start the `tail` command from whatever line you give after the plus).
6. Remove the **first line** of the `Pacifici2013_data.csv` file *(as we don't want the header of the file)*. 
7. Now, create a new text file with the name `Pacifici-ten.txt` that has the **first 10 records** of the `Pacifici2013_data.csv` file *(minus the header)*. (Note: you will need to use both `tail` and `head` to accomplish this.)
8. Create a text file titled `hw2-part3-commands.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

#### Part 4
The unique (`uniq`) command allows you to see the unique values when duplicates are present.
1. Use the `wget` command to download a text file containing fish species names from a recent study Shawn conducted into your `homework-two` directory: `wget -c http://dev.shawntylerschwartz.com/docs/fish_species.txt` **Then, do the git add-commit-push workflow.**.
2. Explore the sort, reverse sort, and unique commands with this text file. Copy and paste your results into three separate text files for the results of each of these three commands:
 - `fishes-sort.txt`
 - `fishes-rev-sort.txt`
 - `fishes-unique.txt`
3. Create a text file titled `hw2-part4-commands.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

**Work through exercises 1.6.2 and 1.6.3 from the textbook that will help you with some of the tasks above.**

#### Part 5
We are giong to create a data set that has the body size, order, family, genus, and scientific name that we are going to extract from the `Pacifici2013_data.csv` file. Things to keep in mind about the new data set that you are generating:
1. We don't want the header from the original `Pacifici2013_data.csv` file, so you will need to use the `tail` option to avoid extracting the first line.
2. We don't want all of the data, just columns 2-6, so use the `cut` option with the properly specified delimiter and column range values.
3. We don't want semicolons separating the data (as semicolons are a non-standard delimiter). Instead, use the `tr` command to subsitite **spaces** as the *new delimiter* instead of **semicolons**.
4. To sort the file, we will want to sort on a numeric column (which is the body mass column, column 6), so we will have to use `-r` to get it in the reverse order, `-n` to sort numerically, and `-k` to specify the column.
5. Create a new file `bodym.csv` that contains all of the specifications from above.
6. Create a text file titled `hw2-part5-commands.txt` containing the commands you used to accomplish this task. This file should be inside the `homework-two` directory. **Then, do the git add-commit-push workflow again.**

#### EXTRA CREDIT
Complete exercises **1.10.1** and **1.10.2** from the textbook. Try to get as far as you can.
1. Post your solutions in a text file titled `hw2-ec.txt`.

### Lecture Homework #1 (Week 2, Due Thursday, 1/16 before lecture by 9:30am)
Work through this Software Carpentry Tutorial [http://swcarpentry.github.io/shell-novice/03-create/index.html](http://swcarpentry.github.io/shell-novice/03-create/index.html). You will need to download the `data-shell.zip` file and extract the contents to the folder that you will be doing this assignment in, which should be in `~/Developer/repos/eeb-c177-homework/class-assignments/` from the top of this page (http://swcarpentry.github.io/shell-novice/setup.html)[http://swcarpentry.github.io/shell-novice/setup.html]. (Once you download it, you can drag it into the folder in your GitHub repo for this assignment, or you can use the commands we learned in class to do it via the shell, i.e., `mv ~/Downloads/data-shell.zip ~/Developers/repos/eeb-c177-homework/class-assignments/` or however you have your file structure laid out. Turn in a file containing the commands you used to complete these tasks, along with another file of any explanations of what you did (if necessary). **Make sure to push this to GitHub before class on Thursday (1/16).
