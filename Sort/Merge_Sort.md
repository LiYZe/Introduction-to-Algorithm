
# Merge Sort
- [Step](#Step)
- [Pseudo-code](#Pseudo-code)
- [Analyse](#Analyse)
  - [Worst case (Based on Step)](#Worst-case)
    - [Conclusion](#Conclusion)
- [Code](#Code)
## Step
1.	If n=1, done  Θ（1）

2.	Recursively sort A[1…[n/2]] and A[[n/2]…n] 2*Θ（n/2）

3.	Merge 2 sorted lists Θ（n）
	
## Pseudo-code
```bash
Merge_sort(A[1...n],p,q,r)
//A is an array and p, q, and r are indices into the array, such that p <= q < r
// assumes that the subarrays A[p..q] and A[q+1..r] are in sorted order.
n1 = q-p+1
n2 = r-q
let L[1..n1+1] and R[1..n2+1] be new arrays
for i = 1 to n1
  L[i] = A[p+i-1]
for j = 1 to n2
  R[j] = A[q+j]
L[n1+1] = ∞
R[n2+1] = ∞
i = 1
j = 1
for k = p to r
  if L[i] <= R[j]
    A[k] = L[i]
    i = i+1
  else A[k] = R[j]
    j = j+1
```
## Analyse

### Worst case
	
Step 1:Θ(1)

Step 2:2*Θ(n/2)

Step 3:Θ(n)

Total: 
```bash
T(n) = Θ(1),     if n = 1
       2*Θ(n/2), if n > 1
```
#### Conclusion:
T(n) = Θ(nlgn)

## Code
```bash
```
