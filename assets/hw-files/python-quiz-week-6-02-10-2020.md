### Quiz (Monday, 2/10, Week 6 Lab)
We will start lab on Monday with a quiz which will test your ability to write the code necessary to:

- initialize a dictionary
- know the differences between the different data types and data structures (collections) that we've discussed in both lab and lecture
- perform operations with a dictionary
- count items in a list and dictionary
- write a for loop to perform operations and iterate through keys and values in a dictionary
 
PDFs from [lectures]({{ site.url }}lectures) have been posted. The _Introduction to Python_ book chapters 6, 7, 8 are useful for studying. Although your homework is to practice with the problems from chapter 8, if you'd like extra practice, go through chapters 6 and 7 as well.

#### Extra Credit
1. You can get extra credit towards this quiz by posting your questions about chapters 6, 7, and/or 8 to the course discussion forum on GitHub with **clear questions and examples of what you've tried** and/or **answer other student's questions** and **provide follow-ups to your posted questions**.
2. If you finish the other exercises, try and make progress on this bonus question.

 - Use `wget -c` to get the data file from `http://dev.shawntylerschwartz.com/docs/blake.csv`
 - In a Jupyter Notebook titled `fairness-extra-credit` in your `week-five` directory within `lab-exercises`, answer the following questions:
 - Blake et al. (Nature 2015) studied how the sense of fairness develops in different cultures. They conducted experiments to test whether and when children became adverse to disadvantageous inequity (peer receives more than self) and advantageous inequity (self receives more than a peer). Their data support the claim that disadvantageous inequity aversion emerged across all populations by middle childhood, while advantageous inequity aversion is more variable.
 - The csv file contains several columns:
    - `condition`: the treatment (`AI` or `DI`).
    - `eq.uneq`: was the distribution equal (`E`) or unequal (`U`)?
    - `decision`: did the actor `accept` or `reject`?
    - `country`: the country of the actor.
    - `actor.id`: identifier for the actor (each actor did several trials).
    - `actor.age.years`, `actor.gender`: age and gender of the actor.
    - `dist`, `trial`: each of 16 trial was associated with a distribution. For `AI`, actor-recipient were either 1-1 or 4-1; for `DI` either 1-1 or 1-4; each was repeated four times.
    - `value`: children were tested with `high` or `low` rewards (e.g., for Canada, Skittles vs. Goldfish crackers)
 
    1. Using python, read the file and extract the names of the countries involved in the experiment.
    2. How many `M`, `F` for each country?
    3. For each country, select actors of age 10-12. Are females more likely than males to reject when the distribution is unequal and to their advantage?