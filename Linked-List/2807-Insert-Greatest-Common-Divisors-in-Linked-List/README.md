# Insert Greatest Common Divisors in Linked List

### Medium

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

Accepted582 / 582 testcases passed

Alla_Venkata_Sri_Karthikeya
submitted at Nov 13, 2026 06:04

Runtime

3ms
Beats80.02%

Memory

35.74MB
Beats97.94%

Code
C++

1/**
2 * Definition for singly-linked list.
3 * struct ListNode {
4 *     int val;
5 *     ListNode *next;
6 *     ListNode() : val(0), next(nullptr) {}
7 *     ListNode(int x) : val(x), next(nullptr) {}
8 *     ListNode(int x, ListNode *next) : val(x), next(next) {}
9 * };
10 */
11class Solution {
12public:
13    ListNode* insertGreatestCommonDivisors(ListNode* head) {
14        ListNode * temp=head;
15        while(temp->next!=NULL)
16        {
17            ListNode*ne=temp->next;
18            int gc=gcd(temp->val,ne->val);
19            ListNode *newnode=new ListNode(gc);
20            newnode->next=ne;
21            temp->next=newnode;
22            temp=ne;
23        }
24        return head;
25    }
26};

View more

0/5

Runtime
Memory
Notes

2
Accepted
a minute ago

C++

3 ms

35.7 MB

Notes

1
Accepted
23 minutes ago

C++

7 ms

35.9 MB

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

/**
* Definition for singly-linked list.
* struct ListNode {
*     int val;
*     ListNode *next;
*     ListNode() : val(0), next(nullptr) {}
*     ListNode(int x) : val(x), next(nullptr) {}
*     ListNode(int x, ListNode *next) : val(x), next(next) {}
* };
*/
class Solution {

In the editor, Tab inserts indentation. Press Ctrl+M to toggle whether Tab moves focus out of the editor. Press Ctrl+' to run the code. Press Ctrl+Enter to submit.
Saved
Ln 1, Col 1

You must run your code first

FindHeaderBarSize
FindTabBarSize
FindBorderBarSize

## Problem Link

[Insert Greatest Common Divisors in Linked List](https://leetcode.com/problems/insert-greatest-common-divisors-in-linked-list/)
