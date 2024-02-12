# Lab Report Two
## Part One
**Screen shot of ChatServer code**
<img width="1512" alt="Screenshot 2024-01-28 at 7 08 43 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/7a607ddf-a6b1-435e-b564-bab91f379df4">
<img width="1512" alt="Screenshot 2024-01-28 at 7 09 02 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/d3383969-a79d-4334-b762-6040e9b9af46">

**Which methods in your code are called?**
- First the main method in the ChatServer class is called, then the handleRequest method is called everytime I use `/add-message`.
- For the second screenshot, the handleRequest method is called everytime I use `/add-message`.

**What are the relevant arguments to those methods, and the values of any relevant fields of the class?**
- In the main method, the argument `String[] args` contains the port number for the server in which you are attemping to start.
- In the handleRequest method, the argument `URI url` is meant to contain the path and query for the server. A relevent field within this method is the `String chatHistory` field, where it stores the chat history after using `/add-message`. The value of this field currently in the first screenshot is `MacBook: Hello World`
- In the second screen shot, the main method argument `String[] args` contains the same port number for the server in which you are currently working in.
- The handleRequest method argument `URI url`, which contains the field `String chatHistory` becomes updated to contain both `MacBook: Hello World` and the new message `Samsung: My name is Apple`.

**How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.**
- The `String chatHistory` field changes everytime `/add-message` is used because it stores the history of the chat within it, and everytime I am using `/add-message`, the new message I am adding becomes stored within this field. In this specific example, I am adding `hello world` said by user `MacBook`, in which the url is `/add-message?s=Hello%20World&user=MacBook`. In doing so, the field changes to `MacBook: Hello World`.
- In the second screen shot, I am adding the message `Samsung: My name is Apple`, which is also being stored in the `String chatHistory` field. Now the updated field contains both the previous added message and the current message that I am adding - "MacBook: Hello World" and "Samsung: My Name Is Apple".

**Screen shots of using `/add-message`**
<img width="1130" alt="Screenshot 2024-01-28 at 7 12 54 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/80433695-fc9b-4805-bbe0-c89c08c3c814">
<img width="1123" alt="Screenshot 2024-01-28 at 7 13 51 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/951c924a-5c50-4f9a-abe6-e0adaf8b275a">


## Part Two
**The absolute path to the private key for your SSH key shown using `ls`**
<img width="337" alt="Screenshot 2024-02-11 at 8 31 56 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/3483b055-2bd5-409f-aca6-cbca9c54ca35">



**The absolute path to the public key for your SSH key shown using `ls`**
<img width="274" alt="Screenshot 2024-02-11 at 8 34 39 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/1f2d69d1-f7b3-41a2-a8fd-1f7206d1931f">


**Terminal interaction where I log into `ieng6` account without being asked for a password**
<img width="567" alt="Screenshot 2024-01-29 at 11 07 07 AM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/a0230c48-917f-4911-b70b-2e12f3692c52">



## Part Three
**What I learned in week 2 and 3**

- Throughout week 2 and week 3, a plethora of new concepts and ideas was introduced to me in which I had never had experience using before. For example, It was my first experience creating a web server and I was also introduced to the technical aspects of it such as the port that it runs on. I also learned that such methods are used for collaboration purposes, where multiple users can make edits or changes to the same documents or pages as long as they are on the same server. Furthermore, I also learned about commands such as `mkdir` and `scp`, which stand for 'make directory' and 'secure copy protocol' and their applications in making code writing more efficient.
