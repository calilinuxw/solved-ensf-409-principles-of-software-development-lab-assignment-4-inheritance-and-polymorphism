Download Link: https://assignmentchef.com/product/solved-ensf-409-principles-of-software-development-lab-assignment-4-inheritance-and-polymorphism
<br>



<strong> </strong>

<strong>The objectives of this lab are to: </strong>

<ul>

 <li>understand the concept of class relationships, particularly inheritance.</li>

 <li>get familiarize with more details in a UML diagram, including syntax for attributes and operations.</li>

 <li>understand the concept of polymorphism</li>

 <li>implement classes in Java with the inheritance, association, aggregation, and composition relationships among them<strong> </strong></li>

</ul>

<strong> </strong>

<strong><u>The following rules apply to this lab and all other lab assignments in future:</u></strong>

<strong> </strong>

<ol>

 <li>Before submitting your lab reports, take a moment to make sure that you are handing in all the material that is required. If you forget to hand something in, that is your fault; you can’t use `I forgot’ as an excuse to hand in parts of the assignment late.</li>

 <li><strong><u>20% marks</u></strong> will be deducted from the assignments handed in up to <strong>24 hours</strong> after each due date. It means if your mark is X out of Y, you will only gain 0.8 times X. There will be no credit for assignments turned in later than 24 hours after the due dates; they will be returned unmarked. Exceptions can be made but the students must inform that Instructor beforehand to accommodate if acceptable</li>

</ol>

<h1>Exercise 1: Drawing a Class Diagram (10 Marks)</h1>

<strong> </strong>

<strong>Read This First – Generalization/specialization: </strong>During lectures, we learned that a relationship among classes can be mainly classified as <em>association</em>, <em>composition, aggregation</em>, and <em>inheritance</em>, and the focus of our previous lab was on the first three relationships. This lab focuses on <em>inheritance</em>.

<strong>What is Inheritance? </strong>

<strong> </strong>Inheritance is an important type of relationship between classes which is also referred to as a generalization/specialization relationship, or a “kind-of” relationship. An example for this type of relationship is the relationship between class Animal and class Cat. Where, Cat <u>is a</u> “kind of” animal. This type of relationship allows a class to be derived from an existing class. In other words, the derived class inherits all the properties (data fields), and behaviors (methods of its base class). UML uses the following notation (a line with a big triangular arrowhead, pointing from sub-class (child) to the super-class (parent), to demonstrate this type of relationship.

<strong><u>What to Do</u>: </strong>First, download 8 java files (Colour.java, Point2.java, Text.java,

Shape.java, Rectangle.java, Circle.java, Prism.java, and

Geometry.java) from D2L. Then, read the content of these files and try to reverse-engineer a class diagram that shows the relationship among these classes. You are expected to draw a detailed class diagram that not only shows the relationships among the classes (including multiplicities, etc.), but also the following two sets of information is required:

<ol>

 <li>Attributes of each class.</li>

 <li>Major operations in each class (constructor, getter, setter, and toString methods are not required)</li>

</ol>

<strong>What to hand in: </strong>submit your UML diagram as an image extension (i.e. .jpg, .jpeg, .png, …etc) or as a PDF in a folder with exercise number as a folder name

<strong>Note</strong>: <em>abstract methods are shown in italic in UML.</em>

Exercise 2: Shapes (10 Marks)

<strong>What to Do: </strong>First compile the java file you downloaded for exercise 1 and run the program. Your program should produce the following output:




<table width="568">

 <tbody>

  <tr>

   <td width="568">Shape name: R1Origin: X_coordinate: 3.0Y-coordinate: 4.0Black pointWidth: 6.0Length: 5.0 Shape name: C1Origin: X_coordinate: 13.0Y-coordinate: 14.0Green pointRadius: 15.0 Shape name: R2Origin: X_coordinate: 23.0Y-coordinate: 24.0Black pointWidth: 26.0Length: 25.0 Shape name: C2Origin: X_coordinate: 33.0Y-coordinate: 34.0Yellow pointRadius: 35.0 Shape name: P1Origin: X_coordinate: 43.0Y-coordinate: 44.0White pointWidth: 46.0Length: 45.0 height: 47.0 Shape name: P2Origin: X_coordinate: 53.0Y-coordinate: 54.0Gray pointWidth: 56.0 Length: 55.0 height: 57.0</td>

  </tr>

 </tbody>

</table>




Then, uncomment the last few lines of code in the Geometry.java file, under the line, which is labeled as “SECTION 2”. If you try to compile the program now it gives you a few compilation errors because methods: add, showAll, and calculator are missing. Your task in this exercise is to write the definition of the missing methods as follows:

<ul>

 <li>Method add: that adds objects of classes such as Rectangle, Circle and Prisms</li>

</ul>

to a TreeSet list, declared in class Geometry.

<ul>

 <li>Method showAll: that displays on the screen the information about those objects that are stored in the TreeSet</li>

 <li>Method calculator: that calculates and displays the area, perimeter, and volume of each object on the screen.</li>

</ul>




<strong><u>Hint:</u></strong> as we discussed in lectures, to make TreeSet list working, you also need to implement Comparable interface. By checking the link below, you should implement the compareto function to deliver the promised return values. <a href="https://docs.oracle.com/javase/8/docs/api/java/lang/Comparable.html">https://docs.oracle.com/javase/8/docs/api/java/lang/Comparable.html</a>

Although you will not be directly comparing objects in your program, a TreeSet needs the objects in its list to be comparable in order to sort them upon insertion. The comparison will be based on the shape name to sort them in lexicographical order.

If you add the definition of the above methods your program is expected to display the following outputs in addition to the previous outputs:

<table width="575">

 <tbody>

  <tr>

   <td width="575">Adding Rectangle, Circle, and Prism objects to the list…Showing information about objects added to the list:Shape name: C1Origin: X_coordinate: 13.0Y-coordinate: 14.0Green pointRadius: 15.0 Shape name: C2Origin: X_coordinate: 33.0Y-coordinate: 34.0Yellow pointRadius: 35.0 Shape name: P1Origin: X_coordinate: 43.0Y-coordinate: 44.0White pointWidth: 46.0 Length: 45.0 height: 47.0 Shape name: P2Origin: X_coordinate: 53.0Y-coordinate: 54.0Gray pointWidth: 56.0 Length: 55.0 height: 57.0 Shape name: R1Origin: X_coordinate: 3.0Y-coordinate: 4.0Black pointWidth: 6.0Length: 5.0</td>

  </tr>

 </tbody>

</table>




Shape name: R2

Origin: X_coordinate: 23.0

Y-coordinate: 24.0

Black point

Width: 26.0

Length: 25.0




Showing area, perimeter, and volume of objects in the list:

The area, perimeter, and volume of C1 are: 706.86, 94.25, 0.00.

The area, perimeter, and volume of C2 are: 3848.45, 219.91, 0.00.

The area, perimeter, and volume of P1 are: 12694.00, 182.00, 97290.00. The area, perimeter, and volume of P2 are: 18814.00, 222.00, 175560.00.

The area, perimeter, and volume of R1 are: 30.00, 22.00, 0.00.

The area, perimeter, and volume of R2 are: 650.00, 102.00, 0.00.

<strong>What to hand in: </strong>in a folder with the exercise number as name, include a screenshot of the program output and all source code files (including ones you did not modify).

Exercise 3: Tic-Tac-Toe Game with the Inheritance (20 marks + 5 Bonus marks)

<strong> </strong>

In this exercise, you are supposed to add a few classes to your Tic-Tac-Toe Game that you developed for Lab 2. To help you understand how to implement these classes the following class diagram, a sample run of the program, and a brief note about the responsibilities of each class are provided. Also, to reduce your workload the definition of class RandomGenerator and a modified version of class Game is available to download from D2L. You can make any changes to the code in these two files, or use a different way to solve this problem.

<strong>A Brief Description on Class </strong><strong>HumanPlayer</strong>: HumanPlayer is a sub-class of class Player. It is a concrete class and it has to define the abstract methods inherited from class Player. As the following sample run shows in this new version of the game the players should have the option of selecting the type of the players. In this example, Mike and Judy, the two players selected the first option (i.e. human player). Which in fact is identical to what the game was doing in lab 2.










<table width="559">

 <tbody>

  <tr>

   <td width="559">Please enter the name of the ‘X’ player: Mike What type of player is Mike?1: human2: Random Player3: Blocking Player4: Smart PlayerPlease enter a number in the range 1-4: 1 Please enter the name of the ‘O’ player: JudyWhat type of player is Judy?1: human2: Random Player3: Blocking Player4: Smart PlayerPlease enter a number in the range 1-4: 1 ……&lt;&lt;&lt; game is continued similar to lab 2&gt;&gt;&gt;</td>

  </tr>

 </tbody>

</table>

<strong>A Brief Description on Class </strong><strong>RandomPlayer</strong>: RandomPlayer is also a kind of Player. In fact, this is a computer-player that uses a random generator and picks a vacant spot on the board, randomly. The following example shows part of the game between a human (Mike) and his computer. As you can see in the sample run, Mike’s Computer plays randomly and places an O- mark in a randomly selected empty place immediately after Mike moves, and without any interaction for entering the row or the column number.







<table width="559">

 <tbody>

  <tr>

   <td width="559">Please enter the name of the ‘X’ player: Mike What type of player is Mike?1: human2: Random Player3: Blocking Player4: Smart PlayerPlease enter a number in the range 1-4: 1Please enter the name of the ‘O’ player: Mike’s ComputerWhat type of player is Mike’s Computer?1: human2: Random Player3: Blocking Player4: Smart PlayerPlease enter a number in the range 1-4: 2Referee started the game…|col 0|col 1|col 2+     +     +     +|   |      |      | row 0 |   |      |      |</td>

  </tr>

 </tbody>

</table>







<table width="559">

 <tbody>

  <tr>

   <td width="559">                |     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 1 |    |      |      ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 2 |    |      |      ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +Mike, what row should your next X be placed in?    1Mike, what column should your next X be placed in? 1 |col 0|col 1|col 2+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 0 |    |      |      ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 1 |    | X | ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 2 |    |      |      ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     + |col 0|col 1|col 2+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 0 |    |      |      ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 1 |    | X | ||     |     |     |+<span style="text-decoration: line-through;">     </span>+     +     +|    |      |      | row 2 |    |      | O ||     |     |     |+     +     +     +Mike, what row should your next X be placed in?    1Mike, what column should your next X be placed in? 0 …&lt;&lt;&lt; game is continued &gt;&gt;&gt;</td>

  </tr>

 </tbody>

</table>




<strong>Hint</strong>: You need to override the definition of method makeMove. Feel free to come up with your own algorithm, but here is a suggestion:




Call the method discrete from class RandomGenerator twice to return random values between 0 and 2 (if you have 3*3 board) for i and j, if the board[i][j] is available (i.e. empty), then mark it. If the cell is not available, repeat the procedure, until you find an empty spot.




Once your method makeMove is completely defined, test it by compiling and running your program a few times. Do not move to the next step until definition of the methods in this class is complete and error free.

<strong> </strong>of <strong>11 </strong>










<strong>A Brief Description on Class BlockingPlayer</strong>: A BlockingPlayer is kind of RandomPlayer that first looks at the board for a move that would block its opponent from winning on the next move. If it can’t find any such move, it picks a vacant spot at random. Therefore, before making any move, this class needs to call a method called testForBlocking. This method should return true if there is a situation that needs to be blocked. In other words, the process is to traverse through the board, and call testForBlocking method for each spot (i<sup>th</sup> row and j<sup>th</sup> column). If the function returns true for any of the i<sup>th</sup> row and j<sup>th</sup> column, put a mark in that spot, otherwise select an empty random spot (same as RandomPlayer).




<strong>Optional (Bonus) </strong><em>– </em>Implementation of class SmartPlayer is optional.




<strong>A Brief Description on Class </strong><strong>SmartPlayer: </strong>A SmartPlayer is a kind of BlockingPlayer, but slightly smarter and takes the following steps to move:




<ol>

 <li>First looks at board, if it can find a move to win immediately, it makes that move.</li>

 <li>Otherwise, it looks for a way to block its opponent’s from winning on the next move.</li>

 <li>Otherwise, it picks a vacant square at random.</li>

</ol>







<strong>What to hand in: </strong>in a folder with exercise number as folder name, include all source code files (including ones you did not modify), and a screenshot for output of each of the test cases when one of the players is human vs one of the two (three if you do the bonus) other player types. Also include a subfolder for the Javadoc generated for your code documentation.










<strong>How to submit: </strong>Include all your files for the lab in one folder, zip your folder and upload it in D2L before the deadline.







<strong> </strong>of <strong>11</strong>