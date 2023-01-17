Hello, everyone. Today we will learn how to log into a course-specific account on ieng6.

# Part 1 - Installing VScode
## Haven't installed
Go to the Visual Studio Code website([Link](https://code.visualstudio.com/)) and follow the 
instructions to install it on your computer. (`Notice`: There are three versions of downloading. 
One for macOS system. Another for Windows system. The other for Linux x64 system.)

After finishing installing, follow the steps in Already installed part.

## Already installed
Open the Visual Studio Code on your computer. After opening, you will see the following 
window on your screen.(It might be a slightly different because of different computer system.)
![Image](openVScode.jpg)

(Because I have already installed the Visual Studio Code on my computer, I can only do the Already installed part 
and show the picture of that part.)

# Part 2 - Remotely Connecting
Now, we will learn how to use VScode/terminal to remotely connect to a computer.

## For Windows system
(If your computer system is not Windows, skip this part and jump to Start connect part.)

Install [`git`](https://gitforwindows.org/) first. After finishing installing, follow the steps in 
[Using Bash on Windows in VScode](https://stackoverflow.com/questions/42606837/how-do-i-use-bash-on-windows-from-the-visual-studio-code-integrated-terminal/50527994#50527994) 
to set your default terminal to `git bash` in the Visual Studio Code.

## Start connect
1. Open a terminal in VScode.(Ctrl or Command + `, or use Terminal tab on the upper bar and choose New Terminal option.)
![Image](OpenTerminal.jpg)
2. Type in the following text in the terminal and press enter.
`$ ssh cs15lwi23ani@ieng6.ucsd.edu`
(`Notice`: You do not need to type in `$` because it already exists in the terminal. The letter after s is one. The letter after 5 is l, lowercase of L. Remember to replace ani by the letters in your course-specific account.)
![Image](Server.jpg)
3. If this is the first time you connect to this server, you will see the following message appear in the terminal. 
If this is not the first time you connect to this server, jump to step 5.
```
$ ssh cs15lwi23ani@ieng6.ucsd.edu
The authenticity of host 'ieng6.ucsd.edu (128.54.70.227)' can't be established.
RSA key fingerprint is SHA256:ksruYwhnYH+sySHnHAtLUHngrPEyZTDl/1x99wUQcec.
Are you sure you want to continue connecting (yes/no/[fingerprint])? 
```
(Because this is my second time to connect to this server, I do not have picture to show on.)
4. Type in `yes` and press enter.
5. The terminal will ask you to enter password. Type in your password.
(`Notice`: When you are typing your password, it is normal that you do not see anything appear or change in the terminal.)
![Image](Password.jpg)
`Notice`: If you forget your password, please follow the instructions 
[here](https://docs.google.com/document/d/1hs7CyQeh-MdUfM9uv99i8tqfneos6Y8bDU0uhn1wqho/edit) to reset your password.
6. After logging in successfully, you will see the following window on your screen.(The window on your screen might be slightly different than mine.)
![Image](SuccessLogin.jpg)
`Notice`: If the terminal keep ask you to enter your password, then the password you type in might be wrong.
![Image](WrongPassword.jpg)
7. Congratulation! You already remotely connect to a computer in the CSE basement. Any commands you run will also run on that computer.
(Your computer is called the client, the computer in the CSE basement is called the server.)

# Part 3 - Trying Some Commands
## Useful command list:
* cd: Change the current Working Directory to the path you enter
* cd ~: Change the current Working Directory to Home Directory
* cd ..: Change the current Working Directory to the directory "above" or "outside" the current directory
* ls: List all of the files and folders in the current Working Directory
* ls -lat
* ls -a
* pwd: Print the current Working Directory
* cat: Print the contents of the file given by the path you enter

## Example:
![Image](Try.jpg)
`Notice`: Please feel free to ask whenever you have question.
