+++
date = '2024-11-19T01:06:26Z'
draft = false
title = 'Nested loops'
+++
# Nested loops and creating grids!

In this example, the outer loop handles the rows, and the inner loop controls the columns. For each row, the inner loop prints the cells, and after each row, a divider is printed to separate the grid.

Here’s a simple example in C++:

Here’s an example of a nested loop in C++ used to create a simple grid:



```cpp
---------------------------------------------------------
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
---------------------------------------------------------
```


## How It Works:
The outer loop (i) iterates over the rows.
The inner loop (j) iterates over the columns.
After each row, a divider is printed (except after the last row).
This approach can be easily adjusted for larger grids or different layouts.