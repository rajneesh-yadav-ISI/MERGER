# MERGER
IT WAS A QUESTION GIVEN IN THE ASSIGNMENT TEST FOR FIRST SEM IN INDIAN STATISTICAL INSTITUTE KOLKATA

Consider a tile game, say MERGER, in which an n ×n square grid is given with titles having numbers labeled (not necessarily) on them. The labeled numbers are mandatorily in the form of 2k (k = 1,...,16). The tiles on the grid can be pairwise merged. The allowed merging actions that can be applied on a pair of tiles are upward, downward, leftward and rightward movement of the tiles. The said actions force the labeled tiles to move toward one of the sides (as applicable) following the same order in which they appeared earlier. However, when a pair of tiles labeled with the same number touch (being neighbors), they merge into one with the added value labeled on the tile in the respective direction leaving the other one unlabeled. Merging of tiles can be done only in the direction the merging action has taken place. An instance of such actions is shown in Fig. 1. The purpose of this game is to obtain the maximum possible number on a tile by applying merging actions.


  |2 |  |  |  |          |8 |8 |  |16|          |  |  |  |32|
  |  |8 |  |  |    -->   |  |4 |  |  |    -->   |  |  |  |4 |
  |2 |4 |  |  |          |  |  |  |  |          |  |  |  |  |
  |4 |  |  |16|          |  |  |  |  |          |  |  |  |  |


Figure 1: The effect of an upward action followed by a rightward action that cause an upward movement of all the tiles and then rightward movement of all the tiles. (Upward) In the first column, when the pair of tiles labeled with 2 touch, they merge into one with 4 labeled on it.This further gets merged with the tile labeled with 4, finally merged into one with 8 labeled on it (Rightward) In the first row, when the pair of tiles labeled with 8 touch, they merge into one with 16 labeled on it. This further gets merged with the tile labeled with 16, finally merged into one with 32 labeled on it.


Write a program to take a dimension of the grid and the initial set of labeled tiles and calculate the maximum possible value that one can get on any arbitrary tile after any arbitrary sequence of merging actions. Note that there can be multiple possible sequence of actions behind the maximum value obtained.

# Input Format #
The first line of input(to be taken from the user) is the integer n denoting the dimension of the grid. This will be followed by the numbers on the tiles maintaining a row major traversal. A value ‘0’ is taken to reflect the empty tiles(with no number on them).

#  Output Format #
The output shows the sequence of actions(as applicable) taken followed by the maximum possible resultant value on a tile in successive lines. If there are multiple possible sets of actions that might lead to the maximum value, then printing anyone of those set of actions will suffice.


SampleInput1:
 3
-1 0  0
 0 2  0
16 0  8
SampleOutput1:
INVALID


SampleInput2:
 4
 12 0  0  0
 0  2  0  0
 2  0  0  0
 4  8  0 32
SampleOutput2:
INVALID

 
SampleInput3:
2
16 16
16 16
SampleOutput3:
Downward
Leftward
64


SampleInput4:
4
2  0  0  0
0  2  0  0
2  4  0  0
4  0  0  8 
SampleOutput4:
leftward
upward
rightward
upward
16


SampleInput5:
4
2  0  0  0
0  8  0  0 
2  4  0  0
4  0  0  16
SampleOutput5:
upward
rightward
32
