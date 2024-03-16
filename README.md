# Leet-code

![LeetCode Logo](https://cdn-images-1.medium.com/max/1600/0*GePc7lo4CF4A3guP.png)
Welcome to my LeetCode solutions repository! Here, you'll find my Python3 solutions to various LeetCode problems.

## About

This repository serves as a collection of my solutions to LeetCode algorithmic challenges. As a passionate programmer, I enjoy tackling these problems and refining my problem-solving skills.

## Navigation

The repository is organized by problem topic, making it easy to find solutions to problems related to specific themes or algorithms. Each topic has its own folder containing the Python solution files.

## How to Use

To explore the solutions:

1. Browse through the folders categorized by problem topic.
2. Open the folder corresponding to the problem theme you're interested in.
3. Inside each folder, you'll find the Python solution files for related problems.

## Example Solution

Below is an example of one of my Python solutions:

### Problem: Contains Duplicate

```python
class Solution:
    def containsDuplicate(self, nums: List[int]) -> bool:
        # Create an empty set to store unique elements encountered so far 
        hashset = set()

        # Iteratate through the list of integers 
        for n in nums:
            # If the current integer is already in the set, it means it's a duplicate
            if n in hashset:
                return True
            # Otherwise, add the integer to the set                
            hashset.add(n)

        # If no duplicates are found after iteration through the entire list, return False
        return False
```

--- 

## Complexity Analysis
- Time Complexity: We iterate through the given list 'nums' once to check each element. Therefore, the time complexity is O(n).
- Space Complexity: We use a Hashset, 'hashset', to store duplicate elements. In the worst-case scenario, if there are no duplicate elements in the given list 'nums', the HashSet 'hashset' can store all elements of 'nums'. Therefore, the space complexity is O(n).
