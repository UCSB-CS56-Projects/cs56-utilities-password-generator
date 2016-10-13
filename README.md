M16-cs56-Password-Generator-lab08
=============================

Contributors:

* JH Peng and Sunimal E.: https://github.com/EdieS/cs56-utilities-password-generator

JavaDoc: http://www.cs.ucsb.edu/~108498asdf//cs56/W11/issues/0000042/javadoc


project history
===============

```
High-Level Description(User's View)
===================================

This is a program that creates a random password with a given length of max and min. You can also input a list of special 
characters that can be added to the library of special characters that will be used to create the password.In the current state, 
I have implemented everything that it is suppose to do.


Some Internal Documentation(Developer's View)
=============================================

1. The main GUI code is located in PasswordGUI.java. 

2. This is the main function that generates the output. It also calls other functions to do stuff.
    ```java
	public String generate(int min, int max, ArrayList<CharType> userSpec)
	 {
	 // code here 
	 }
    ```
3. class Password has all the variables that are used in this project.  class PasswordGUI contains all the GUI swing elements.

How to run this project?
========================

git clone the Repo then open the git project as a new Java Project in eclipse
then choose the class you want to run
Or clone the project and run ant

M16 Final Remarks
=================
We were asked to leave a note to whoever receives this project in the future. Here's some information about each source code 
file in the src folder.

Password.java contains the definition of the structure of a password, namely what a password contains (its definition)

PasswordGenerator.java contains the logic of the generate algorithm. Namely the generate() method and other helper functions

PasswordGUI.java is a view for the GUI version of the program. It currently inherits PasswordGenerator.

CharType.java holds the class for CharType. More on that below.

Perhaps the biggest change we made was the addition of this "CharType" class, which divides the characters that make up a 
password into four distinct types: uppercase letters, lowercase letters, digits, and special characters. We believe the generate 
algorithm is pretty straightforward now that it uses these objects (and if you have trouble understanding it, the code is 
heavily commented in that area).

We currently have a commented out section in PasswordGUI that lets users generate x numbers of password of a given spec and save 
it to a txt file

One final thought if you REALLY want to go above and beyond: Generated passwords are secure, but hard to remember. If all of 
your passwords are generated by this program, how do you expect to remember them all? A good addition to the program would be 
the ability to store passwords (securely) so a user can remember them if ever forgotten.

Good luck,
JH Penger and Edie S.

```

# Note from M16 mentor:
This project was completely rewritten during M16 (Summer Session A 2016). In order to merge the new project with the old, an M16 
branch had to be created with the forked branch's work (via pull). The master branch is now fully updated (07/29/16).
~Christian Newkirk 
