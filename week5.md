# **Lab Report 5 - Debugging/Reflection**

## Part 1 ##

### Student's Post ### 
![Image of Student post](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images5/Screenshot%202023-06-04%20213607.png?raw=true) 

![Image of Student screenshot](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images5/Screenshot%202023-06-04%20194207.png?raw=true) 

### TA Response ###

It seems like eveyrthing should be fine from the command-line, so it seems like you are using the correct command and file you inteded to use. I would use vim ```grade.sh``` to edit through the java file. Based on the error message, there seems to be an issue when it comes to compiling/testing the file.

### Student Solution ### 

![Image of Student solution 1](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images5/Screenshot%202023-06-04%20220748.png?raw=true) 

![Image of Student solution 2](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images5/Screenshot%202023-06-04%20220808.png?raw=true) 

- After trying what that, I went through the two files responsible for compiling the tests, and saw tat there were no issues with the test themselves, but with the file being ran. There was an issue running the TestListExamples file. The file was already compiled, but when using java to try and run the tests, it was looking for a java file rather than the class file. 

- To setup this debugging scenario, you'll need to log onto ieng6 and use git clone to copy [this repository](https://github.com/ucsd-cse15l-f22/list-examples-grader/blob/main/grade.sh). Once you've done that the grade.sh file should be edited so the java command is ran on ```TestListExamples.java``` instead of just TestListExamples. Running the command, ```bash grade.sh https://github.com/ucsd-cse15l-f22/list-methods-lab3``` will trigger the bug since the bug is found within grade.sh rather than being in the command-line. To fix the bug, you'll need to go to make sure you're in the correct directory with the cloned repository and check using ```ls```. You then use ```vim``` to edit the ```ListExamples.java``` file to fix the bug by making sure the java command is looking for the correct file. Exiting vim and running the bash command should show the intended output.

## Part 2 ##

