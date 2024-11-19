+++
date = '2024-11-19T01:06:26Z'
draft = false
title = 'Firstpost'
+++
# Nested loops and creating grids!

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