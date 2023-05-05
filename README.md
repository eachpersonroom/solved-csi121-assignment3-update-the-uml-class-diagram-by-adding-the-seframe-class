Download Link: https://assignmentchef.com/product/solved-csi121-assignment3-update-the-uml-class-diagram-by-adding-the-seframe-class
<br>
This assignment requires you to write a program that designs and creates the graphic user interface (GUI) for the student enrolment system by using Java Swing.

Background

Assignment 3 is based on the Assignments 1&amp;2 (please see Moodle for Assignment 1&amp;2’s solutions). Please refer to A1’s description for the Bachelor of Computer Science course structure and A2’s description for the Master of Computer Science course structure.

You are required to design, implement and test a student system with GUI to 1) load BCS or MCS course structure via the Java ObjectInputStream; 2) to enrol one student into either the Bachelor of Computer Science course or the Master of Computer Science; and 3) to save the student enrolment information into a text file. The detailed steps are as follows:

<ol>

 <li>Upgrade your UML diagram.</li>

</ol>

You should upgrade your existing UML diagram for Assignment 3 by considering the new GUI class (named SEFrame extending JFrame).

<ol start="2">

 <li>Design a GUI.</li>

</ol>

The SEFrame class shall contain some basic Swing components such as JLabel, JTextField, JButton, JList and etc. With the new GUI, a user shall able to input his/her personal information, to select a course (either BCS or MCS), to select a major within the course and to select some elective subjects to complete the enrolment. An example of the GUI is displayed as follows. You can either use this GUI layout or design your own GUI.

<ol start="3">

 <li>Load BCS or MCS course structure via Java ObjectInputStream</li>

</ol>

The Java ObjectInputStream shall be used to load either BCS (“bcs.ser”) or MCS (“mcs.ser”) course structure to the system. The given “bcs.ser” and “mcs.ser” files are generated based on A2’s solutions. If you make any modification of A2’s classes, you shall create new “bcs.ser” and “mcs.ser” files by using the Lab5’s program. The given example shows the BCS or MCS course structure after clicking the “Bachelor of Computer Science Course Structure” or the “Master of Computer Science Course Structure” button.

(by clicking the “Bachelor of Computer Science Course Structure” button)

(by clicking the “Master of Computer Science Course Structure” button)

<ol start="4">

 <li>Select a major for a course.</li>

</ol>

After a course structure is loaded.

<ol>

 <li>The system shall automatically enroll all core subjects and update the total enrolled credits (96 cp for BCS, 54 cp for MCS).</li>

 <li>To allow the user to select a major and show the major core subjects. The system shall automatically update the total enrolled credits after the user selects a major (enrolling the user to all major core subjects automatically). The user is only allowed to select ONE major. For example, in MCS, if the user selects the Intelligent System Major or the Machine Learning and Big Data Major, the three major core subjects shall be displayed on the right side and the enrolled total credits shall be updated automatically. The elective subject list shall also be updated automatically by removing the selected major’s core subjects.</li>

</ol>

(by clicking the Intelligent System Major)

(by clicking the Machine Learning and Big Data Major)

<ol start="5">

 <li>Select elective subjects</li>

</ol>

The user shall able to select elective subjects from the list. The user can make multiple selection and the system shall automatically update the total enrolled credits. For example, the user can select the top three subjects from the elective subject list which make the total enrolled credits to 90 cp.




<ol start="6">

 <li>Enroll the student and create the enrolment record as a text file (“studentName_courseName.txt”)</li>

</ol>

The user can click the “Enrol” button anytime to complete the enrolment. By clicking the “Enrol” button, the system will do the following things automatically.

<ol>

 <li>The system will check whether the user’s personal information is provided and valid by using the exception handling (please see Lab 4’s solution). The student’s name must be a string, the student number must be an int. The DOB must be a string, use the format</li>

</ol>

“dd/mm/yyyy” and the date must exist. If any information is not provided or invalid, a popup window will alert the mistakes and ask the user to complete/correct the inputs.




(The exception for not inputting the student number)

(The exception for inputting a wrong student number)




(The exception for not inputting the DOB)




<ol>

 <li>The system will automatically check whether the user enrolls sufficient credits for the course. For BCS, the minimal requirement is 144 cp. For MCS, the minimal requirement is 96 cp. If not, the system will handle this as an exception and show a pop-up window to alert the user to enroll some extra subjects to reach the minimal requirement.</li>

</ol>

(The exception for not selecting sufficient subjects)

<ul>

 <li>When the user’s personal information is completed and valid and the user selects sufficient subjects (the user can enroll more subjects than the minimal requirement), the system will complete the course enrollment (with a pop-up window) and create a text file to keep the enrolment record. The text file’s name must be “studentName_courseName.txt”.</li>

</ul>

(The enrollment record is kept by a text file, named “studentName_courseName.txt”. The expected graduation date can be specified manually in the program.)

<ol start="7">

 <li>Reset the system</li>

</ol>

The user shall able to click the “Reset” button to reset all inputs, course structure, user’s selection and the total enrolled credit anytime.

(The reset button is clicked)

<strong> </strong>

Tasks

Task 1 : Update the UML class diagram by adding the SEFrame class. Complete the GUI design and implementation.

Task 2 : Implement the system according to the specified steps. The program shall

<ul>

 <li>be consistent with the UML class diagram;</li>

 <li>follow the conventions for naming all classes, variables, and methods;</li>

 <li>provide sufficient comments;</li>

 <li>use proper blank spaces, indentation and braces to make your code easy to read and understand;</li>

 <li>follow the steps specified above to enrol one student into either the Bachelor of Computer Science course or Master of Computer Science course;</li>

 <li>be able to load BCS or MCS course structure via Java ObjectInputStream;</li>

 <li>be able to response to user’s selection;</li>

 <li>be able to automatically update the enrolled total credits and calculate the remaining elective subject number for the minimal credit points requirement;</li>

 <li>be able to do the validation checking and handle the exceptions;</li>

 <li>be able to create a text file to keep the user’s enrolment record;</li>

 <li>be able to reset the system anytime.</li>

</ul>

Task 3: Compilation and test.

<ul>

 <li>You shall compile and test your program by using two different cases. The first testing case must enrol a student (bob) to the Bachelor of Computer Science course and the second testing case must enrol another student (Amy) to the Master of Computer Science course.</li>

 <li>You shall also test the exception handling of your program.</li>

 <li>Please carefully compile and test your program and make sure your program can pass the compilation by using “javac” command. Please do not define the package in your program (a special alert for students who use IDE to complete the assignment).</li>

</ul>