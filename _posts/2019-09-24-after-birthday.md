--
layout: post
title: "Super Martin Yang Site"
date: 2019-09-24
---

# Leetcode
Let's get started on leetcode. This blog is going to resolve all leetcode questions.

## Challenge 1. Two Sum (easy)
Given an array of integers, return indices of the two numbers such that they add up to a specific target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

Example:
```
Given nums = [2, 7, 11, 15], target = 9,

Because nums[0] + nums[1] = 2 + 7 = 9,
return [0, 1].
```

{% highlight python %}
class Solution:
    def twoSum(nums, target):
        dic = {}
        for idx, num in enumerate(nums):
            if target - num in dic:
                return [dic[target - num], idx]
            dic[num] = idx
{% endhighlight %}
