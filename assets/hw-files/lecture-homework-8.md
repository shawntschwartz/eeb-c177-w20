# Lecture Homework #8 (Due Sunday, 2/16 by 11:59am)

1a)  Change the program below so that it reports the temperature in Fahrenheit or Celsius depending on user input. (We did this in class so you can repost your code if you finished it.)
```python
xx = input("What is the temperature in Fahrenheit?")
yy = (float(xx) - 32) * 5 / 9
print("The temperature in Celsius is {}".format(yy))
```
1b) Modify your code above to robustly handle user input (as we discussed this idea in class). The `isdigit()` function will likely be helpful.

1c) Change your code above so that it is a function.

2a) Write a python block that will read the file Dalziel2016_data.csv, extract the cases from 1920, and write them to a new file.

2b) Write a python block that uses csv.DictReader (see example in Allesina and Wilmes, 3.7) to write the cases in Washington to a new file.

2c) Write code that prints the loc and pop for all the rows in the file Dalziel2016_data.csv.

2d) Write code that takes user input to specify a location and that writes the records correpsonding to that location to a new file. Write one or more functions in your code to handle the file reading and writing. Make this code robust to handle cases where no records exist for the specified input.

3a) Keep working with the file `Dalziel2016_data.csv` Write a program that extracts the names of all the cities in the database (one entry per city).

3b) Write a program that creates a dictionary where the keys are the cities and the values are the number of records (rows) for that city in the data.

3c) Write a program that calculates the mean population for each city, obtained by averaging the values of pop.

3d) Write a program that calculates the mean population for each city and year.

**4)** Singh et al. (2015) show that, when infected with a parasite, the four genetic lines of D. melanogaster respond by increasing the production of recombinant offspring (arguably, trying to produce new recombinants able to escape the par- asite). They show that the same outcome is not achieved by artificially wound- ing the flies. The data needed to replicate the main claim (figure 2 of the original article) is contained in the file Singh2015_data.csv in your data directory.
Open the file, and compute the mean RecombinantFraction for each Drosophila Line, and InfectionStatus (W for wounded and I for infected). Print the results in the following form:
```
Line 45 Average Recombination Rate:
W : 0.187
I : 0.191.
```