# Lecture Homework #4 (Due Sunday, 1/26 by 11:59pm)
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