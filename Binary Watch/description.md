A binary watch has 4 LEDs on the top to represent the hours (0-11), and 6 LEDs on the bottom to represent the minutes (0-59). Each LED represents a zero or one, with the least significant bit on the right.



For example, the below binary watch reads ."4:51"

H 8 ***4*** 2 1

M ***32 16*** 8 4 ***2 1***



Given an integer which represents the number of LEDs that are currently on (ignoring the PM), return all possible times the watch could represent. You may return the answer in any order.



The hour must not contain a leading zero.



For example, is not valid. It should be ."01:00""1:00"

The minute must consist of two digits and may contain a leading zero.



For example, is not valid. It should be ."10:2""10:02"

&nbsp;



Example 1:



Input: turnedOn = 1

Output: \["0:01","0:02","0:04","0:08","0:16","0:32","1:00","2:00","4:00","8:00"]

Example 2:



Input: turnedOn = 9

Output: \[]

&nbsp;



Constraints:



0 <= turnedOn <= 10

