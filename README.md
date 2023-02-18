# Maze-Solver-and-Recursive-Problems

This project consists of five parts. For each
part you should write both a recursive function and an iterative function to solve the
problem (i.e., you’ll write a total of eight functions for this project). Each of the projects
is independent, and they’re all very short. 

Part 1: Write three functions to find the smallest element in a set. The first function,
minIt, should use a loop (i.e., be an iterative solution). The second function minRec1
should be a recursive function that uses a decomposition where the size of the smaller
problem is n-1 (where n is the size of the original problem). The third function,
minRec2 should be a recursive function that uses a decomposition where the size of the
smaller problem is n/2. Note that your recursive functions will not have any loops!

Part 2: Write two functions to calculate the square root of a number. The first function,
squareIt should be iterative and the second function squareRec should be recursive.
You’ll be using floating point numbers (type double) for this question, so it is impossible
to calculate the square root exactly. Instead you must calculate the square root accurate
to 15 (decimal) significant digits. Your functions will use three parameters. The first
parameter is the value for which you must calculate the square root. The other two
parameters are “guesses”. The first guess is guaranteed to be smaller than the actual
square root. The second guess is guaranteed to be larger than the actual square root.
These parameters should give you a big hint how to solve this problem.

Part 3: Write two functions to perform string comparison. Both functions must use only
recursion (no loops or global variables). In the first function, write the conventional
strcmp function, which compares characters using their ASCII values. The comparison is
case sensitive, and punctuation is significant. So, for example, “ zzz” is less than “aaa”
because the former string has a space in front (ASCII 32) which is less than the ASCII for
‘a’. Follow the conventions for strcmp, return -1 if the first string is less than the second,
return 0 if the strings are the same and return 1 if the first string is greater than the
second. Call your function strCompare (it’s already declared for you in the project file).
Once you’ve finished writing the traditional strcmp function (using only recursion!) write
a new version of the function that compares only the letters in the strings and ignores the
case (upper/lower case) of the letters. For this version, “ ZZZ” is greater than “aaa” since
the space is ignored and the capitalization is also ignored. Similarly, the two strings “C++
programming” and “c programming” are equal to each other. Name this function
strCompare2 (it’s also already declared for you in the project file).

Part 4: Write two functions to find the solution to a maze. The maze is represented by a
two-dimensional matrix. The syntax for accessing an element of the matrix is
maze[row][col] where row and col are the row number and column number for a
cell in the matrix. If the value of an element in the matrix is 1, then the corresponding
square in the matrix is a wall, and you cannot go into that square. If the value of the
element is 0, then you can go into the square. The entrance to the maze is a square in row
0 and the exit is a square in the last row (MATRIX_SIZE – 1). The maze is square with
MATRIX_SIZE rows and MATRIX_SIZE columns. The maze is generated with some special properties that make finding a solution
relatively easy. There is exactly one path between any two squares in the maze (except
walls of course, there are no paths that allow you to walk into a wall). To look at the
maze that’s generated, call the printMaze function and you’ll see what I mean. This
means that there are no loops or circular paths in the maze.

Part 5: Write a function that makes change. The input to the function is the amount of
money (cents). The return value from the function must be a struct where the components
indicate the number of coins which will add up to the amount of money. For this
problem, we’ll use a fictitious currency (Martian currency) which has 1-cent, 5-cent and
12-cent coins (pennies, nicks and dodeks). To receive credit, your function must use the
minimum number of coins possible. For example, if the input to the function were 15,
then you should return a Martian struct with the dodek and pennies components both set
to zero and the nicks component set to 3 (since three nicks is the most efficient way to
create 15 cents using martian currency). If the input were 17, then you should return a
Martian struct with pennies equal to zero, nicks equal to 1 and dodeks equal to 1.
The real version of this problem is one where the value of each of the coins is not known
in advance. i.e., you know there are three coins, and one of the coins (the penny) is worth
1 cent. However all you know about the other coins is that the nick is worth a cents, the
dodek is worth b cents, and 1 < a < b for some integers a and b. Clearly, if you can solve
this version of the problem, then you can solve the specific case where a = 5 and b = 12
(described above). Both versions of the problem are included in Project6.cpp for you to
complete.
