# Longest Strictly Increasing or Strictly Decreasing Subarray

### Easy

## Problem

Problem List
Problem List

Debugging...

255:07:46

Alla_Venkata_Sri_KarthikeyaAccess all features with our Premium subscription!

My Lists

Favorites

Notebook

Progress

Points

Try New Features

Orders

My Playgrounds

Settings

Appearance

Appearance

System Default

Light

Dark

Sign Out

System Default

Light

Dark

Premium

Description
Description

Editorial
Editorial

Solutions
Solutions

Submissions
Submissions

Code
Code

Accepted
Accepted

Testcase
Testcase

Test Result
Test Result

Runtime
Memory
Notes

4
Accepted
a minute ago

C++

0 ms

27.7 MB

Notes

3
Accepted
14 hours ago

C++

0 ms

27.7 MB

Notes

2
Accepted
14 hours ago

C++

0 ms

27.9 MB

Notes

1
Wrong Answer
14 hours ago

C++

N/A

N/A

Notes

1

c

In the editor, Tab inserts indentation. Press Ctrl+M to toggle whether Tab moves focus out of the editor. Press Ctrl+' to run the code. Press Ctrl+Enter to submit.
Saved
Ln 1, Col 1

You must run your code first

All Submissions

Accepted868 / 868 testcases passed

Alla_Venkata_Sri_Karthikeya
submitted at Nov 13, 2026 06:04

Runtime

0ms
Beats100.00%

Memory

27.75MB
Beats74.37%

Code
C++

1class Solution {
2public:
3    int longestMonotonicSubarray(vector<int>& nums) {
4        int b=0,s=0,b1=1,s1=1;
5        for(int i=1;i<nums.size();i++)
6        {
7            if(nums[i]>nums[i-1])
8            {
9                s1++;
10                if(b1>b)
11                {
12                    b=b1;
13                }
14                b1=1;
15            }
16            else if(nums[i]<nums[i-1])
17            {
18                b1++;
19                if(s1>s)
20                {
21                    s=s1;
22                }
23                s1=1;
24            }
25            else
26            {
27                if(b1>b)
28                {
29                    b=b1;
30                }
31                if(s1>s)
32                {
33                    s=s1;
34                }
35                b1=s1=1;
36            }
37        }
38        if(b1>b)
39        {
40            b=b1;
41        }
42        if(s1>s)
43        {
44            s=s1;
45        }
46        return (b>s)?b:s;
47    }
48};

View more

0/5

FindHeaderBarSize
FindTabBarSize
FindBorderBarSize

## Problem Link

[Longest Strictly Increasing or Strictly Decreasing Subarray](https://leetcode.com/problems/longest-strictly-increasing-or-strictly-decreasing-subarray/)
