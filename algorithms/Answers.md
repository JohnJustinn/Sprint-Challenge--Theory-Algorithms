1. Exercise 1: Analysis of Runtimes
    * A. O(n)
    * B. O(log n)
    * C. O(sqrt(n))
    * D. O(n log n)
    * E. O(n^3)
    * F. O(n)
    * G. O(n)

2. Exercise 2: Analysis of Algorithms

    * A. 
         ```js
        function maxDifference(array) {
            let min = array[0];
            let max = array[0];

            for (let i = 0; i < array.length; i++) {
                const value = array[i];

                if (value < min) min = value;
                if (value > max) max = value;
            }
            return max - min;
        }

        ```
    * B. 

        A strategy for breaking less eggs:

        Start with the idea of using a binary search tree.
        Pick a floor and if the egg breaks, move down a floor/ Otherwise, move up.
        
        Stop if the egg doesn't break at a particular floor, but does break at the floor above that.  

3. Exercise 3:  Time Complexity

    * A. As the algorithm is iterated, the left array remains empty and the right is n - 1, n - 2 etc.  For this reason, the complexity is O(n^2).

    * B. At every iteration of this algorithm, the array is split into two arrays.  A (log n) will be performed again on these arrays, and at each point has linear complexity, making it O(n log n).