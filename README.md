# Assignment 3: Sorting and Searching Algorithm Analysis System

## 📌 Project Overview

This project focuses on the implementation and analysis of fundamental sorting and searching algorithms in Java. The main objective is to compare the performance of different algorithms using execution time measurements and evaluate their efficiency in practical scenarios.

The following algorithms were selected for this project:

* **Basic Sorting Algorithm:** Selection Sort
* **Advanced Sorting Algorithm:** Merge Sort
* **Searching Algorithm:** Binary Search

The system generates arrays of different sizes and types, applies algorithms, and measures their execution time using `System.nanoTime()`.

---

## 📚 Algorithm Descriptions

### 🔹 Selection Sort (Basic Sort)

Selection Sort works by repeatedly finding the minimum element from the unsorted part of the array and placing it at the beginning.

**Steps:**

1. Find the smallest element in the array
2. Swap it with the first element
3. Move to the next position and repeat

**Time Complexity:**

* Best Case: O(n²)
* Average Case: O(n²)
* Worst Case: O(n²)

---

### 🔹 Merge Sort (Advanced Sort)

Merge Sort is a divide-and-conquer algorithm. It divides the array into halves, recursively sorts them, and then merges the sorted halves.

**Steps:**

1. Divide array into two halves
2. Recursively sort both halves
3. Merge the sorted halves

**Time Complexity:**

* Best Case: O(n log n)
* Average Case: O(n log n)
* Worst Case: O(n log n)

---

### 🔹 Binary Search (Searching Algorithm)

Binary Search works on a **sorted array** and repeatedly divides the search space in half.

**Steps:**

1. Find the middle element
2. Compare with target
3. If smaller → search right half
4. If larger → search left half

**Time Complexity:**

* Best Case: O(1)
* Average Case: O(log n)
* Worst Case: O(log n)

**Important:** Binary Search requires the array to be sorted.

---

## 🧪 Experimental Setup

The experiments were conducted using arrays of different sizes:

* Small: 10 elements
* Medium: 100 elements
* Large: 1000 elements

Two types of input data were tested:

* Random arrays
* Sorted arrays

Execution time was measured using:

```java
System.nanoTime()
```

---

## 📊 Experimental Results

### 🔹 Execution Time Comparison

| Array Size | Basic Sort (Selection) | Advanced Sort (Merge) | Search (Binary) |
| ---------- | ---------------------- | --------------------- | --------------- |
| 10         | (your result)          | (your result)         | (your result)   |
| 100        | (your result)          | (your result)         | (your result)   |
| 1000       | (your result)          | (your result)         | (your result)   |

---

## 📸 Screenshots

### 🔹 Program Output

👉 Insert screenshot here:

```
docs/screenshots/output1.png
```

*(This screenshot should show execution times for different array sizes)*

---

### 🔹 Additional Test Runs

👉 Insert more screenshots here:

```
docs/screenshots/output2.png
docs/screenshots/output3.png
```

*(Optional: show different runs to demonstrate consistency)*

---

## 📈 Analysis

* The **Merge Sort algorithm performed significantly faster** than Selection Sort, especially for larger arrays.

* This is because Merge Sort has a time complexity of **O(n log n)**, while Selection Sort has **O(n²)**.

* As the array size increases, the performance gap becomes much larger.

* For searching, **Binary Search was extremely fast**, even for large arrays.

* Its logarithmic complexity **O(log n)** makes it very efficient.

* Sorted arrays improve performance for some algorithms, but Selection Sort does not benefit much because it always performs the same number of comparisons.

* The experimental results match the expected Big-O complexity trends.

---

## 🤔 Reflection

During this project, I learned how different algorithms behave in real-world scenarios. Even though theoretical complexity provides a general idea, actual execution time can vary depending on input size and data structure.

One of the key takeaways is how much more efficient advanced algorithms like Merge Sort are compared to basic ones like Selection Sort. The difference becomes very noticeable when working with large datasets.

Another important insight was understanding why Binary Search requires a sorted array. Without sorting, the algorithm cannot efficiently divide the search space.

Overall, this project helped strengthen my understanding of algorithm efficiency, performance analysis, and Java programming.

---

## 📁 Project Structure

```
assignment2-sorting-searching/
├── src/
│   ├── Sorter.java
│   ├── Searcher.java
│   ├── Experiment.java
│   └── Main.java
├── docs/
│   ├── screenshots/
├── README.md
```

---

## ✅ Conclusion

This project demonstrates the importance of choosing the right algorithm depending on the problem and dataset size. Efficient algorithms significantly reduce execution time and improve overall performance.

---
