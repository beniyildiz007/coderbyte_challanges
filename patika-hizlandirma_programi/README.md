# Kodluyoruz Hızlandırma Programı Coderbyte Challanges

## Hafta 3
### Soru 1
<p align="left">
  <img width="250" height="250" src="https://i.hizliresim.com/5a30crf.jpg">
</p>

V1:
```python
def StringChallenge(strParam):
  nums=[]
  control=0
  if strParam.count(" ")==0:
    listem=list(strParam)
    for i in range(0,len(listem)):
        if listem[i].isdigit():
            nums.append(listem[i])
    for i in listem:
        if i.isdigit():
            ilk=listem.index(i)
            break
    if listem[ilk].isdigit() == listem[ilk+1].isdigit() == listem[ilk+2].isdigit():
        control+=1
    for i in nums:
        if nums.count(i)>1:
            control+=1
  else:
    ayrac = strParam.split()
    for i in range(0,len(ayrac)):
        listem=list(ayrac[i])
        for j in range(0,len(listem)):
            if listem[j].isdigit():
                nums.append(listem[j])
        for x in listem:
            if x.isdigit():
                ilk=listem.index(x)
                break
        if listem[ilk].isdigit() == listem[ilk+1].isdigit() == listem[ilk+2].isdigit():
            control+=1
        for y in nums:
            if nums.count(y)>1:
                control+=1
        nums=[]
  if control==0:
    return "true"
  else:
    return "false"
# keep this function call here 
print(StringChallenge(input()))
```
V2:
```python
def StringChallenge(strParam):
	ayrac = strParam.split()
	for k in ayrac:
		nums = []
		control = 0
		for i in k:
			if i.isdigit():
				for j in nums:
					if j == i:
						return "false"
				nums.append(i)
				if len(nums) == 3:
					if control == 0:
						return "false"
					break
			elif len(nums) > 0:
				control = 1
	return "true"

print(StringChallenge(input()))
```
V3:
```python
def StringChallenge(strParam):
	ayrac = strParam.split()
	for j in range(0, len(ayrac)):
		nums = []
		listem = list(ayrac[j])
		for i in range(0, len(listem)):
			if listem[i].isdigit():
				nums.append(listem[i])
		ilk = listem.index(nums[0])
		if listem[ilk].isdigit() == listem[ilk+1].isdigit() == listem[ilk+2].isdigit():
			return "false"
		for i in nums:
			if nums.count(i) > 1:
				return "false"
	return "true"

print(StringChallenge(input()))
```
V4:
```python
def StringChallenge(strParam):
	ayrac = strParam.split()
	for k in ayrac:
		nums = []
		for i in range(len(k)):
			if k[i].isdigit():
				if nums.count(k[i]) == 1:
					return "false"
				if len(nums) == 2:
					if k[i].isdigit() == k[i-1].isdigit() == k[i-2].isdigit():
						return "false"
					break
				nums.append(k[i])
	return "true"

print(StringChallenge(input()))
```
V5:
```python
def StringChallenge(strParam):
	ayrac = strParam.split()
	for metin in ayrac:
		nums = []
		for i in range(10):
			if metin.count(str(i)) > 1:
				return "false"
			elif metin.count(str(i)) == 1:
				nums.append(metin.index(str(i)))
				if len(nums) == 3:
					if nums[0] in [nums[1] - 1, nums[1]  + 1, nums[2] - 1, nums[2]  + 1] and  nums[1] in [nums[0] - 1, nums[0]  + 1, nums[2] - 1, nums[2]  + 1] and nums[2] in [nums[1] - 1, nums[1]  + 1, nums[0] - 1, nums[0]  + 1]:
						return "false"
					break
	return "true"

print(StringChallenge(input()))
```
### Soru 2
<p align="left">
  <img width="250" height="250" src="https://i.hizliresim.com/4mfthf9.jpg">
</p>

```python
def MathChallenge(num1,num2):

  # code goes here
  ebob=1
  if num1 < num2:
    for i in range (1,(num1+1)):
      if num1%i==0 and num2%i==0:
        ebob=i
  else:
    for i in range (1,(num2+1)):
      if num2%i==0 and num1%i==0:
        ebob=i
  return ebob

# keep this function call here 
print(MathChallenge(input()))
```
### Soru 3
<p align="left">
  <img width="250" height="250" src="https://i.hizliresim.com/sn6j9d1.jpg">
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

