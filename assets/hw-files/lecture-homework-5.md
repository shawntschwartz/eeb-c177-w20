# Lecture Homework #5 (Due Tuesday, 2/4 by 9:30am)
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