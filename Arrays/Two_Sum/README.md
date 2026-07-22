# 001. Two Sum

## Problem

Given an array of integers `nums` and an integer `target`, return the indices of the two numbers such that they add up to the target.

**LeetCode:** https://leetcode.com/problems/two-sum/

**Difficulty:** Easy

---

## Example

**Input**

```text
nums = [2,7,11,15]
target = 9
```

**Output**

```text
[0,1]
```

Explanation:

```
nums[0] + nums[1] = 2 + 7 = 9
```

---

# Approach 1: Brute Force

### Idea

Check every possible pair of elements.
If their sum equals the target, return their indices.

### Time Complexity

```
O(n²)
```

### Space Complexity

```
O(1)
```

### File

```
brute_force.py
```

---

# Approach 2: Hash Map

### Idea

Store previously visited numbers in a dictionary.

For every element:

- Find `target - current_number`
- If it already exists in the dictionary, return the answer.
- Otherwise store the current number.

### Time Complexity

```
O(n)
```

### Space Complexity

```
O(n)
```

### File

```
hashmap.py
```

---

# What I Learned

- Brute Force is easy to understand but inefficient.
- Dictionaries (Hash Maps) provide O(1) average lookup time.

