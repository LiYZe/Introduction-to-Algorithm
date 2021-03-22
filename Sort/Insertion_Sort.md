# Inertion Sort

## Pseudo-code

```bash
Inertion_sort(A[1...n]
  for j = 2 to n
    key  = A[j]
    //Inser A[j] int othe sorted sequence A[1..j-1]
    i = j-1
    while i > 0 and A[i] > key
      A[i+1] = A[i]
      i = i-1
    A[i+1] = key
```

## Analyse

### Worst case
input reverse sorted (Arithmetic series)
```bash
T(n) = θ(n^2)
```
