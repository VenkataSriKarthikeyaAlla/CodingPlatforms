# Can Place Flowers

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

Accepted
Accepted

Editorial
Editorial

Solutions
Solutions

Submissions
Submissions

Code
Code

Testcase
Testcase

Test Result
Test Result

All Submissions

Accepted130 / 130 testcases passed

Alla_Venkata_Sri_Karthikeya
submitted at Nov 01, 2026 08:23

Runtime

0ms
Beats100.00%

Memory

23.94MB
Beats94.78%

Code
C++

1class Solution {
2public:
3    bool canPlaceFlowers(vector<int>& flowerbed, int n) {
4      int c=0;
5      for(int i=0;i<flowerbed.size();i++)
6      {
7        if(flowerbed[i]==0&&(i-1<0||flowerbed[i-1]==0)&&(i+1>=flowerbed.size()||flowerbed[i+1]==0))
8        {
9            c++;
10            flowerbed[i]=1;
11        }
12      }
13      if(c>=n)
14      {
15        return true;
16      }
17      return false;
18    }
19};

View more

0/5

Runtime
Memory
Notes

1
Accepted
a few seconds ago

C++

0 ms

23.9 MB

Notes

1

2

3

4

5

6

7

8

9

10

11

12

13

14

15

16

17

class Solution {
public:
bool canPlaceFlowers(vector<int>& flowerbed, int n) {
int c=0;
for(int i=0;i<flowerbed.size();i++)
{
if(flowerbed[i]==0&&(i-1<0||flowerbed[i-1]==0)&&(i+1>=flowerbed.size()||flowerbed[i+1]==0))
{
c++;
flowerbed[i]=1;
}
}
if(c>=n)
{
return true;
}
return false;

In the editor, Tab inserts indentation. Press Ctrl+M to toggle whether Tab moves focus out of the editor. Press Ctrl+' to run the code. Press Ctrl+Enter to submit.
Saved
Ln 1, Col 1

You must run your code first

FindHeaderBarSize
FindTabBarSize
FindBorderBarSize

## Problem Link

[Can Place Flowers](https://leetcode.com/problems/can-place-flowers/)
