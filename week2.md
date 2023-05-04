**Lab Report 2 - Servers & Bugs**

*Part 1 - String Server*

Using the code based off of 
# NumberServer.java 
from week 2, I created a simple alternate version that stores a string from input in the url and adds on to it. There's some code to show how it functions, as well as two screenshots of add-message implementation at work.

![Image of StringServer Code](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230322.png?raw=true) 



![Image of AddMessage-1](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230424.png?raw=true)   

For this example of how add message is used, in the specific moment shown, handle request is called and skips the first if statement since there's more characters beyond the '/'. It goes through the method to add the inputted string since add-message comes after the '/', where the string is then returned and seen on the site. The method takes in any argument that is of type URI, and the following if statements check specific strings to determine what should be done. The value for the URI field would be a url, while the input for the if statements check strings. There's also a string named input for the method. Whenever /add-message is used, the value of String input is being changed by adding a new portion of a string and a new line chracter. In the image, "I love ECE 35" and a new line character is stored.   



![Image of AddMessage-2](https://github.com/Yves-M22/cse15l-lab-reports/blob/main/images2/Screenshot%202023-04-24%20230457.png?raw=true)

This example is similar to the last one with the only difference being the addition of another string into input. The same method is called as in the first example, and will go through the same lines of code to add this new string into the input. When /add-message is used, the value of String input is changed by adding "So much :D" to input, which sould already contain something from previously using /add-message. After this is called, input now contains "I love ECE 35" and "So much :D" with a new line character between them and after the second added message.

*Part 2 - Array Bugs*

Test that fails program

    @Test
    public void testReversedWithArrayLength3() {
        int[] input1 = {3, 6, 9};
        assertArrayEquals(new int[]{9, 6, 3}, ArrayExamples.reversed(input1));
    }
  
Test that can pass the program

    @Test
    public void testReversed() {
        int[] input1 = { };
        assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
    }
    

These are two JUnit tests that tests whether the Reversed method works properly with different inputs, which are arrays that are reversed and returned. 


*Part 3 - Reflection on Lab*

I've already done a lot of debugging and testing in CSE 12 last quarter, and that wasn't my favorite thing to do, so learning that in lab wasn't very intuitive, but learning more about how servers work in week 2 and using the remote computers in tangent with that was new to me. Integrating and making code that made some changes to a site felt more impactful and different from what I've coded in the past. I aslo enjoyed learning more about GitHub the last two weeks since I;m sure these are useful skills to have and I feel as if I've developed a better understanding of GitHub pages and the desktop interface for it. 
