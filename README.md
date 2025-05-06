# COMP1210-Project-IceCreamCone-List2-Menu-App-

Download Here: [COMP1210 Project: IceCreamCone List2 Menu App ](https://codingherolab.com/product/comp1210-project-icecreamcone-list2-menu-app/)

For Custom/Original Work email codingprolab@gmail.com/whatsapp +1(541)423-7793

Overview: The objective is to modify your Project 6 to use arrays instead of ArrayList objects. You
will write a program this week that is composed of three classes: the first class defines IceCreamCone
objects, the second class defines IceCreamConeList2 objects, and the third,
IceCreamConeList2MenuApp, presents a menu to the user with eight options and implements these:
(1) read input file (which creates an IceCreamConeList2 object), (2) print report, (3) print summary,
(4) add an IceCreamCone object to the IceCreamConeList2 object, (5) delete an IceCreamCone
object from the IceCreamConeList2 object, (6) find an IceCreamCone object in the
IceCreamConeList2 object, (7) Edit an IceCreamCone in the IceCreamConeList2 object, and (8) quit
the program. [You should create a new “Project 7” folder and copy your Project 6 files
(IceCreamCone.java, IceCreamConeList.java, IceCreamConeListMenuApp.java,
IceCreamCone_data_1.txt, and IceCreamCone_data_0.txt) to it, rather than work in the same
folder as Project 6 files.]
To rename an existing .java file, open the file in jGRASP, change the name of the class
and the name of the constructor (if it has one) in the source file, and then click the Save button.
In the dialog that pops up, click the “Rename and Save” button. This will rename and save the
.java file and delete the old associated .class file.
• IceCreamCone.java (assuming that you successfully created this class in Project 4, 5, or 6,
just copy the file to your new Project 7 folder and go on to IceCreamConeList2.java on page
4. Otherwise, you will need to create IceCreamCone.java as part of this project.)
Requirements: Create an IceCreamCone class that stores the label, radius, and height. The
radius and height must be greater than zero. The IceCreamCone class also includes methods to set
and get each of these fields, as well as methods to calculate the surface area and volume of the
cone, hemisphere, and the IceCreamCone object, and a method to provide a String value of an
IceCreamCone object (i.e., a class instance).
Project: IceCreamCone List2 Menu App Page 2 of 11
Page 2 of 11
An ice cream cone is a cone with a hemisphere on top as depicted below with cone height h
and cone radius r, where r is also the radius of the hemisphere. The formulas are provided to
assist you in computing return values for the respective methods in the IceCreamCone class
described in this project.
radius (r)
height (h)
Cone Side Area (cA)
Hemisphere Area (hA)
Surface Area (A)
Cone Volume (cV)
Hemisphere Volume (hV)
Volume (V)
�� = � � ‘ℎ) + �)
ℎ� = 2 ��)
� = �� + ℎ�
�� = ℎ��)⁄3
ℎ� = 2��/⁄3
� = �� + ℎ�
Design: The IceCreamCone class has fields, a constructor, and methods as outlined below.
(1) Fields (instance variables): label of type String, radius of type double, and height of type
double. Initialize the String to “” and the double to 0 in their respective declarations. These
instance variables should be private so that they are not directly accessible from outside of the
IceCreamCone class, and these should be the only instance variables in the class.
(2) Constructor: Your IceCreamCone class must contain a public constructor that accepts three
parameters (see types of above) representing the label, radius, and height. Instead of
assigning the parameters directly to the fields, the respective set method for each field
(described below) should be called. For example, instead of the statement label =
labelIn; use the statement setLabel(labelIn); Below are examples of how the
constructor could be used to create IceCreamCone objects. Note that although String and
numeric literals are used for the actual parameters (or arguments) in these examples, variables
of the required type could have been used instead of the literals.
IceCreamCone ex1 = new IceCreamCone(“Ex 1″, 1, 2);
IceCreamCone ex2 = new IceCreamCone(” Ex 2 “, 12.3, 25.5);
IceCreamCone ex3 = new IceCreamCone(“Ex 3”, 123.4, 900);
(3) Methods: Usually a class provides methods to access and modify each of its instance
variables (known as get and set methods) along with any other required methods. The
methods for IceCreamCone, which should each be public, are described below. See formulas
in Code and Test below.
o getLabel: Accepts no parameters and returns a String representing the label field.
o setLabel: Takes a String parameter and returns a boolean. If the string parameter is
not null, then the label field is set to the “trimmed” String and the method returns true.
Otherwise, the method returns false and the label field is not set.
Project: IceCreamCone List2 Menu App Page 3 of 11
Page 3 of 11
o getRadius: Accepts no parameters and returns a double representing the radius field.
o setRadius: Accepts a double parameter and returns a boolean as follows. If the
double is greater than zero, sets the radius field to the double passed in and returns true.
Otherwise, the method returns false and does not set the radius field.
o getHeight: Accepts no parameters and returns a double representing the height field.
o setHeight: Accepts a double parameter and returns a boolean as follows. If the
double is greater than zero, sets the height field to the double passed in and returns true.
Otherwise, the method returns false and does not set the height field.
o surfaceArea: Accepts no parameters and returns the double value for the total
surface area calculated using formula above and the values of the radius and height fields.
o volume: Accepts no parameters and returns the double value for the volume calculated
using formula above and the values of the radius and height fields.
o toString: Returns a String containing the information about the IceCreamCone object
formatted as shown below, including decimal formatting (“#,##0.0######”) for the
double values. Newline and tab escape sequences should be used to achieve the proper
layout. In addition to the field values (or corresponding “get” methods), the following
methods should be used to compute appropriate values in the toString method:
surfaceArea() and volume(). Each line should have no trailing spaces (e.g., there
should be no spaces before a newline (\n) character). The toString value for ex1, ex2,
and ex3 respectively are shown below (the blank lines are not part of the toString
values).
IceCreamCone “Ex 1” with radius = 1.0 and height = 2.0 units has:
surface area = 13.308 square units
volume = 4.1887902 cubic units
IceCreamCone “Ex 2” with radius = 12.3 and height = 25.5 units has:
surface area = 2,044.5837657 square units
volume = 7,937.3689278 cubic units
IceCreamCone “Ex 3” with radius = 123.4 and height = 900.0 units has:
surface area = 447,847.2056927 square units
volume = 18,287,175.0307675 cubic units
Code and Test: As you implement your IceCreamCone class, you should compile it and then test
it using interactions. For example, as soon you have implemented and successfully compiled the
constructor, you should create instances of IceCreamCone in interactions (e.g., copy/paste the
examples above). Remember that when you have an instance on the workbench, you can unfold
it to see its values. You can also open a viewer canvas window and drag the instance from the
Workbench tab to the canvas window. After you have implemented and compiled one or more
methods, create an IceCreamCone object in interactions and invoke each of your methods on the
object to make sure the methods are working as intended. You may find it useful to create a
separate class with a main method that creates an instance of IceCreamCone then prints it out.
This would be similar to the IceCreamConeApp class you will create below, except that in the
IceCreamConeApp class you will read in the values and then create and print the object.
Project: IceCreamCone List2 Menu App Page 4 of 11
Page 4 of 11
• IceCreamConeList2.java – You must use arrays instead of ArrayList objects. (Assuming
that you successfully created this class in Project 6, just copy IceCreamConeList.java to
your new Project 7 folder. Otherwise, you will need to create all of
IceCreamConeList2.java as part of this project. To rename the existing .java file to
IceCreamConeList2, open the file in jGRASP, change the name of the class and the name of
the constructor in the source code, and then click the Save button. In the dialog that pops
up, click the “Rename and Save” button. This will rename and save the .java file and then
delete old associated .class file). In the requirements below, IceCreamConeList has been
changed to IceCreamConeList2. Be sure to make these changes in your methods as necessary.
Requirements: Create an IceCreamConeList2 class that stores the name of the list and an array
of IceCreamCone objects, and the number of IceCreamCone objects in the array. It also includes
methods that return the name of the list, number of IceCreamCone objects in the
IceCreamConeList2, total surface area, total volume, average surface area, and average volume
for all IceCreamCone objects in the IceCreamConeList2. The toString method returns a String
containing the name of the list followed by each IceCreamCone in the array, and a summaryInfo
method returns summary information about the list (see below).
Design: The IceCreamConeList2 class has three fields, a constructor, and methods as outlined
below.
(1) Fields (or instance variables): (1) a String representing the name of the list, (2) an array of
IceCreamCone objects, and (3) an int representing the number of IceCreamCone objects in
the IceCreamCone array. These are the only fields (or instance variables) that this class
should have.
(2) Constructor: Your IceCreamConeList2 class must contain a constructor that accepts a
parameter of type String representing the name of the list, a parameter of type
IceCreamCone[], representing the list of IceCreamCone objects, and a parameter of type
int representing the number of IceCreamCone objects in the IceCreamCone array. These
parameters should be used to assign the fields described above (i.e., the instance variables).
(3) Methods: Methods: The methods for IceCreamConeList are described below.
o getName: Returns a String representing the name of the list.
o numberOfIceCreamCones: Returns an int representing the number of
IceCreamCone objects in the IceCreamConeList. Note that this is the value of the third
field in the class, not the length of the array.
o totalSurfaceArea: Returns a double representing the total surface areas for all
IceCreamCone objects in the list. If there are zero IceCreamCone objects in the list, zero
should be returned.
o totalVolume: Returns a double representing the total volumes for all IceCreamCone
objects in the list. If there are zero IceCreamCone objects in the list, zero should be
returned.
Project: IceCreamCone List2 Menu App Page 5 of 11
Page 5 of 11
o averageSurfaceArea: Returns a double representing the average surface area for
all IceCreamCone objects in the list. If there are zero IceCreamCone objects in the list,
zero should be returned.
o averageVolume: Returns a double representing the average volume for all
IceCreamCone objects in the list. If there are zero IceCreamCone objects in the list, zero
should be returned.
o toString: Returns a String (does not begin with \n) containing the name of the list
followed by each IceCreamCone in the array. In the process of creating the return result,
this toString() method should include a while loop that calls the toString() method for
each IceCreamCone object in the list (adding a \n before and after each). Be sure to
include appropriate newline escape sequences. For an example, see lines 2 through 16 in
the output from the original IceCreamConeListApp for the IceCreamCone_data_1.txt
input file. [Note that the toString result should not include the summary items in lines 18
through 24 of the example. These lines represent the return value of the summaryInfo
method.]
o summaryInfo: Returns a String (does not begin with \n) containing the name of the
list (which can change depending of the value read from the file) followed by various
summary items: number of IceCreamCone objects, total surface area, total volume,
average surface area, and average volume. Use “#,##0.0##” as the pattern to format the
double values. For an example, see lines 18 through 24 in the output from the original
IceCreamConeListApp for the IceCreamCone_data_1.txt input file. The second example
shows the output from IceCreamConeList2App for the IceCreamCone_data_0.txt input
file which contains a list name but no IceCreamCone data.
o getList: Returns the array of IceCreamCone objects (the second field above).
o readFile: Takes a String parameter representing the file name, reads in the file,
storing the list name and creating an array of IceCreamCone objects, uses the list name,
the array, and number of IceCreamCone objects in the array to create an
IceCreamConeList2 object, and then returns the IceCreamConeList2 object. See note #1
under Important Considerations for the IceCreamConeList2MenuApp class (last page) to
see how this method should be called.
o addIceCreamCone: Returns nothing but takes three parameters (label, radius, and
height), creates a new IceCreamCone object, and adds it to the IceCreamConeList2
object. Finally, the number of IceCreamCone objects field must be incremented.
o findIceCreamCone: Takes a label of an IceCreamCone as the String parameter and
returns the corresponding IceCreamCone object if found in the IceCreamConeList2
object; otherwise returns null. Case should be ignored when attempting to match the
label.
o deleteIceCreamCone: Takes a String as a parameter that represents the label of the
IceCreamCone and returns the IceCreamCone if it is found in the IceCreamConeList2
object and deleted; otherwise returns null. Case should be ignored when attempting to
match the label; consider calling/using findIceCreamCone in this method. When an
element is deleted from an array, elements to the right of the deleted element must be
shifted to the left. After shifting the items to the left, the last IceCreamCone element in
the array should be set to null. Finally, the number of IceCreamCone objects field must
be decremented.
o editIceCreamCone: Takes three parameters (label, radius, and height), uses the label to
find the corresponding the IceCreamCone object. If found, sets the radius and height to
Project: IceCreamCone List2 Menu App Page 6 of 11
Page 6 of 11
the values passed in as parameters, and returns true. If not found, returns false. This
method should not change the label.
Code and Test: Remember to import java.util.Scanner, java.io.File,
java.io.FileNotFoundException. These classes will be needed in the readFile method which will
require a throws clause for FileNotFoundException. Some of the methods above require that you
use a loop to go through the objects in the array. You may want to implement the class below in
parallel with this one to facilitate testing. That is, after implementing one to the methods above,
you can implement the corresponding “case” in the switch for menu described below in the
IceCreamConeList2MenuApp class.
• IceCreamConeList2MenuApp.java (replaces IceCreamConeListMenuApp class from Project
6; the file and class name in the file must be renamed to reflect IceCreamConeList2MenuApp).
To rename an existing .java file, open the file in jGRASP, change the name of the class in
the source code, and then click the Save button. In the dialog that pops up, click the
“Rename and Save” button. This will rename the .java file, save it, and delete the old
associated .class file. Be sure to make these changes in your main method as necessary.
Requirements: Create an IceCreamConeList2MenuApp class with a main method that presents
the user with a menu with eight options, each of which is implemented to do the following: (1)
read the input file and create an IceCreamConeList2 object, (2) print the IceCreamConeList2
object, (3) print the summary for the IceCreamConeList2 object, (4) add an IceCreamCone object
to the IceCreamConeList2 object, (5) delete an IceCreamCone object from the
IceCreamConeList2 object, (6) find an IceCreamCone object in the IceCreamConeList2 object,
(7) edit an IceCreamCone object in the IceCreamConeList2 object, and (8) quit the program.
Design: The main method should print a list of options with the action code and a short
description followed by a line with just the action codes prompting the user to select an action.
After the user enters an action code, the action is performed, including output if any. Then the
line with just the action codes prompting the user to select an action is printed again to accept the
next code. The first action a user would normally perform is ‘R’ to read in the file and create an
IceCreamConeList2 object. However, the other action codes should work even if an input file
has not been processed. The user may continue to perform actions until ‘Q’ is entered to quit (or
end) the program. Note that your program should accept both uppercase and lowercase action
codes. Below is output produced after printing the action codes with short descriptions, followed
by the prompt with the action codes waiting for the user to make a selection from the menu.
Project: IceCreamCone List2 Menu App Page 7 of 11
Page 7 of 11
Line # Program output
1
2
3
4
5
6
7
8
9
10
IceCreamCone List System Menu
R – Read File and Create IceCreamCone List
P – Print IceCreamCone List
S – Print Summary
A – Add IceCreamCone
D – Delete IceCreamCone
F – Find IceCreamCone
E – Edit IceCreamCone
Q – Quit
Enter Code [R, P, S, A, D, F, E, or Q]:
Below shows the screen after the user entered ‘r’ and then (when prompted) the file name. Notice
the output from this action was “File read in and IceCreamCone List created”. This is followed
by the prompt with the action codes waiting for the user to make the next selection. You should
use the IceCreamCone_data_1.txt file from Project 5 to test your program.
Line # Program output
1
2
3
4
5
Enter Code [R, P, S, A, D, F, E, or Q]: r
File Name: IceCreamCone_data_1.txt
File read in and IceCreamCone List created
Enter Code [R, P, S, A, D, F, E, or Q]:
The result of the user selecting ‘p’ to Print IceCreamCone List is shown below and next page.
Line # Program output
1
2
3
4
5
6
7
8
9
10
11
12
13
14
15
16
Enter Code [R, P, S, A, D, F, E, or Q]: p
IceCreamCone Test List
IceCreamCone “Ex1” with radius = 1.0 and height = 2.0 units has:
surface area = 13.308 square units
volume = 4.1887902 cubic units
IceCreamCone “Ex 2” with radius = 12.3 and height = 25.5 units has:
surface area = 2,044.5837657 square units
volume = 7,937.3689278 cubic units
IceCreamCone “Ex 3” with radius = 123.4 and height = 900.0 units has:
surface area = 447,847.2056927 square units
volume = 18,287,175.0307675 cubic units
Enter Code [R, P, S, A, D, F, E, or Q]:
Project: IceCreamCone List2 Menu App Page 8 of 11
Page 8 of 11
The result of the user selecting ‘s’ to print the summary for the list is shown below.
Line # Program output
1
2
3
4
5
6
7
8
9
10
Enter Code [R, P, S, A, D, F, E, or Q]: s
—– Summary for IceCreamCone Test List —–
Number of IceCreamCone Objects: 3
Total Surface Area: 449,905.097
Total Volume: 18,295,116.588
Average Surface Area: 149,968.366
Average Volume: 6,098,372.196
Enter Code [R, P, S, A, D, F, E, or Q]:
The result of the user selecting ‘a’ to add an IceCreamCone object is shown below. Note that
after ‘a’ was entered, the user was prompted for label, radius, and height. Then after the
IceCreamCone object is added to the IceCreamCone List, the message “*** IceCreamCone added
***” was printed. This is followed by the prompt for the next action. After you do an “add”, you
should do a “print” or a “find” to confirm that the “add” was successful.
Line # Program output
1
2
3
4
5
6
7
Enter Code [R, P, S, A, D, F, E, or Q]: a
Label: Ex 4
Radius: 10.5
Height: 1000
*** IceCreamCone added ***
Enter Code [R, P, S, A, D, F, E, or Q]:
Here is an example of the successful “delete” for an IceCreamCone object, followed by an
attempt that was not successful (i.e., the IceCreamCone object was not found). You should do
“p” to confirm the “d”.
Line # Program output
1
2
3
4
5
6
7
8
9
Enter Code [R, P, S, A, D, F, E, or Q]: d
Label: ex 2
“Ex 2” deleted
Enter Code [R, P, S, A, D, F, E, or Q]: d
Label: Fake
“Fake” not found
Enter Code [R, P, S, A, D, F, E, or Q]:
Project: IceCreamCone List2 Menu App Page 9 of 11
Page 9 of 11
Here is an example of the successful “find” for an IceCreamCone object, followed by an attempt
that was not successful (i.e., the IceCreamCone object was not found).
Line # Program output
1
2
3
4
5
6
7
8
9
10
11
Enter Code [R, P, S, A, D, F, E, or Q]: f
Label: ex 3
IceCreamCone “Ex 3” with radius = 123.4 and height = 900.0 units has:
surface area = 447,847.2056927 square units
volume = 18,287,175.0307675 cubic units
Enter Code [R, P, S, A, D, F, E, or Q]: f
Label: another fake
“another fake” not found
Enter Code [R, P, S, A, D, F, E, or Q]:
Here is an example of the successful “edit” for an IceCreamCone object, followed by an attempt
that was not successful (i.e., the IceCreamCone object was not found). In order to verify the edit,
you should do a “find” for “medium” or you could do a “print” to print the whole list.
Line # Program output
1
2
3
4
5
6
7
8
9
10
11
12
13
Enter Code [R, P, S, A, D, F, E, or Q]: e
Label: Ex 3
Radius: 250
Height: 1000
“Ex 3” successfully edited
Enter Code [R, P, S, A, D, F, E, or Q]: e
Label: Ex 33
Radius: 1.5
Height: 4.5
“Ex 33” not found
Enter Code [R, P, S, A, D, F, E, or Q]:
Finally, below is an example of entering an invalid code, followed by an example of entering a
‘q’ to quit the application with no message.
Line # Program output
1
2
3
4
5
Enter Code [R, P, S, A, D, F, E, or Q]: k
*** invalid code ***
Enter Code [R, P, S, A, D, F, E, or Q]: q
Project: IceCreamCone List2 Menu App Page 10 of 11
Page 10 of 11
Code and Test:
Important considerations: This class should import java.util.Scanner and
java.io.FileNotFoundException. Carefully consider the following information as you develop
this class.
1. At the beginning of your main method, you should declare and create an array of
IceCreamCone objects and then declare and create an IceCreamConeList2 object using the
list name, the array, and 0 as the parameters in the constructor. This will be an
IceCreamConeList2 object that contains no IceCreamCone objects. For example:
String _______ = “*** no list name assigned ***”;
IceCreamCone[] _________ = new IceCreamCone[100];
IceCreamConeList2 _________ = new IceCreamConeList2(_________,_________,_________);
The ‘R’ option in the menu should invoke the readFile method on your IceCreamConeList2
object. This will return a new IceCreamConeList2 object based on the data read from the
file, and this new IceCreamConeList2 object should replace (be assigned to) your original
IceCreamConeList2 object variable in main. Since the readFile method throws
FileNotFoundException, your main method needs to do this as well.
2. Very Important: You should declare only one Scanner on System.in for your entire
program, and this should be done in the main method. That is, all input from the
keyboard (System.in) must be done in your main method. Declaring more than one Scanner
on System.in in your program will likely result in a very low score from Web-CAT.
3. For the menu, your switch statement expression should evaluate to a char and each case
should be a char; alternatively, your switch statement expression should evaluate to a String
with a length of 1 and each case should be a String with a length of 1.
After printing the menu of actions with descriptions, you should have a do-while loop that prints
the prompt with just the action codes followed by a switch statement that performs the indicated
action. The do-while loop ends when the user enters ‘q’ to quit. You should strongly consider
using a for-each loop as appropriate in the new methods that require you to search the list. You
should be able to test your program by exercising each of the action codes. After you implement
the “Print IceCreamCone List” option, you should be able to print the IceCreamConeList2 object
after operations such as ‘A’ and ‘D’ to see if they worked. You may also want to run in debug
mode with a breakpoint set at the switch statement so that you can step-into your methods if
something is not working. In conjunction with running the debugger, you should also create a
canvas drag the items of interest (e.g., the Scanner on the file, your IceCreamConeList2 object,
etc.) onto the canvas and save it. As you play or step through your program, you’ll be able to see
the state of these objects change when the ‘R’, ‘A’, and ‘D’ options are selected.
a. For option P, when you print the IceCreamConeList2 object (e.g., myList) be sure to
append a leading “\n” in println:
System.out.println(“\n” + myList);
Project: IceCreamCone List2 Menu App Page 11 of 11
Page 11 of 11
b. For option S, when you print the summary for IceCreamConeList2 object (e.g., cList)
be sure to append a leading and trailing “\n” in the .println:
System.out.println(“\n” + myList.summaryInfo() + “\n”);
Although your program may not use all of the methods in your IceCreamCone and
IceCreamConeList2 classes, you should ensure that all of your methods work according to the
specification. You can run your program in the canvas and then after the file has been read in,
you can call methods on the IceCreamConeList2 object in interactions or you can write another
class and main method to exercise the methods. Web-CAT will test all methods to determine
your project grade.
