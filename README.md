# BEC-108-HMM

## Query Sequence

```text
CTTCATGTGAAAGCAGACGTAAGTCA
```

---

## Viterbi Value Matrix

```text
[[        -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf]

 [ -1.38629436  -2.87794924  -4.36960411  -5.86125899  -7.35291387
   -8.84456875 -10.33622362 -11.8278785  -13.31953338 -14.81118825
  -16.30284313 -17.79449801 -19.28615288 -20.77780776 -22.26946264
  -23.76111751 -25.25277239 -26.74442727 -28.23608214 -29.72773702
  -31.2193919  -32.71104677 -34.20270165 -35.69435653 -37.1860114
  -38.67766628]

 [        -inf         -inf         -inf         -inf -11.15957636
          -inf -11.19844713         -inf -14.18175689 -18.61785074
  -20.10950562 -21.6011605  -20.14837639         -inf -26.07612513
  -24.62334102 -29.05943488         -inf -29.09830565         -inf
  -35.02605439 -36.51770926 -35.06492516         -inf         -inf
  -42.48432877]

 [        -inf         -inf         -inf         -inf         -inf
  -12.07586709 -14.4838127  -12.11473786 -14.52268347 -15.09804762
  -16.11969887 -17.14135011 -19.54929572 -21.95724133 -22.97889258
  -25.38683819 -25.53963176 -27.94757736 -30.35552297 -30.01459639
  -31.03624763 -32.05789888 -34.46584449 -35.48749574 -37.89544135
  -38.91709259]

 [        -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf         -inf         -inf         -inf         -inf
          -inf]]
```

---

## Viterbi Trace Matrix

```text
[[ 0 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1  -1 -1]
 [ 0  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1  1   1  1]
 [ 0 -1 -1 -1  1 -1  1 -1  1  1  1  1  1 -1  1  1  1 -1  1 -1  1  1  1 -1  -1  1]
 [ 0 -1 -1 -1 -1  2  3  2  3  2  3  3  3  3  3  3  2  3  3  2  3  3  3  3   3  3]
 [ 0 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1 -1  -1 -1]]
```

---

## Best State Path

```text
EEEEEEEEEEEEEEEEEEEEEEEEEE
```

---

## Best Log Probability

```text
-38.677666280562796
```

---

## Observation

The Viterbi algorithm predicts that the entire sequence belongs to the exon (`E`) state. This happens because the transition probability of remaining in the exon state is high, while transitioning to the splice donor state (`5`) has relatively low probability.

The final log probability is negative because all computations are performed in log scale. Since probabilities are values between 0 and 1, their logarithms are negative.
