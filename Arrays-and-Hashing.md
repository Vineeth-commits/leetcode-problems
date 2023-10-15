# Array and Hashing
### Problem 1 - [Two Sum](https://leetcode.com/problems/two-sum/)
#### Approach
1. Bruteforce [Time Complexity O(n<sup>2</sup>)] - Construct a nested loop to traverse and find all the combinations possible in the elements of the array. Once the summation of two elements are equivalent to target, return their position.
2. HashTable [Time Complexity O(n)] - Store all the Value of the elements and their positions in the Hashtable as key and value respectively. Once stored make a variable to find the difference between the target and num in the array while traversing linearly through the array. The difference gives the possbile second element which is found in the HashTable. Add another condition to check if the Value(position) is not equal to the current search element (Avoid repeating the same element). Once the match is found return the positions. 

### Problem 2 - [Contains duplicate](https://leetcode.com/problems/contains-duplicate/)
#### Approach
1. HashSet 1 [Time Complexity O(n)] - Start to store all the elements of the array in a hashset. Hashset doesnt allow duplicate values to be stored. It replaces the old value instead. We then compare the length of the hashset to the array. If they are equal, they dont contain duplicates, else they do.
2. HashSet 2 [Time Complexity O(n)] - Start to store all the elements of the array in a hashset but add a condition to check if the value that is being added is present in the hashset or not. If present report duplicate, else continue adding.
