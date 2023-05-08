Download Link: https://assignmentchef.com/product/solved-prog1385-assignment-7-shape-operators
<br>
This set of assignments (A-04, A-07 and A-08) are meant to give you practice (once again) at developing class definitions from scratch – but in this second installment – you will be adding some overloaded operators to your existing classes.  The set of activities are broken down into a 3 stages.

<ul>

 <li>A-04 : Gets you to develop 3 classes (with inheritance and polymorphism) as well as a test harness</li>

 <li>A-07 : Gets you to use some operator overloading</li>

 <li>A-08 : Gets you to develop some template functions and exception handling</li>

</ul>




<h2>Commenting in Assign-04, Assign-07 and Assign-08</h2>

In order to give you practice creating and writing DOxygen style comments – I want you to comment these 3 assignments using DOxygen.  This means that all of your class header and method header comments must be written so that DOxygen can extract them and produce the set of online documentation.  As well, I want you to also have commented all of the different class’ datamembers and constant values (if any) to also be extracted by DOxygen.  You will want to revisit the DOxygen-Dog example from Module-06 to remind yourself how this is done.  One final DOxygen expectation … I want you to also have a main project page for the <strong>Shapes</strong> project.  You can place whatever you want on this main project page, but remember that the purpose of this page is to inform the reader about the project – what is the project all about? What is it modelling? Perhaps you could also tell the reader about what underlying OOP concepts and techniques are being used in the implementation?




<h2>STEP 1 – Connecting to your Source Repository and Extracting your Starting Point</h2>

<ol>

 <li>Since this exercise is based upon A-04 – all you need to do is to sign-out your existing Shape code from your repository

  <ol>

   <li>Create a directory on the local machine – e.g. C:SETRepo</li>

   <li>Connect to your repository in the cloud (remembering your repository’s URL and your login credentials) using the Tortoise SVN client and perform an SVN Checkout.  What you should notice is that you have signed out your DisneyCharacter solution as well as your Shapes solution.</li>

  </ol></li>

 <li>If you like you can erase the DisneyCharacter subdirectory as you won’t be modifying that source in this exercise</li>

 <li>Once you have the Shapes solution – you are ready to begin this exercise … so let’s get into the requirements …</li>

</ol>







<h2>STEP 2 – The Requirements and Programming</h2>




In this exercise, you will take your existing classes from A-04 and add to them :

<u>The Shape Class</u>

<ul>

 <li>No changes</li>

</ul>




<h3>The Circle Class</h3>

<ul>

 <li>Add the following methods to this class – you can add to the .H file – watch best practices !! o An overloaded + operation</li>

 <li>When adding one circle to another, the resultant circle will take on the colour of the left-hand operand (the LHS)</li>

 <li>The resultant radius is the sum of the left and right operand’s radii o An overloaded * operation</li>

 <li>When multiplying one circle with another, the resultant circle will take on the colour of the righthand operand (RHS)</li>

 <li>The resultant radius is the product of the left and right operand’s radii o An overloaded = operation o          An overloaded == operation</li>

 <li>Which will return that 2 circles are equal if the radius and colours match</li>

</ul>







<h3>The Square Class</h3>

<ul>

 <li>Add the following methods to this class – you can add to the .H file – watch best practices !! o An overloaded + operation</li>

 <li>When adding one square to another, the resultant square will take on the colour of the left-hand operand (the LHS)</li>

 <li>The resultant sideLength is the sum of the left and right operand’s sideLengths</li>

</ul>




<h1>Assign-07</h1>

<em>Shapes – Adding Operators </em>

o    An overloaded * operation

<ul>

 <li>When multiplying one square with another, the resultant square will take on the colour of the righthand operand (RHS)</li>

 <li>The resultant sideLength is the product of the left and right operand’s sideLengths o An overloaded = operation o An overloaded == operation</li>

 <li>Which will return that 2 squares are equal if the sideLengths and colours match</li>

</ul>




<h2>The myShape Main</h2>

<ul>

 <li>Modify your testHarness to create the following shapes o    you can simply instantiate the objects required – no need for user input …  o        Circle shape called “round1” with radius 5.5 cm and colour “red” o   Circle shape called “round2” with radius 10.5 cm and colour “blue” o                Circle shape called “playARound” – instantiated with the default constructor of the Circle class

  <ul>

   <li>Square shape called “square1” with sideLength of 5 cm and colour “orange” o Square shape called “square2” with sideLength of 12 cm and colour “purple”</li>

   <li>Square shaped called “playASquare” – instantiated with the default constructor of the Square class</li>

  </ul></li>

 <li>After creating these shapes, call the appropriate method to print out the specifics of each shape</li>

 <li>Then use your overloaded operators to o Add round2 to round1 and store it in playAround                  (i.e. round1 + round2)

  <ul>

   <li>You should end up with playARound being “red” with radius of 16.0 cm o Add square1 to square2 and store in playASquare (i.e. square2 + square1)</li>

   <li>You should end up with playASquare being “purple” with sideLength of 17 cm) o Print out the specifics of playARound and playASquare</li>

  </ul></li>

 <li>Multiply round1 by round2 and store in playARound             (i.e. round1 * round2)

  <ul>

   <li>You should end up with a playARound being “blue” with a radius of 57.75 cm o Multiply square2 by square1 and store in playASquare (i.e. square2 * square1)</li>

   <li>You should end up with a playASquare being “orange” with a sideLength of 60 cm o Print out the specifics of playARound and playASquare</li>

  </ul></li>

 <li>Assign round1 to playAround, and then test to see if they are equivalent

  <ul>

   <li>e. playRound = round1; followed by if(playAround == round1)</li>

   <li>If they are – then print “Hurray !!” to the screen</li>

   <li>If they are not equal – then print “Awww !!” to the screen</li>

  </ul></li>

</ul>




<h2>STEP 3 – Putting your Code back into the Repository</h2>

When you have made these changes to your class definitions and mainline – you can simply save your VS Solution and commit your files.

<ul>

 <li>Start by saving all files in solution and existing Visual Studio.</li>

 <li>In the previous exercise – you were reminded of repository best-practices o                Where each source file needs to be committed individually with its own custom / specific comment o           So locate all of your source files (.H files and .CPP files) and commit them one-by-one</li>

 <li>After committing the source files – you return to the C:SETRepo directory where you do a final commit on the Shapes folder to pick up any stray files that also need to be committed</li>

</ul>





