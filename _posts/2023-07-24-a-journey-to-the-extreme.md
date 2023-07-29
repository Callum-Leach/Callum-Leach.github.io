---
title: "A Journey To The Extreme"
last_modified_at: 2023-07-24
mathjax: true
categories:
  - Statistics
tags:
    - Statistics
---

Who wants to be average? To fit perfectly into a trend? Those who dare to explore beyond the ordinary, are the ones to reveal the treasures that lie at the fringes. Let's go down this rabbit hole of Extreme Value Analysis, and see where it comes out.

## Why do we only study extreme observations?

Phenomena which generate extreme value observations are fundamentally different than those which generate typical values. So, we make it of paramount importance that for our modelling we select only the extreme values. There are two common methods of doing this:

1. Block Maxima
2. Peaks Over Threshold

Assuming we have a series of independent and identically distributed observations $$X_1, X_2, \dots$$ for *Block Maxima* data are blocked into sequences of observations of length $$n$$ generating $$M_{n,1}, \dots, M_{n,m}$$. Often the blocks correspond to a time period, so for example annual maxima where $$n$$ is the number of observations in a year.

For example: Say we have measurements taken every hour, for a 50 year span. Here $$n=365*24=8760$$ observations per year. We could thus denote this as

$$M_{8760, i}, \space i=1,\dots,50$$

Which would give the annual maxima for each year $$i$$. Hence we call $$n$$ our *block length*.

If we assume that $$X_t$$ has cdf $$F_X(x)$$:

$$F_{M_n}(x) = P(M_n \leq x) = P(X_t \leq x \space \forall t=1,\dots,n)$$