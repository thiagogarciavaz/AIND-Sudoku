# Artificial Intelligence Nanodegree
## Introductory Project: Diagonal Sudoku Solver

# Question 1 (Naked Twins)
Q: How do we use constraint propagation to solve the naked twins problem?  
A: I created a constraint that in a square, when two boxes have the same 2-value "probability", no other box can assume these 2 values.
So, we can eliminate when it appear in a square. And we can keep applying multiple times to reinforce this constraint and achieve better results, propagating that rule.
# Question 2 (Diagonal Sudoku)
Q: How do we use constraint propagation to solve the diagonal sudoku problem?  
A: The original Sudoku has three constraints: no repeated values (1-9) over rows, columns and squares.
So, the idea when I programmed the Diagonal Sudoku was to include one more constraint in the model, controlling rows, columns, squares and diagonals.
As the 'eliminate' function already used a 'peer' control, it automatically included diagonals in the function, too.
And, as in the naked twins, we can iterate multiple times (using search or eliminate) to take advantage of this restriction and find a better solution.

### Install

This project requires **Python 3**.

We recommend students install [Anaconda](https://www.continuum.io/downloads), a pre-packaged Python distribution that contains all of the necessary libraries and software for this project. 
Please try using the environment we provided in the Anaconda lesson of the Nanodegree.

##### Optional: Pygame

Optionally, you can also install pygame if you want to see your visualization. If you've followed our instructions for setting up our conda environment, you should be all set.

If not, please see how to download pygame [here](http://www.pygame.org/download.shtml).

### Code

* `solutions.py` - You'll fill this in as part of your solution.
* `solution_test.py` - Do not modify this. You can test your solution by running `python solution_test.py`.
* `PySudoku.py` - Do not modify this. This is code for visualizing your solution.
* `visualize.py` - Do not modify this. This is code for visualizing your solution.

### Visualizing

To visualize your solution, please only assign values to the values_dict using the ```assign_values``` function provided in solution.py

### Data

The data consists of a text file of diagonal sudokus for you to solve."# aind-sudoku" 
