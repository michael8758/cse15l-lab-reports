# Lab Report Two
## Part One
**Screen shot of ChatServer code**
<img width="1512" alt="Screenshot 2024-01-28 at 7 08 43 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/7a607ddf-a6b1-435e-b564-bab91f379df4">
<img width="1512" alt="Screenshot 2024-01-28 at 7 09 02 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/d3383969-a79d-4334-b762-6040e9b9af46">

**Which methods in your code are called?**
- First the main method in the ChatServer class is called, then the handleRequest method is called everytime I use `/add-message`.

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
- In the main method, the argument `String[] args` contains the port number for the server in which you are attemping to start.
- In the handleRequest method, the argument `URI url` is meant to contain the path and query for the server. A relevent field within this     method is the `String chatHistory` field, where it stores the chat history after using `/add-message`.

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**
- The `String chatHistory` field changes everytime `/add-message` is used because it stores the history of the chat within it, and everytime I am using `/add-message`, the new message I am adding becomes stored within this field.

**Screen shots of using `/add-message`**
<img width="1130" alt="Screenshot 2024-01-28 at 7 12 54 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/80433695-fc9b-4805-bbe0-c89c08c3c814">
<img width="1123" alt="Screenshot 2024-01-28 at 7 13 51 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/951c924a-5c50-4f9a-abe6-e0adaf8b275a">


## Part Two
**The absolute path to the private key for your SSH key shown using `ls`**
<img width="480" alt="Screenshot 2024-01-28 at 7 56 23 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/d9630994-a251-46c6-9272-b0a11f60a44c">

**The absolute path to the public key for your SSH key shown using `ls`**
<img width="524" alt="Screenshot 2024-01-28 at 7 57 46 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/fe50fd62-e5d9-4708-8994-f1180f4f076b">

**Terminal interaction where I log into `ieng6` account without being asked for a password**
<img width="1039" alt="Screenshot 2024-01-28 at 7 52 27 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/e977acfc-5303-406c-aa1d-737fb8daa830">


## Part Three
**What I learned in week 2 and 3**

- Throughout week 2 and week 3, a plethora of new concepts and ideas was introduced to me in which I had never had experience using before. For example, It was my first experience creating a web server and I was also introduced to the technical aspects of it such as the port that it runs on. I also learned that such methods are used for collaboration purposes, where multiple users can make edits or changes to the same documents or pages as long as they are on the same server. Furthermore, I also learned about commands such as `mkdir` and `scp`, which stand for 'make directory' and 'secure copy protocol' and their applications in making code writing more efficient.
