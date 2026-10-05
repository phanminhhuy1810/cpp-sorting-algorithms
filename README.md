# C++ Sorting and Array Algorithms

My first GitHub project: a small C++ learning exercise with 11 sorting and array algorithm demonstrations. The program runs each example on fixed data and prints intermediate steps and results.

## Algorithms

| Algorithm | Purpose | Time complexity |
| --- | --- | --- |
| Bubble sort | Sort integers in ascending order | O(n²) in all cases for this implementation |
| Selection sort | Sort integers in ascending order | O(n²) in all cases |
| Insertion sort | Sort integers in ascending order | O(n) best; O(n²) average and worst |
| Quick sort | Sort integers using the last element as the pivot | O(n log n) average; O(n²) worst |
| Merge sort | Sort integers by merging sorted halves | O(n log n) |
| Counting sort | Sort integers using counts over the value range | O(n + r) |
| Quickselect | Find the k-th largest element | O(n) average; O(n²) worst |
| Min-heap selection | Keep the k largest values in a min-heap to find the requested rank | O(n log(k + 1)) |
| Merge-based inversion count | Count pairs where an earlier element is larger than a later one | O(n log n) |
| Odd-before-even partition | Group odd values before even values, preserving order within each group | O(n) |
| Multi-criteria sort | Sort students by grade ascending, score descending, then name ascending | O(n log n) comparisons |

Here, `n` is the number of elements, `r` is `max − min + 1`, and `k` is the requested rank. These bounds describe the algorithm work and exclude console output; printing intermediate arrays adds overhead. The average bounds for quick sort and Quickselect depend on the input order because both use a fixed pivot.

## Build and run

Use a C++17 compiler. From the repository root:

```sh
g++ -std=c++17 -Wall -Wextra sort.cpp -o sorting_demo
./sorting_demo
```

The program takes no interactive input. To try different examples, edit `data`, `K`, or the student records in `sort.cpp` and rebuild. The current array example uses nine integers and finds the third-largest value. Console explanations are in Vietnamese.

This is a collection of demonstrations rather than a general-purpose sorting library. The selection examples assume `1 <= k <= n`, and counting sort assumes a nonempty array with a manageable value range.
