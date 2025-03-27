# CMPS 2200 Reciation 5
## Answers

**Name:**____Zoe Murphy___


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**


|      n |   qsort-fixed-pivot |   qsort-random-pivot |   ssort |
|--------|---------------------|----------------------|---------|
|    100 |               0.077 |                0.074 |   0.674 |
|    200 |               0.144 |                0.161 |   0.615 |
|    500 |               0.391 |                0.405 |   0.591 |
|   1000 |               0.793 |                0.830 |   3.067 |
|   2000 |               1.658 |                1.809 |   7.657 |
|   5000 |               4.758 |                4.931 |   0.780 |
|  10000 |               9.680 |                9.955 |   0.815 |
|  20000 |              19.319 |               20.721 |   0.892 |
|  50000 |              51.287 |               58.223 |   0.890 |
| 100000 |             108.595 |              119.783 |   0.949 |


qsort_fixed_pivot has a decent runtime. ssort is very very slow. It has an overall runtime of O(n^2), so that is expected. qsort-random-pivot also has a decent runtime similar to qsort-fixed-pivot (they both have O(n log n) overall runtimes)

- **1c.**

|      n |   qsort-fixed-pivot |   qsort-random-pivot |   ssort |   tim_sort |
|--------|---------------------|----------------------|---------|------------|
|    100 |               0.074 |                0.078 |   0.730 |      0.005 |
|    200 |               0.136 |                0.161 |   0.586 |      0.010 |
|    500 |               0.368 |                0.435 |   0.576 |      0.028 |
|   1000 |               0.820 |                0.872 |   3.300 |      0.066 |
|   2000 |               1.634 |                1.786 |  52.990 |      0.154 |
|   5000 |               4.452 |                5.128 |   0.887 |      0.385 |
|  10000 |               9.520 |               10.140 |   0.826 |      0.746 |
|  20000 |              19.813 |               20.879 |   0.816 |      1.671 |
|  50000 |              51.303 |               56.848 |   0.915 |      4.590 |
| 100000 |             106.616 |              116.361 |   0.972 |      9.706 |

tim_sort is obviously our fastest method, it outpaces all of our other methods. It has an O(n log n) runtime, but it can have an O(n) runtime which is great. 