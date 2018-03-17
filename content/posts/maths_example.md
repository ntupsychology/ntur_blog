---
title: "A post with some maths"
date: 2018-03-16T20:12:57Z
draft: true
author: Mark Andrews
---

In this post, we explain the difference between binary and binomial logistic regression.


If we have $N$ data points $(y_1, x_1), (y_2, x_2) \ldots (y_i, x_i) \ldots (y_N, x_N)$, where for each $i$, $y_i \in \{0, 1\}$, we can model this data as 
$$
y_i \sim \mathrm{bernoulli}(p_i),\quad \log\large\left(\frac{p_i}{1-p_i}\right) = \alpha + \beta x_i.
$$
This is binary logistic regression.

<!--more-->

On the other hand, if we have $N$ data points $(n_1, m_1, x_1), (n_2, m_2, x_2)
\ldots (n_i, m_i, x_i) \ldots (n_N, m_N, x_N)$, where for each $i$, $n_i$ is
the number of *successes*, and $m_i$ is the number of *failures*, out of a
total number of $n_i + m_i$ independent *trials*, then we can model this data as
$$
n_i \sim \mathrm{binomial}(p_i, n_i+m_i),\quad \log\large\left(\frac{p_i}{1-p_i}\right) = \alpha + \beta x_i.
$$
This is binomial logistic regression.

