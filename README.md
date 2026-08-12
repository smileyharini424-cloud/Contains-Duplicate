# Contains Duplicate

## 1. Explanation

The **Contains Duplicate** problem checks whether an integer array contains any duplicate values.

The program returns `true` if at least one value appears more than once. If every value appears only once, it returns `false`.

The solution uses a `HashSet` to efficiently keep track of the elements that have already been visited.

---

## 2. Problem Statement

Given an integer array `nums`, return `true` if any value appears at least twice in the array. Otherwise, return `false`.

### Example

```text
Input:
nums = [1, 2, 3, 1]

Output:
true
```

The value `1` appears more than once, so the result is `true`.

---

## 3. Features

* Detects duplicate elements in an array.
* Uses Java `HashSet`.
* Traverses the array only once.
* Provides an efficient solution.
* Simple and easy-to-understand implementation.
* Includes a `main()` method for testing.

---

## 4. How It Works

The program creates a `HashSet` to store the elements that have already been encountered.

For every element in the array:

1. Check whether the element already exists in the `HashSet`.
2. If it exists, a duplicate has been found, so return `true`.
3. If it does not exist, add the element to the `HashSet`.
4. Continue until all elements are checked.
5. If no duplicate is found, return `false`.

---

## 5. Technologies Used

* Java
* HashSet
* Arrays
* For-each loop
* Conditional statements
* Methods
* Classes

---

## 6. Data Structure Used

### HashSet

The program uses:

```java
HashSet<Integer> set = new HashSet<>();
```

A `HashSet` stores unique elements and allows efficient checking to determine whether an element already exists.

---

## 7. Methods Used

### `containsDuplicate()`

```java
public static boolean containsDuplicate(int[] nums)
```

This method checks whether the given array contains duplicate elements.

**Parameter:**

* `nums` – Integer array to be checked.

**Return value:**

* `true` – If a duplicate is found.
* `false` – If no duplicate exists.

### `main()`

```java
public static void main(String[] args)
```

The `main()` method provides sample input, calls the `containsDuplicate()` method, and displays the result.

---

## 8. Program Flow

```text
Start
  ↓
Create integer array
  ↓
Create HashSet
  ↓
Read each element
  ↓
Is element already in HashSet?
  ↓
 ┌───────────────┐
 │               │
Yes              No
 │               │
 ↓               ↓
Return true      Add element
 │               │
 ↓               ↓
End          Continue loop
                 ↓
          All elements checked?
                 ↓
             Return false
                 ↓
                End
```

---

## 9. Sample Input

```text
nums = [1, 2, 3, 1]
```

## 10. Sample Output

```text
Contains Duplicate: true
```

---

## 11. Time Complexity

The array is traversed once, and `HashSet` provides average constant-time lookup.

```text
Time Complexity: O(n)
```

where `n` is the number of elements in the array.

---

## 12. Space Complexity

In the worst case, all elements are stored in the `HashSet`.

```text
Space Complexity: O(n)
```

---

## 13. Key Learning

This problem demonstrates how a `HashSet` can be used to efficiently detect duplicate values.

Instead of comparing every element with every other element using nested loops, the program stores previously encountered values and checks for duplicates while traversing the array.

This improves the time complexity from **O(n²)** to **O(n)**.

---

## 14. File Location

```text
Arrays/ContainsDuplicate.java
```

---

## 15. Repository Structure

```text
Contains-Duplicate/
│
├── README.md
│
└── Arrays/
    └── ContainsDuplicate.java
```

---

## 16. Author

**V.Harini**
