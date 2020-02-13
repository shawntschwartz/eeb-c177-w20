# Lecture Homework #3 (Due Thursday, 1/23 by 11:59pm)
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