Download Link: https://assignmentchef.com/product/solved-coms4701-homework4-csps
<br>
The objective of Sudoku is to ll a 9×9 grid with the numbers 1-9 so that each column, row, and 3×3 sub-grid (or box) contains one of each digit. You may try out the game here: <u>​</u><strong><u><a href="http://www.sudoku.com/">sudoku.com</a></u></strong><u>​</u><a href="http://www.sudoku.com/">.</a> Sudoku has 81 ​<strong>variables</strong>​, i.e. 81 tiles. The variables are named by ​<strong>row</strong>​ and ​<strong>column</strong>​, and are ​<strong>valued</strong>​ from 1 to 9 subject to the constraints that no two cells in the same row, column, or box may be the same.

Frame your problem in terms of ​<strong>variables</strong>​, ​<strong>domains</strong>​, and ​<strong>constraints. </strong>​We suggest representing a Sudoku board with a Python dictionary, where each key is a variable name based on location, and value of the tile placed there. Using variable names ​<strong>Al</strong>​… <strong>A9… I1… I9, </strong>​ ​ the board above has: –          <em>sudoku_dict</em>​[“​<strong>B1</strong>​”] = <strong>9</strong>​​, and  –      <em>sudoku_dict</em>​[“​<strong>E9</strong>​”] = ​<strong>8</strong>​.

We give value ​<strong>zero</strong>​ to a tile that has not yet been filled.

Your program will be executed as follows:

$ python driver_3.py &lt;input_string&gt;

In the starter zip, ​sudokus_start.txt​, contains hundreds of sample unsolved Sudoku boards, and sudokus_finish.txt​ the corresponding solutions. Each board is represented as a single line of text, starting from the top-left corner of the board, and listed left-to-right, top-to-bottom.

The first board in ​sudokus_start.txt​ is represented as the string:

003020600900305001001806400008102900700000008006708200002609500800203009005010300

Which is equivalent to:

0  0  3  0  2  0  6  0  0

9  0  0  3  0  5  0  0  1

0  0  1  8  0  6  4  0  0

0  0  8  1  0  2  9  0  0

7  0  0  0  0  0  0  0  8

0  0  6  7  0  8  2  0  0

0  0  2  6  0  9  5  0  0

8  0  0  2  0  3  0  0  9

0  0  5  0  1  0  3  0  0




Your program will generate ​output.txt, containing a single line of text representing the finished Sudoku​      board. E.g.:

483921657967345821251876493548132976729564138136798245372689514814253769695417382




Test your program using ​sudokus_finish.txt​, which contains the solved versions of all of the same puzzles.




<strong>Besides your driver (and any other python code dependency), submit a </strong>​<strong>README.txt</strong>​<strong> with your results and observations, including the: </strong>

<ul>

 <li><strong>number AND line numbers of boards you could solve from </strong><strong>txt</strong>​ <strong>,</strong>​</li>

 <li><strong>running time, and </strong></li>

 <li><strong>any other relevant information. </strong></li>

</ul>




<h1>III.   Backtracking Algorithm</h1>

Implement <strong>backtracking</strong>​ search using the ​ <strong>minimum remaining value</strong>​      ​ heuristic. Pick your own order of​             values to try for each variable, and apply ​<strong>forward checking</strong>​ ​to reduce variables domains.

<ul>

 <li>Test your program on ​txt​.</li>

 <li>Report the puzzles you can solve now, running time, observations.</li>

</ul>




<h1>IV.  Important Information</h1>

<ol>

 <li><strong>Test-Run Your Code </strong></li>

</ol>

Test, test, test. Make sure you produce an output file with the ​<strong>exact format </strong>​of the example given.

<ol start="3">

 <li><strong>Time Limit</strong></li>

</ol>

No brute-force! Your program should solve puzzles in ​<strong>well under a minute</strong>​ per board. Programs with much longer running times will be killed.

<ol start="4">

 <li><strong>Just for fun </strong></li>

</ol>

Try your code on the world’s hardest Sudokus! There’s nothing to submit here, just for fun. For example:




<strong>Sudoku: </strong>

800000000003600000070090200050007000000045700000100030001000068008500010090000400

<strong> </strong>

<strong>Solution: </strong>

812753649943682175675491283154237896369845721287169534521974368438526917796318452





