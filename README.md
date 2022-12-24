
**Repository link**: https://github.com/nahid98/RushHour
------------
<br>

# Rush-hour
------------
<br>
<br>

<B>REQUIREMENTS</B>
1. Having Python 3.8 or above
2. Use this python as venv (interpretor)
3. Activate venv
4. Open the requirements.txt and install all of them in your project.

<br>

<h2>TO RUN THE PROGRAM</h2>

Simply run the main.py

<br>

<h2>ABOUT THIS PROGRAM</h2>
<br>
<br> 

We have 6x6 puzzles (can change the puzzle size by changing the <B>Width1</B> and <B>Width2</B> values in the code).
This puzzles represent a parking lot filled with cars and the goal is to move the Ambulance ( a car represented with "AA",
has a length of 2 and is horizontal) which is located at the 3rd row, to the exit position (row3 column6).
<br>
In this program, 3 different search algorithms UCS, GBFS, and A/A* & 4 different heuristics H1, H2, H3, and H4 are used to solve these puzzles.
<br>

<h3> About the puzzles</h3>

<br> 
Puzzles are saved in a text file in the form of a string (ex: BBIJ....IJCC..IAAMGDDK.MGH.KL.GHFFL.)
, where the alphabets represent the cars and the <b>" . "</b> represent an empty space.
<br>
If at the end of the puzzle string, the initial feul of a car is given, that value is used to initialize that car's feul level,
otherwise the car feul level is set to 100.
For example when given <span style="color:rgb(0,102,0)">BBB..MCCDD.MAAKL.MJ.KLEEJ.GG..JHHHII J0 B4 </span>, feul level of car <b>J</b> is set to <b>0</b>, feul level of car <b>B</b> is set to <b>4</b>, and other cars will have the initial feul level of 100.
<br>
Horizontal cars in this game can be moved up & down, while vertical cars can be moved left & right. Also, if a horizontal 
car is located at the exit position, it will be removed from the board.
<br>
<br>

<div>
  <span style="color:red"><B>Please Note:</B></span> <br> 
  The code is written to generate 50 random puzzles in the <B>PuzzleGenerator.py</B> and the generated puzzles are saved as <B>generatePuzzles.txt</B> under <u>input</u> folder. 
  

There is also <U>sample-input.txt</U> under input folder to test the program with.
To <span style="color:rgb(136,176,75)">generate outputs(Search files & Solution files)</span> for <B>generatePuzzles.txt</B>, that contains 50 random puzzles, "generatedPuzzles text file" is used as <B>default</B> in the class <u>main.py</u> & this text file is <B>created</B> by using the <span style="color: orange">creatPuzzles( puzzleNum, board_size)</span> function from the <B>PuzzleGenerator.py</B> file.

<br>

To use a different text file with different name to test this program, its just needed to save this file under **input folder** and change the <U>default</U> value in **main.py** to its corresponding name.

<br>

Finally to see the analysis table of this program on the puzzles, a text file, called <b>analysis.txt</b>, is generated to show the statistics of the algorithms' searches based on the 50 random puzzles.


---------------

<span style="color:rgb(146,106,166)"> Thank You! &#128578;</span>
  
</div>
