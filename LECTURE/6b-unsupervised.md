# Roadmap
#### Density-Based Methods
#### Evaluating of Clustering

# Density-Based Clustering Methods
* Clustering based on density (local cluster criterion)
* Motivation
  * Discover clusters of arbitrary shape
  * Handle noise
 
<img width="613" height="218" alt="Screenshot 2025-11-10 at 2 39 58 PM" src="https://github.com/user-attachments/assets/5f5123b5-122f-4aab-8169-54055dbd7c21" />

### Two Parameters:
##### Eps: Maximum radius of the neightborhood
##### MinPts: Minimum number of points in an Eps-neighborhood of that point

### $N_{Eps}(p)$
Points q belong to beighborhood of $p | dist(p,q) \leq Eps$

### Directly desnsity reachable
A point p is directly density reachable from a point $q w.r.t. Eps, MinPts$ if 
* p belongs to $N_{Eps}(q)$, and
* core point condition: <br>
$|N{Eps}(q)| \geq MinPts$
