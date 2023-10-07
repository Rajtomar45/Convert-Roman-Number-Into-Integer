# Convert-Roman-Number-Into-Integer
Here's an explanation of how the program works:
The romanToInt method takes a Roman numeral string s as input.
It initializes two variables: ans to store the final integer result and num to store the integer value of the current Roman numeral character being processed. Both are initially set to 0.
The program starts a loop that iterates through the characters of the input string s from right to left (i.e., from the least significant Roman numeral character to the most significant).
Inside the loop, a switch statement is used to determine the integer value (num) corresponding to the current Roman numeral character. It uses the following mappings:
'I' -> 1
'V' -> 5
'X' -> 10
'L' -> 50
'C' -> 100
'D' -> 500
'M' -> 1000
After determining the integer value num for the current character, the program checks whether subtracting 4 times num from the current accumulated result ans would be a valid representation. If this is the case, it subtracts num from ans, which accounts for cases like 'IV' (4) or 'IX' (9), where a smaller Roman numeral character appears before a larger one, indicating subtraction.
If the condition in step 5 is not met, it simply adds the integer value num to the accumulated result ans.
The loop continues until all characters in the Roman numeral string have been processed.
Finally, the program prints the computed integer ans, which represents the conversion of the Roman numeral string to its corresponding integer value.
