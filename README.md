# binary-search Implementation of binary search algorithm!!

 We will prove that binary search is faster than naive search!

Binary Search is a searching algorithm used in a sorted array by repeatedly dividing the search interval in half. The idea of binary search is to use the information that the array is sorted and reduce the time complexity to O(Log n). 

Binary Search Algorithm: The basic steps to perform Binary Search are:

Begin with the mid element of the whole array as a search key.
If the value of the search key is equal to the item then return an index of the search key.
Or if the value of the search key is less than the item in the middle of the interval, narrow the interval to the lower half.
Otherwise, narrow it to the upper half.
Repeatedly check from the second point until the value is found or the interval is empty.
Binary Search Algorithm can be implemented in the following two ways

Iterative Method
Recursive Method

naive search
Naïve pattern searching is the simplest method among other pattern searching algorithms. It checks for all character of the main string to the pattern. This algorithm is helpful for smaller texts. It does not need any pre-processing phases. We can find substring by checking once for the string. It also does not occupy extra space to perform the operation.

The time complexity of Naïve Pattern Search method is O(m*n). The m is the size of pattern and n is the size of the main string.

Input and Output
Input:
Main String: “ABAAABCDBBABCDDEBCABC”, pattern: “ABC”
Output:
Pattern found at position: 4
Pattern found at position: 10
Pattern found at position: 18
Algorithm
naivePatternSearch(pattern, text)
Input − The text and the pattern

Output − location, where patterns are present in the text

Begin
   patLen := pattern Size
   strLen := string size

   for i := 0 to (strLen - patLen), do
      for j := 0 to patLen, do
         if text[i+j] ≠ pattern[j], then
            break the loop
      done

      if j == patLen, then
         display the position i, as there pattern found
   done
End

