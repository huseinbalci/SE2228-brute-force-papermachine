A paper machine can produce an unlimited number of master (jumbo) rolls, each X(Example: 3000) mm wide.
The length of the items must be cut is given as an array.
Write a function to find the total wasted product by, using greedy approach.
** When the roll with excessive waste is discarded, a new one is placed.
Therefore, you have "unlimited number" of rolls with the same length (wide).

// Example
vector<int> lengths = {1380, 1930, 1520, 1880, 1560, 1710, 1220}
={1380, 1930, 1520, 1880, 1560, 1710, 1220}
int rollWidth = 3000
The function must return 3800.
                      Lengths                                  Pieces      Waste
1 - Iteration | {1380, 1930, 1520, 1880, 1560, 1710, 1220} |  1380,1520 | 100mm
2 - Iteration | {1930,1880, 1560, 1710, 1220}              |  1930      | 1070mm
3 - Iteration | {1880, 1560, 1710, 1220}                   |  1880      | 1120mm
4 - Iteration | {1560, 1710, 1220}                         |  1560,1220 | 220mm
5 - Iteration | {1710}                                     |  1710      | 1290mm
total_waste = 100+1070+1120+220+1290 = 3800mm
