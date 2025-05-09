# 🧮 Two Sum (LeetCode #1)

- **Date Solved:** May 9, 2025  
- **Difficulty:** Easy  
- **Category:** Array / HashMap  
- **Link:** [https://leetcode.com/problems/two-sum](https://leetcode.com/problems/two-sum)

## ✅ My Solution (Python)
```python
def twoSum(nums, target):
    seen = {}
    for i, num in enumerate(nums):
        if target - num in seen:
            return [seen[target - num], i]
        seen[num] = i
```

## 💡 Key Insight
Used hashmap for O(n) solution. Avoided brute-force.

## ❌ Mistakes or Confusions
Initially used nested loops — too slow.

## 🔁 Follow-ups
Return all pairs

Variation: Return indices of last valid pair
