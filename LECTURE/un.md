# DIANA (Divisive Analysis)
* Introduced in Kaufamann and Rousseeuw (1990)
* Inverse order of AGENS
1. All objects belong to the same cluster
2. Repeat until all objects belong to their own cluster
   * Split clusters so that distance of clusters generated > threshold
<img width="565" height="167" alt="Screenshot 2025-11-10 at 2 22 34 PM" src="https://github.com/user-attachments/assets/80f656ec-6207-4599-af3d-f168be6aaf27" />

## Challenge in Divisive Methods
* For every split, need to consider $2^n - 1$ ways of partitioning a set of *n* objects to two exclusive subsets
* This can be very expensive
   * DIANA does not enumerate all splits
   * Uses greedy heuristics for partitioning:
       ###### Pick object with max dissimilarity from the rest, move it to a new cluster
       ###### Keep doing so until distance threshold satisfied


## An Optimization Comparison
| K-means (Lloy's algorithm) | AGENS & DIANA |
|:-------------------------------|:-----------------------|
| Uses "algernating optimization" or "block coordinate descent" | Uses "greedy optimization" |
| Fixing all but one variable, update the rest | Makes a locally optimal (**greedy**) choice |
| Iterate over all variables <br> Iterate until convergence | Also uses heuristics on top of that |
