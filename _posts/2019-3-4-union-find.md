---
layout: post
title: Union Find algorithm
---

### Union Find 


#### Find
```python
def find(ar, i):
    if ar[i] != i:
        ar[i] = ar[ar[i]]
    return ar[i]
```

#### Union
```python
def union(ar, i, j):
    pi, pj = find(ar, i), find(ar, j)
    if pi != pj:
        ar[pi] = pj
```

#### Check if connected
```python
def connected(ar, i, j):
    return find(ar, i) == find(ar, j)
```

#### Full code with unit test
{% gist 635dc9371370ce9b21f101fbfca680bb %}
