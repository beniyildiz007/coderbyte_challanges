# Kodluyoruz Hızlandırma Programı Coderbyte Challanges

## Hafta 3
### Soru 1
### Soru 2
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

