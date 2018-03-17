---
title: "A post with some code"
date: 2018-03-17T10:47:12Z
draft: false
---

In Python (Python 3), here's one way to get a list of non-zero integers that
are less than $N$, e.g. $N=50$, and that are multiples of $k$, e.g. $k=3$:

<!--more-->
``` python
N = 50
k = 3
[n for n in range(1, N) if n % k == 0]
```

Here is how you would do the same thing in R:
``` r
N <- 50
k <- 3
Filter(function(x) x %% k == 0, seq(N-1))
```

