**Lab Report 2 - Servers & Bugs**

*Part 1 - String Server*

Using the code based off of Number Server from week 2, I created a simple alternate version that stores a string from input in the url and adds on to it. There's some code to show how it functions, as well as two screenshots of add-message implementation at work.

![Image of StringServer Code](Screenshot 2023-04-24 230322.png)

*Part 2 - Remotely Connecting*

You will want to access your specific course account at [this website](https://sdacs.ucsd.edu/~icc/index.php) and reset your password (Note: This means you should reset the password for the course specific account, not your general UCSD email/account). You will also need to install [Git if you're on Windows](https://gitforwindows.org/).
After copying your username, password, and installing Git if needed, head over to VSCode and create a new terminal with the toolbar at the top. Select the downward arrow on the righthand side and select Git Bash to change the terminal.

![Git Bash & Terminal](https://raw.githubusercontent.com/Yves-M22/cse15l-lab-reports/main/images/Screenshot%202023-04-08%20185625.png)

    Once you've made it this far, type in ssh @ieng6.ucsd.edu, with your course specific username coming before the @ sign. Type yes when it asks you to continue to connecting. It only asks this if you've never tried before, but if this is your first time doing this and this does not pop up and ask for a password, your username was incorrect. Afterwards, put in your password into the terminal (Note: You will not be able to see what you're typing for security reasons). This is the screen you should see if you have successfully connected. 

![Successful connection](https://raw.githubusercontent.com/Yves-M22/cse15l-lab-reports/main/images/Screenshot%202023-04-05%20154830.png)

*Part 3 - Running Commands*

There are some commands that can be run once you connect to the remote computer. The image below uses two specific commands

* ls -lat
* ls -a

Both of which utilize the list command to list out the files and folders of the given path. In this case they show all the files in the specific path of the remote computer, as seen in the terminal of the image below. But there are other specific commands you can also try to test.

* cd ~
* cd
* cp /home/linux/ieng6/cs15lsp23/public/hello.txt ~/
* cat /home/linux/ieng6/cs15lsp23/public/hello.txt

The following commands have different actions. The first two change the directory to a given path, but since the first has a ~ symbol and the second is blank, they should change the directory to the home directory. The cp command creates a copy of a specified file, the one above can be used on the remote computer to copy hello.txt. Cat prints the contents of one or more given files, so the command above would print out whatever is written inside hello.txt.


![Example of some commands](https://raw.githubusercontent.com/Yves-M22/cse15l-lab-reports/main/images/Screenshot%202023-04-05%20160826.png)
