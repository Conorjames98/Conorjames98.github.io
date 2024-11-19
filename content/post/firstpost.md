+++
date = '2024-11-19T01:06:26Z'
draft = false
title = 'Firstpost'
+++
# Nested loops and creating grids!

I've firstly initialised a grid that's 3x3 and then used a for loop for using initialising (i) as 0 then checking if (i) is less than the gridSize which is 3, the next for loop will be inside the initial for loop this is what we call a nested loop, these types of loops consist of outer loops & inner loops in my case (i) controls the rows and (j) controls the columns after this I use a conditional statement that controls the dividers between each column by using if (i) is less than the grid size minus 1 then to console out the dividers.

Here’s an example of a nested loop in C++ used to create a simple grid:

```cpp
#include <iostream>
using namespace std;

int main() {
    int gridSize = 3;
    // This is a nested loop
    // This is the outer loop
    for (int i = 0; i < gridSize; ++i) {
        // This is the inner loop
        for (int j = 0; j < gridSize; ++j) {
            cout << "  |";
        }
        cout << endl;
        if (i < gridSize - 1) {
            cout << "-----+-----" << endl;
        }
    }

    return 0;
}