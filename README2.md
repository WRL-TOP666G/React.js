### Can an O(n) algorithm ever exceed O(n^2) in terms of computation time?

It’s dependent on the dataset and algorithms. Big-O analysis isn’t used to determine absolute resource usage, but to compare how the resource usage grows with the input size. For example, let’s say the o(n^2) algorithm takes cn^2 operations for some c and the O(n) algorithm takes dn operations for some d. If c=1 and d=100, then the O(n) algorithm would be slower until n=100, at which point the O(n^2) algorithm would become slower.


