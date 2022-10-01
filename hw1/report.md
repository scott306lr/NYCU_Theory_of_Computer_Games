# TCG HW1 Report

### Heuristic for Threes! :

The method is based on [*Composition of Basic Heuristics for the Game 2048*](https://theresamigler.files.wordpress.com/2020/03/2048.pdf), with some modifications to fit Threes!.

The heuristic first selects the steps that has the most empty tiles. If two moves have the same value, we then compare the one with higher monotonicity.

Below is the heuristic for measuring monotonicity in 2048:

<img src="/home/scott/coding/class_work/NYCU_Theory_of_Computer_Games/hw1/mono_pseudo.png" alt="mono_pseudo" style="zoom:100%;" /> 

By measuring using monotonicity, we can build up a board having the highest score, by arranging the tiles, so that they are all non-increasing or all non-decreasing along all rows and columns, and have the highest value being in one of the corners.  



<img src="/home/scott/coding/class_work/NYCU_Theory_of_Computer_Games/hw1/mono_example.png" alt="mono_example" style="zoom:60%;" /> 

However, in Threes!, which is different from 2048, 3s are merged by 1s and 2s. 

We view 1s and 2s as the same value, so the above figure shows an example with the highest monotonicity that can be made with the given tiles.

