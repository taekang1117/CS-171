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

## Single-linkage & Minimum Spannig Tree
##### Minimum Spanning Tree
<img width="610" height="310" alt="Screenshot 2025-11-10 at 2 29 08 PM" src="https://github.com/user-attachments/assets/abf0ae59-28df-4691-b2dc-1083e88d2590" />

* Can be shown that those problems are equivalent
  * See: Gower and Ross, *Minimum Spanning Trees and Single Linkage Cluster Analysis*, Journal of the Royal Statistical Society, 1969
* Greedy algorithms can give (one of the many) MST optimal solution
  * Kruskal's algorithm
  * Prim's algorithm
* This also carries over for Single-linkage Hierarchical Clustering 
