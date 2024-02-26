# **Lab Report Four**
---
## **Step 4** - Logging into ieng6

<img width="771" alt="Screenshot 2024-02-26 at 1 14 22 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/7bbf3b72-6045-43ce-91ab-997f482b0a55">

Keys pressed: `ssh mil118@ieng6.ucsd.edu` `<enter>`. 

Typing `ssh mil118@ieng6.ucsd.edu` is the command to log into my ieng6 account, and `<enter>` is the command used to execute this command.

---
## **Step 5** - Clone your fork of the repository from your Github account (using the SSH URL)

<img width="738" alt="Screenshot 2024-02-26 at 1 16 16 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/070f8747-77da-48bb-9f82-79974850ab39">

Keys pressed: git clone `<Command-V>` `<enter>`.

I had previously copied my `SSH` URL using `<Command-C>`, so I pasted it into the command line using `<Command-V>`. I then press `<enter>` to execute the command.

---
## **Step 6** - Run the tests, demonstrating that they fail

<img width="378" alt="Screenshot 2024-02-26 at 1 48 30 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/91fdf100-4c99-44c4-8b33-6ca99bfdff78">

Keys pressed: `cd` `l` `<tab>` `<enter>`.

I am using `cd` to change my directory to lab7, which contains all the code and test files. I then type `l` and `<tab>` because pressing `<tab>` autocompletes the command/path you are writing, and by writing `l`, it matches with the existing paths and autocompletes it based on the existing paths.


<img width="917" alt="Screenshot 2024-02-26 at 1 17 48 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/3f23bced-8258-451f-8db4-51e930afd553">

Keys pressed: `<Command-C>` `<Command-V>` `<enter>` , `<Command-C>` `<Command-V>` `<enter>`

I used `<Command-C>` to copy the `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command from the `test.sh` file in `lab7`. Then I used `<Command-V>` to paste the command I had just copied into the command line and I used `<enter>` to execute the command, which compiled the code. 


Then, I used `<Command-C>` to copy the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` command from the `test.sh` file in `lab7`. I used `<Command-V>` to paste the command I had just copied into the command line and I used `<enter>` to execute the command, which ran the tests for the code.

---
## **Step 7** - Edit the code file to fix the failing test

<img width="378" alt="Screenshot 2024-02-26 at 1 24 13 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/7dfbf956-76cb-4013-811a-e58f62fbc1f8">

Keys pressed: `vim` `ListExamples.java` `<enter>`.

The `vim` command, followed by the file name `ListExamples.java`, allows me to make changes to file using vim. I used `<enter>` to execute the command, which brought me to the vim text editor.

<img width="577" alt="Screenshot 2024-02-26 at 1 23 41 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/1e9ad26f-4b4f-4330-ad94-84286cddd902">

Keys pressed: `/x1` `n` `n` `n` `n` `n` `n` `n` `<right>` `r` `2` `:x`.

The `/x1` command searches for the first occurance of the characters `x1` in the entire file, then I press `n` to go to the next occurance of the same characters. When I get to the specific text that I need to change, I press the `<right>` key to hover over the `1` character. Now that I am hovering over the character, I press `r`, which stands for replace, and then I press the key `2` to replace the original character of `1` to the new character of `2`. Finally, I type `:x`, which is the command to save and exit the file.


## **Step 8** - Run the tests, demonstrating that they now succeed

<img width="917" alt="Screenshot 2024-02-26 at 1 24 47 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/bd5521db-fbe0-48d3-867a-caafc559e2bc">

Keys pressed: `<up>` `<up>` `<up>` `<up>` `<enter>` , `<up>` `<up>` `<up>` `<up>` `<enter>`

The `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java` command was 4 up in the search history, so I used the `<up>` arrow to access it. After getting it in the command line, I pressed `<enter>` to recompile the code.

Then, the `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore ListExamplesTests` was also 4 up in the search history, so I used the `<up>` arrow key to access it. After getting it in the command line, I pressed `<enter>` to run the tests. 


## **Step 9** - Commit and push the resulting change to your Github account
<img width="489" alt="Screenshot 2024-02-26 at 1 26 49 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/46fc5c46-194f-47a8-a06a-ed2b107229a3">

Keys pressed: `git add .` `<enter>` , `git commit -m "Fix failing test"` `<enter>` , `git push origin main` `<enter>`

First, I typed `git add .`, which adds all the files from my current directory to the index and prepares it to be committed. I press `<enter>` to execute this command. Now, I am enabled to type `git commit -m "Fix failing test"`, which allows me to commit all the changes I made to the files, and the message I enter is "Fix failing test", which is what I did with the changes that I made to the file. I press `<enter>`, which executes the command, thus committing the changes to the files. Next, I type `git push origin main`, which pushes the new changed files to the main branch of the original repository where it was originally cloned from. I then press `<enter>` to execute this command.
