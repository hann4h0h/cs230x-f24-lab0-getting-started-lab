[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/FLMsUR8t)
# CS230X-lab0-S24
# Lab 0 for CS230X 
In this lab, you will get started with the tools we will use this semester for labs and assignments.

Goals:
- Creating a Github account and review basics of Git
- Start working with BlueJ
- Write some simple java programs
- Learn how to submit your work on Gradescope

## Task 1: Organizing your work
Try to be well organized in your work. Start by creating a CS230X folder to keep your work on your computer’s Desktop, for easy access, or in your Documents, and name it appropriately. 

## Task 2: Git and Github for CS230X
In this class we will use Github to release assignments and labs. The instructions will be available in the README files of each assignment and lab, and the repository will contain the starter code when available. 

1) Create a Github account
2) Familiarize yourself with Git
3) Clone the starter code for this assignment

## Task 3: Meet BlueJ
In CS230X, we will use BlueJ to develop, test, compile, and run our Java programs. Compiling a Java program converts Java source code (files ending in .java) into something called bytecodes (files ending in .class) which can then be understood by the computer.

1) Download the BlueJ application to your own computer for free by visiting the BlueJ site for information and downloads. 
2) Please visit this BlueJ documentation page, which contains pointers to reference material as well as some nice tutorials (including video tutorials). 

Once you start BlueJ, a window should open. Please examine its components carefully: 
In BlueJ, Java code is organized in Projects. Let's create our first New Project in BlueJ:
Name it lab0Project, and save it into the lab0_yourname folder on your Desktop. This project will contain all the java files we will write today. At this point, your first java Project has been created.
 
## Task 3: Basic Programming in Java

### Create your first Java class: Profile.java
1) In the BlueJ project window, click on the New Class... button. Name the new class Intro and click ok. An "Intro" icon should appear in the project window. Note the diagonal lines decorating the "Intro" icon; it means the class has not been compiled yet:

2) To see the code associated with the Intro.java class, simply double-click on the "Intro" icon (or, control-click on the "Intro" icon, and from the pop-up menu select the option "Open Editor"). A new Editor Window will open, showing the class's source code.
Examine the template of the source code. It contains the "anatomy" of a java class:
top-of-the-file comments 
body of the class definition, which contains:
instance variable(s)
constructor(s)
method(s)

3) Add a main() method
When running a java class, execution starts from the main() method of that class. At the bottom of the Intro.java file, and before the last closing curly-bracket 
} 
add the definition of the main() method, exactly as you see it right below:

You do not need to remove the template code above your code (though you can), because only the main() method (as shown above) will be executed.

4) Compile a class
To compile the Intro class just click on the "Compile" button, at the top-left of the Editor window. Alternatively, you can go back to the lab0Project window, control-click on the class icon, and from the pop-up window, select "Compile". If all goes well, and your compilation is successful (i.e no compilation/syntax errors), you should see that the icon of the class is no longer decorated with diagonal lines. That's what you want! If not, you need to fix any syntax errors your code contains, before you are ready to move on.

5) Run a class
In the lab0Project window, control-click on the class's icon, and select to run the main() method:

An input window will appear. Just click OK for now, we will talk about that in a few weeks.
A Terminal Window should open up, and the greeting should be printed in there!
That's it! You now know how to create a new java class, how to compile it and run it, all within the BlueJ environment!

6) In this task, we will create a better Intro class: We will introduce ourselves to the user by name!
Then write the main() method inside class Intro2 to look like this: (Feel free to copy and paste here but edit the @author and @version accordingly.)

/** Intro2 - My second program!
 * @author (Write your name here)
 * @version (Write today's date here)
 */
public class Intro2 {
     public static void main(String [] args) {
     //replace the values of the following variables as you wish
        String name = "Catherine";
        int gradYear = 2009;
        double money = 12.53;
        boolean csMajor = true;
        System.out.println("Hello there! My name is " + name + ".");
        System.out.println("I am Wellesley class of " + gradYear + ".");
        System.out.println("I am a computer science major: " + csMajor);
        System.out.println("And, I'll buy you coffee! I have $" + money + " on me.");
    }
}


Notice that Java (as opposed to Python) is a strongly typed language, which means that it is required that every variable is declared with its type before use. Experiment with removing some of the variable declarations in your code and see what happens. Read, and familiarize yourselves with the error messages that will be produced.

Task 3B: The Java API
Open a new tab in your browser's window, and load the following page:
https://docs.oracle.com/javase/8/docs/api/
This is the online java documentation for every class in the language. We recommend that you always have this page loaded when you set up to do any cs230 work.

Task 3C: Java documentation
There are three kinds of comments in java:
Use the // to indicate one-line comments
Use the /* */ to indicate multiple-line comments
Use the /** */ to write javadoc (documentation in proper style)
Add some comments to your code.
A first word on javadoc: Javadoc is a documentation tool which defines a standard format for comments, and which can generate HTML files to view the documentation from a web browser. (As an example, see Oracle's Javadoc documentation for the Java libraries at https://docs.oracle.com/javase/8/docs/api/.) We will talk and start using javadoc soon in this class, but for now, here are a couple of resources on it:
https://en.wikipedia.org/wiki/Javadoc
https://www.oracle.com/technetwork/java/javase/documentation/index-137868.html

DATA CONVERSION
In Java, everything is represented using objects, except for the following eight primitive data types:
Integers (have no fractional part)
byte (1 byte of memory space)
short (2 bytes of memory space)
int (4 bytes of memory space)
long (8 bytes of memory space)
Decimal numbers (do have fractional part)
float (4 bytes of memory space)
double (8 bytes of memory space)
We need to be careful when converting (explicitly or implicitly) one type to another!

To practice with data conversions, look at the Conversions.java file in this repository. If you try compiling this class, you will immediately see some errors. Try fixing the methods definitions and completing the requested methods. 

## SUBMITTING
Turn in your work submitting files Profile.java and Conversions.java to your Gradescope account for Lab0. You will receive full credit for this lab if you submit a reasonable attempt at completing the lab by the deadline. [Click here for Gradescope instructions.](https://docs.google.com/document/d/1zGAJrbdAhfPZVlyDP9N3MmdKXWvNo7rQqehKNM5Q0_M/edit) 

## AUTOGRADER
When you submit your lab to Gradecope, you will immediately see some feedback through the autograder. You are welcome to resubmit as many times as you wish until the deadline. The autograder will check for accuracy, style, and documentation. Make sure there are no remaining `TODO` comments in your submission code. Click here for 230X instructions on: [testing your code](https://docs.google.com/document/d/19cKOyolT8UtSfMNrVw8MGgVWS-lYgHpBs8g2Cf_8Vvc/edit#heading=h.rt39ohf1jp6s), [styling your code](https://docs.google.com/document/d/14uwj9HAjNKfFBm0ZjUpWR7jdqKSj13rudIEJaG74mPk/edit), and [documenting your code](https://docs.google.com/document/d/15uqs_NH8y2sAuLLpiZuSxlI0UsL6a8CHuWY_qcvF4B4/edit). 

## LAB SOLUTIONS
Lab solutions will be added to this repository after the lab deadline. 
