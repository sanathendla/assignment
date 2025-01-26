Implementation of Insertion Sort

This program showcases how the Insertion Sort algorithm works, taking as input random integer arrays to sort, as well as benchmarks execution time against various sizes for comparison.
How it Works

1. Insertion Sort Implementation:**
   This is achieved in the `insertion_sort` function through repeated iterations: the correct placement of every element relative to elements within the already sorted section of the array. Compare.
2. User Input:

- The user will define the number of elements.
   - Creates a random integer array between the range of -1000 to 1000.
3.Sorting Procedure:
  - Loop Explanation:
    - Loop through each of the elements of the array
      1. Take that current element to be the `key`.
2. Compare the `key` with elements to its left in the sorted portion of the array.
   3. Shift all elements larger than the `key` one position to the right.
   4. Place the `key` in its correct position.
- Repeat the process for all elements until the array is sorted.
   - Step-by-Step Iteration Example:

     - Original Array: `[102, -50, 23, 78, -15]`
     1. Iteration 1:
        - Key: `-50`
        - Compare with `102`. Shift `102` to the right.
- At index 0, put `-50`.
        - Post-iteration array: `[-50, 102, 23, 78, -15]`
     2. Iteration 2:
        - Key: `23`
        - Compare with `102`. Move `102` right.
- Put `23` at index 1.
        Array after pass: `[-50, 23, 102, 78, -15]
    3. Pass 3
        Key: `78`
        Compare with `102`. Shift `102` right end.
- Place `78` at index 2.
        - List after pass: `[-50, 23, 78, 102, -15]`
     4. Pass 4:
        - Key: `-15`
        - Compare with `102`, `78`, `23`, and `-50`. Shift all to the right.
- Place `-15` at index 1.
    Array after loop: `[-50, -15, 23, 78, 102]`
4. **Performance Benchmarking:**

   The execution time is recorded for arrays of different sizes ranging from 1 to the size defined by the user.
   A plot is created that shows the correlation between the array size and execution time.
---

## Code Features

- **Generation of Random Array:** 
  - Arrays will be generated filled with random integers in the range -1000 to 1000 for the sorting.
  - For the benchmarking case, integers go from -100 to 100 so that faster computations are realized for smaller arrays.
- **Performance Measurement:** 

  The program will be using Python's time module to get the time consumed by the Insertion Sort algorithm for different array sizes.
- **Visualization:**

- Plot of array size versus execution time is shown using `matplotlib`.
-----

## Example Output

### User Input:
```
Enter the size of array: 5
```
### Generated Output:

```
Original Array: [102, -50, 23, 78, -15]
Insertion Sort: [-50, -15, 23, 78, 102]
```
### Visualization:

The plot below displays the execution time in seconds against the array size. The performance of Insertion Sort for an array size of 12:
![image](https://github.com/user-attachments/assets/b181e225-d618-4ff7-b6d3-38b3246d982e)

Implementation of Selection Sort
This program demonstrates the functionality of the Selection Sort algorithm. It takes random integer arrays as input to sort and benchmarks its execution time against varying array sizes for comparison.

How it Works
Selection Sort Implementation:
The selection_sort function iterates through the array multiple times. In each iteration, it:

Finds the smallest (or largest, depending on sorting order) element from the unsorted portion of the array.
Swaps it with the first element in the unsorted portion, effectively "selecting" the smallest/largest element and moving it to its correct position.
User Input:

The user defines the number of elements in the array.
A random integer array is generated within the range of -1000 to 1000.
Sorting Procedure:

Loop Explanation:

The algorithm iterates over each element, keeping track of the unsorted portion of the array.
For each iteration:
Find the minimum value in the unsorted portion.
Swap it with the first element of the unsorted portion.
Mark the next element as the start of the new unsorted portion.
Step-by-Step Iteration Example:

Original Array: [102, -50, 23, 78, -15]
Iteration 1:
Find the smallest element in [102, -50, 23, 78, -15], which is -50.
Swap -50 with the first element (102).
Post-iteration array: [-50, 102, 23, 78, -15]
Iteration 2:
Find the smallest element in [102, 23, 78, -15], which is -15.
Swap -15 with 102.
Array after pass: [-50, -15, 23, 78, 102]
Iteration 3:
Find the smallest element in [23, 78, 102], which is 23.
No swap needed (already in the correct position).
Iteration 4:
Find the smallest element in [78, 102], which is 78.
No swap needed (already in the correct position).
Final sorted array: [-50, -15, 23, 78, 102]
Performance Benchmarking:

Execution time is recorded for arrays of various sizes ranging from 1 to the size defined by the user.
A plot is created to visualize the correlation between array size and execution time.


