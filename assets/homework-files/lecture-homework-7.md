# Final Project Assignment (8% of final project grade)
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