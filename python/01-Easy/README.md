# GCF Challenge
![Python](https://i.hizliresim.com/i1f8d09.jpg)
```python
"""
Have the function GCF(arr) take the array of numbers stored in arr which will always
contain only two positive integers, and return the greatest common factor of them.
For example: if arr is [45, 12] then your program should return 3.
There will always be two elements in the array and they will be positive integers.

Input: [1, 6] Output: 1
Input: [12, 28] Output: 4
1. For input [45, 12] the output was incorrect. The correct output is 3

2. For input [1, 6] the output was incorrect. The correct output is 1

3. For input [12, 28] the output was incorrect. The correct output is 4

4. For input [106, 212] the output was incorrect. The correct output is 106

5. For input [12, 12] the output was incorrect. The correct output is 12

6. For input [12, 11] the output was incorrect. The correct output is 1

7. For input [6, 167] the output was incorrect. The correct output is 1

8. For input [2345, 2562] the output was incorrect. The correct output is 7

9. For input [24, 92] the output was incorrect. The correct output is 4

10. For input [10, 100] the output was incorrect. The correct output is 10

"""


#10/10
def GCF(arr):
  for i in reversed(range(min(arr)+1)):
    if arr[0]%i == 0 and arr[1]%i == 0:
      return i

# keep this function call here 
print(GCF(input()))


```
