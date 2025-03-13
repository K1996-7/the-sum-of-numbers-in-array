# the-sum-of-numbers-in-array


## student information
Name:kidist abebe
ID:RNS-9562/23
course title: DSA
## algorism 
1. Input Phase:

   1. Prompt the user to enter the number of elements (n).

   2. If n is less than or equal to 0, display an error message and terminate the program.

   3. Initialize an empty list (or vector) to store the integers.

   4. For each element from 1 to n:

      • Prompt the user to enter an integer.

      • Store the integer in the list.

2. Choice Phase:

   1. Prompt the user to choose whether they want to find the second largest or third largest unique number.

   2. Read the user's choice.

3. Finding Second Largest:

   1. Initialize two variables: first and second to the minimum possible integer value (using numeric_limits<int>::min()).

   2. For each number in the list:

      • If the number is greater than first, update second to be first, and then update first to be the current number.

      • Else if the number is greater than second and not equal to first, update second to be the current number.

   3. After processing all numbers, check if second is still equal to the minimum integer value:

      • If yes, return -1 (indicating that a second largest unique number doesn't exist).

      • Otherwise, return second.

4. Finding Third Largest:

   1. Initialize three variables: first, second, and third to the minimum possible integer value.

   2. For each number in the list:

      • If the number is greater than first, update third to be second, update second to be first, and then update first to be the current number.

      • Else if the number is greater than second and not equal to first, update third to be second, and then update second to be the current number.

      • Else if the number is greater than third, not equal to first, and not equal to second, update third to be the current number.

   3. After processing all numbers, check if third is still equal to the minimum integer value:

      • If yes, return -1 (indicating that a third largest unique number doesn't exist).

      • Otherwise, return third.

5. Output Phase:

   1. Based on the user's choice, print either the second or third largest unique number.

   2. If the result is -1, print "Not available"



