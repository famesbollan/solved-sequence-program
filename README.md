Download Link: https://assignmentchef.com/product/solved-sequence-program
<br>
The program explores the properties of the 3n + 1 sequence which has two very simple rules for generating its elements: starting with a positive number, if the current number n is odd, the next one is 3n + 1; if it is even, the next one is n/2. The number 1 is a special case. If the current number is 1, the sequence terminates and there is no next element. A few examples below with different starting values:

– start = 3: 3, 10, 5, 16, 8, 4, 2, 1 has 8 elements

– start = 4: 4, 2, 1 has 3 elements

-start = 1: 1 has 1 element

It is conjectured, but never proven, that the 3n+1 sequence always reaches 1 and terminates, regardless of its starting value. We can’t check infinitely many start values, but we can find quite a few.

The program asks the user to enter the start and the end of the range for start values to check. We will generate a sequence for each of the values in the given range. When (or if? &#x1f642; ) the program terminates, we will output the longest sequence we encountered and the number of elements it has.

Samples

Sample Run 1

Enter the min of the range for the sequence to start 1

Enter the max of the range for the sequence to start 5 The longest sequence with a start value in the range [1, 5] has 8 elements.

3, 10, 5, 16, 8, 4, 2, 1

We did not find a non terminating case.

Sample Run 2

Enter the min of the range for the sequence to start 10 Enter the max of the range for the sequence to start 100

The longest sequence with a start value in the range [10, 100] has 119 elements.

97, 292, 146, 73, 220, 110, 55, 166, 83, 250, 125, 376, 188, 94, 47, 142, 71, 214, 107, 322, 161, 484, 242, 121, 364, 182, 91, 274, 137, 412, 206, 103, 310, 155, 466, 233, 700, 350, 175, 526, 263, 790, 395, 1186, 593, 1780, 890, 445, 1336, 668, 334, 167, 502, 251, 754, 377, 1132, 566, 283, 850, 425, 1276, 638, 319, 958, 479, 1438, 719, 2158, 1079, 3238, 1619, 4858, 2429, 7288, 3644, 1822, 911, 2734, 1367, 4102, 2051, 6154, 3077, 9232, 4616, 2308, 1154, 577, 1732, 866, 433, 1300, 650, 325, 976, 488, 244, 122, 61, 184, 92, 46, 23, 70, 35, 106, 53, 160, 80, 40, 20, 10, 5, 16, 8, 4, 2, 1

We did not find a non terminating case.

You will decompose the program into the 4 functions

getUserInput – takes two parameters start and end and asks the user to enter the min and max of the

range to check. It sets start to min and end to max. The function returns nothing.

getNextElement – takes a value and returns the next value in the sequence according to the rules. 1

shall return 1.

generateSequence – takes a start value for the sequence and a sequence string. It returns the length of

the generated sequence starting with that start value and the sequence string is set to the generated

sequence.

longestSequence – takes a start and an end value specifying the range of start values to check and a

sequence string. It returns the length of the longest sequence encountered with a start value in the range

[start, end] and the sequence string is set to the longest sequence encountered.