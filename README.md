# MERGER
IT WAS A QUESTION GIVEN IN THE ASSIGNMENT TEST FOR FIRST SEM IN INDIAN STATISTICAL INSTITUTE KOLKATA

Consider a tile game, say MERGER, in which an n ×n square grid is given with titles having numbers labeled (not necessarily) on them. The labeled numbers are mandatorily in the form of 2k (k = 1,...,16). The tiles on the grid can be pairwise merged. The allowed merging actions that can be applied on a pair of tiles are upward, downward, leftward and rightward movement of the tiles. The said actions force the labeled tiles to move toward one of the sides (as applicable) following the same order in which they appeared earlier. However, when a pair of tiles labeled with the same number touch (being neighbors), they merge into one with the added value labeled on the tile in the respective direction leaving the other one unlabeled. Merging of tiles can be done only in the direction the merging action has taken place. An instance of such actions is shown in Fig. 1. The purpose of this game is to obtain the maximum possible number on a tile by applying merging action

  ![image](https://github.com/user-attachments/assets/067cc57a-416f-45be-a47b-f7104e97ced8)



Figure 1: The effect of an upward action followed by a rightwas.rd action that cause an upward movement of all the tiles and then rightward movement of all the tiles. (Upward) In the first column, when the pair of tiles labeled with 2 touch, they merge into one with 4 labeled on it.This further gets merged with the tile labeled with 4, finally merged into one with 8 labeled on it (Rightward) In the first row, when the pair of tiles labeled with 8 touch, they merge into one with 16 labeled on it. This further gets merged with the tile labeled with 16, finally merged into one with 32 labeled on it.


Write a program to take a dimension of the grid and the initial set of labeled tiles and calculate the maximum possible value that one can get on any arbitrary tile after any arbitrary sequence of merging actions. Note that there can be multiple possible sequence of actions behind the maximum value obtained.

# Input Format #
The first line of input(to be taken from the user) is the integer n denoting the dimension of the grid. This will be followed by the numbers on the tiles maintaining a row major traversal. A value ‘0’ is taken to reflect the empty tiles(with no number on them).

#  Output Format #
The output shows the sequence of actions(as applicable) taken followed by the maximum possible resultant value on a tile in successive lines. If there are multiple possible sets of actions that might lead to the maximum value, then printing anyone of those set of actions will suffice.


#SampleInput1:
![image](https://github.com/user-attachments/assets/b541d356-94b4-4390-ab38-44385961a71b)

#SampleOutput1:
![image](https://github.com/user-attachments/assets/1e709742-2e4f-46c0-bea5-9069f9c97592)



#SampleInput2:
![image](https://github.com/user-attachments/assets/abc68d65-f803-4ecf-aea0-a44fd7afc859)

#SampleOutput2:
![image](https://github.com/user-attachments/assets/1e709742-2e4f-46c0-bea5-9069f9c97592)

 
#SampleInput3:
![image](https://github.com/user-attachments/assets/a82d936d-0f32-40f8-b823-6c9179906f10)

#SampleOutput3:
![image](https://github.com/user-attachments/assets/1f20bf64-2235-44a2-b21a-1542e5eb6a87)



#SampleInput4:
![image](https://github.com/user-attachments/assets/e1a08ad3-0248-4bfc-803e-2e8ecedcc7c8)

#SampleOutput4:
![image](https://github.com/user-attachments/assets/c293b52a-486b-4f3e-8da8-9a96b329a439)


#SampleInput5:
![image](https://github.com/user-attachments/assets/e374bd43-d18a-4a1a-870e-7908aff469a9)

#SampleOutput5:
![image](https://github.com/user-attachments/assets/4db625f8-b276-419b-8391-e61e6d74cf71)

