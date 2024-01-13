# **Lab Report one**

## `cd` Command Behaviour

**`cd` - no arguments**

<img width="779" alt="Screenshot 2024-01-10 at 1 03 32 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/415606e6-cd7f-4dbf-96ca-bb7e9c6c0e36">

- The working directory when the command was run was /home

- `cd` stands for "change directory", which allows you to change the current working directory to the given path, runnning the cd command with no argument will change the directory to the home directory, but since I am already in the home directory, running the cd command with no argument will not change my directory.

- The output of this command is not an error.


**`cd` - path to directory as an argument**

<img width="500" alt="Screenshot 2024-01-10 at 1 37 41 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/bc9cc760-5273-480d-b50e-14e992b01cf2">

- The working directory when the command was run was /home

- The command line shows "`cd` lecture1", in which I am changing the directory from the /home directory to the /home/lecture1 directory. After the command is run, the prompt updates to the directory that I am in - "lecture1" - which is highlighted in green.

- The output of this command is not an error.

**`cd` - path to a file as an argument**

<img width="547" alt="Screenshot 2024-01-11 at 9 23 27 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/e0b1a50e-b1ff-40aa-b3c8-d3bd8c6595e1">

- The working directory when the command was run was /home

- After running the command "`cd` /home/lecture1/messages/de.txt", the output stated that the argument I entered was not a directory, and therefore it resulted in an error. Since the change directory command is only meant to take in paths to directories as an argument, a path to a file as the argument will automatically result in an error.

- The output of this command is an error because the command `cd` can only take in arguments that are directory paths. Since I ran the command with a path to a file as the argument, the output of this command was an error.

## `ls` Command Behaviour

**`ls` - no arguments**

<img width="511" alt="Screenshot 2024-01-10 at 1 24 12 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/4d4f4c90-ac21-4664-ba0f-adebeef0e4f0">

- The working directory when the command was run was /home

- `ls` stands for "list", which lists the files and folders in the given path. Since I am currently in the home directory, the `ls` command lists "hello.txt" and "lecture1" because those are the file and folder located in the home directory.

- The output of this command is not an error.
  

**`ls` - path to directory as an argument**

<img width="402" alt="Screenshot 2024-01-11 at 9 27 24 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/3065a277-7c73-44c6-8498-07550019e244">

- The working directory when the command was run was /home

- After running `ls` with the argument "/home/lecture1", the output printed "Hello.class  Hello.java  messages  README", which represents a list of all the files and folders in the /home/lecture1 path.

- The output of this command is not an error.


**`ls` - path to a file as an argument**

<img width="427" alt="Screenshot 2024-01-11 at 9 52 22 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/d03ccfdc-5c6e-492a-8369-e23cad347cff">

- The working directory when the command was run was /home

- After running `ls` with the argument "/home/lecture1/README", the output printed "/home/lecture1/README", which is the exact same as the argument. This happens because since there are no more files or folders in the given path, the output just prints out the path to the file entered in the argument.

- The output of this command is not an error.


## `cat` Command Behaviour

**`cat` - no arguments**

<img width="355" alt="Screenshot 2024-01-10 at 1 25 46 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/01045c30-0d78-4298-a511-43b65c304890">

- The working directory when the command was run was /home

- When running the `cat` command without an argument, the `cat` command defaults to reading from the terminal since there are no files for it to read. Since there are no files for it to read, it first prints out nothing, since it read nothing. Further, if I were to type any argument in the terminal and execute it, it would return the same thing as I typed for my argument because it is reading from the terminal.

- The output of this command is not an error.

**`cat` - path to directory as an argument**

<img width="437" alt="Screenshot 2024-01-11 at 10 05 51 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/e21e8d04-8011-48b5-ad51-5dd9f4d09224">

- The working directory when the command was run was /home

- The argument of this command is a path to a directory, which resulted in an error in the output due to the invalid input. The `cat` command is only meant to take in files, not directories, as it is meant to take in files and print the contents within it, and it is unable to do so with directories.

- The output of this command is an error. The `cat` command is only meant to take in paths to a file, but the argument is a path to a directory, therefore it causes an erorr. The `cat` command is unable to read the contents of a directory, it is only able to read the contents of a file.

**`cat` - path to a file as an argument**

<img width="579" alt="Screenshot 2024-01-11 at 9 24 30 PM" src="https://github.com/michael8758/cse15l-lab-reports/assets/152559576/a7f7d4f4-320e-4713-858c-72bed2473d6b">

- The working directory when the command was run was /home

- When making the path to a file as the argument to the `cat` command, the output prints the contents in the file, which is exactly what is being displayed as occuring in the output. The path to the file given by "lecture1/messages/zh-cn.txt" allows the `cat` command to print out the contents inside the zh-cn.txt file, which is 你好世界.

- The output of this command is not an error.

