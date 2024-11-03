Interview Question - John Venn
Problem Statement: Write a program that accepts two sets of alpha-numeric characters and performs an efficient matching between them. Finally, display the results.

The intent of this challenge is to play with set theory. Avoid using pre-built framework functions that perform this work in a single line of code. Instead, illustrate how you would efficiently operate with two sets of data when trying to match values between them.

There are many ways to approach this algorithm, so be creative!

Input:
Two lines of input, each with a space-delimited series of values that represent the two sets. For example:

mathematica
Kodu kopyala
1 2 3 A B C
X 11 G M 2 9 3 C N R
Output:
The set of values that exist in both input sets, sorted alpha-numerically. For example:

mathematica

2 3 C
If no common values exist, output NULL.

Test Cases:
Test 1

Input:
1 2 3 A B C
X 11 G M 2 9 3 C N R
Expected Output:

2 3 C

If no common values exist, output NULL

Test 2
Input
Test 2
6 0 2 4 7 1 8 3 9 5
A1 3 G DOG 18 3 9 E BIRD ONE 5 U J X2
Output
Test 2 
3 5 9

Test 3
Input
Test 3 
1 2 3 4 5 6 7 8 9 0
A B C D E F G
Output
Test 3 
NULL

Process Of Coding :
When I first looked at the problem, I knew I needed to find common values between two sets of alpha-numeric characters. My approach began with understanding the requirements clearly. I had to read two lines of input and split them into two separate sets of values. This is essential because I want to compare these two sets.

Next, I thought about how to efficiently find the common values. Instead of using complex functions, I decided to create a dictionary for the first set. A dictionary is great because it allows for fast lookups. By adding each element of the first set into the dictionary, I could quickly check if each element of the second set exists in it.

After finding the common values, I realized that I needed to sort them. The challenge mentioned sorting alpha-numerically, so I created a sorting rule. I made sure that numbers come before letters. This way, if I have a number like ‘2’ and a letter like ‘C’, ‘2’ will appear first in the output.

Finally, I printed the results. If there were common values, I joined them into a string; if there were none, I simply printed "NULL." This solution feels efficient and straightforward, and I believe it effectively demonstrates the principles of set theory while also being creative in its approach.  
