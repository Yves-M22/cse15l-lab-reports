**Lab Report 2 - Servers & Bugs**

*Part 1 - String Server*

Using the code based off of Number Server from week 2, I created a simple alternate version that stores a string from input in the url and adds on to it. There's some code to show how it functions, as well as two screenshots of add-message implementation at work.

![Image of StringServer Code](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230322.png?raw=true) 



![Image of AddMessage-1](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230424.png?raw=true)   

For this example of how add message is used, in the specific moment shown, handle request is called and skips the first if statement since there's more characters beyond the '/'. It goes through the method to add the inputted string since add-message comes after the '/', where the string is then returned and seen on the site. The method takes in any argument that is of type URI, and the following if statements check specific strings to determine what should be done. The value for the URI field would be a url, while the input for the if statements check strings. There's also a string named input for the method. Whenever /add-message is used, the value of String input is being changed by adding a new portion of a string and a new line chracter. In the image, "I love ECE 35" and a new line character is stored.   



![Image of AddMessage-2](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230457.png?raw=true)

This example is similar to the last one with the only difference being the addition of another string into input. The same method is called as in the first example, and will go through the same lines of code to add this new string into the input. When /add-message is used, the value of String input is changed by adding "So much :D" to input, which sould already contain something from previously using /add-message. After this is called, input now contains "I love ECE 35" and "So much :D" with a new line character between them and after the second added message.

*Part 2 - Remotely Connecting*

You will want to access your specific course account at [this website](https://sdacs.ucsd.edu/~icc/index.php) and reset your password (Note: This means you should reset the password for the course specific account, not your general UCSD email/account). You will also need to install [Git if you're on Windows](https://gitforwindows.org/).
After copying your username, password, and installing Git if needed, head over to VSCode and create a new terminal with the toolbar at the top. Select the downward arrow on the righthand side and select Git Bash to change the terminal.

![Git Bash & Terminal](https://raw.githubusercontent.com/Yves-M22/cse15l-lab-reports/main/images/Screenshot%202023-04-08%20185625.png)

    @Test
  public void testReverseInPlaceWithArrayLength2() {
    int[] input1 = {1, 2};
    ArrayExamples.reverseInPlace(input1);
    assertArrayEquals(new int[]{ 2, 1 }, input1);
 } 

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
