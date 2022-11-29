# Kodluyoruz Hızlandırma Programı Coderbyte Challanges

## Hafta 3
### Soru 1
<p align="left">
  <img width="250" height="250" src="https://imgyukle.com/f/2022/11/29/JHVV26.png">
</p>

```python

```
### Soru 2
<p align="left">
  <img width="250" height="250" src="https://imgyukle.com/f/2022/11/29/JHVV26.png">
</p>

```python
def MathChallenge(num1,num2):

  # code goes here
  ebob=1
  if num1 < num2:
    for i in range (1,(num1+1)):
      if num1%i==0 and num2%i==0:
        ebob=i
  if num2 < num1:
    for i in range (1,(num2+1)):
      if num2%i==0 and num1%i==0:
        ebob=i
  return ebob

# keep this function call here 
print MathChallenge(raw_input())
```
### Soru 3
<p align="left">
  <img width="250" height="250" src="https://imgyukle.com/f/2022/11/29/JHEcff.png">
</p>

```python
def ArrayChallenge(arr):

  # code goes here
  liste2 = arr[arr[0]:(len(arr))]
  for i in range (0,arr[0]):
    liste2.append(arr[i])
  for num in liste2:
    print(num, end="")

# keep this function call here 
ArrayChallenge(input())
```

