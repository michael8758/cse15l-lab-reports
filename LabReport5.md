# **Lab Report 5**
---
## **Part 1 - Debugging Scenario**

**Student Post:**

<img width="500" alt="Screenshot 2024-03-07 at 7 14 39 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/e33a4221-5954-43ed-b700-1c08b2cec87e">

<img width="888" alt="Screenshot 2024-03-07 at 7 12 29 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/a5d55043-254d-49c4-a66c-274b7a9d6719">

<img width="784" alt="Screenshot 2024-03-07 at 7 15 17 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/de984967-d79a-46a4-a412-d4bd4eb52bcf">


Hi, I am having an issue with my code where my code is not able to compile and run properly, and it is also failing the test cases specifically for the prepend method, and something is very wrong with the prepend method but I cannot figure it out. The output when I try to compile the code returns saying I have 5 errors and a bunch of statements I do not understand. I have attatched screenshots of both the code I have written for the prepend method, and the output when I try to compile the file using the bas script.

**TA Response:**

Hi there! There are a lot of things going on with your code, but may I suggest you to start off by carefully reviewing line by line if there are any unusual looking code, perhaps something **missing** within specific lines. Try referring to the documentation for a for-loop.

**Student Response:**

<img width="584" alt="Screenshot 2024-03-07 at 7 31 42 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/ea77d7f4-db9a-4f73-aa56-bc93d68e577c">

<img width="1485" alt="Screenshot 2024-03-07 at 7 31 59 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/95e15b50-eb4e-4f4c-a5c0-a1fd67528608">

I have figured out what the error was after referring to the for-loop documentation and carefully checking line by line if anything looked unusual. I realized that I had not been incrementing and decrementing properly as the syntax for it is supposed to be `i++` and `i--`, not `i+` and `i-`. Furthermore, I realized that I had forgotten to add a closing bracket to the end of the method, which caused a syntax error. After making these changes, I was able to make my code compile and run successfully, and also pass all of the test cases. 


## **Part 2 - Reflection**

Throughout the second half of the quarter in CSE 15L, I was introduced to a lot of new concepts that I would be working with for the very first time. For example, 
