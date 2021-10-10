### Can an O(n) algorithm ever exceed O(n^2) in terms of computation time?
It’s dependent on the dataset and algorithms. Big-O analysis isn’t used to determine absolute resource usage, but to compare how the resource usage grows with the input size. For example, let’s say the o(n^2) algorithm takes cn^2 operations for some c and the O(n) algorithm takes dn operations for some d. If c=1 and d=100, then the O(n) algorithm would be slower until n=100, at which point the O(n^2) algorithm would become slower.


### Signed 32 bits and unsigned 32 bits can represent the same number of integers
In 32bit integers, an unsigned integer has a range of 0 to 32 power of 2 -1 = 0 to about 4 billion. The signed version goes from -31 power of 2-1 to 31 power of 2, which is about -2 billion to +2 billion. The range is the same, but it is shifted on the number line.



### Running a task on 1 thread can be faster than running it on 2 threads
No, running a task on 1 thread is slower than running it on 2 threads. For example, I work on software that analyzes documents. One of the things I do to documents is break them up into individual words. And when I’m breaking documents up into words, I’m never working with just one document. Usually my minimum is 1000 separate documents that I want to break up into words. One of the great things about breaking documents up into words is that the work I do to break another into words. If my problem is to break 1000 documents into the words in each document, and a single threaded solution takes 100 seconds to do this work on 1000 documents, it is pretty easy to create a solution with 2 threads that dose the same amount of work in 50 seconds. Therefore, two threads will be closed to twice as fast as one thread.


### All recursive algorithms can be altered to iterative algorithms.
Yes, any problem that can be solved recursively can also be solved through the use of iteration. There’s a simple ad hoc proof for this. Since we can build a Turing complete language using strictly iterative structures and a Turing complete language using only recursive structures, then the two are therefore equivalent. Iteration is the use of a looping construct like a while loop, for loop, etc in order to solve a problem, whereas recursion is the use of a function that calls itself to solve a problem. Recursion uses more memory but is sometimes clearer and more readable. 


### 2 different hash keys will always have different hash codes.
No, when two different objects have the same hash code, we call this a collision. A collision is nothing critical, it just means that there is more than one object in a single bucket, so a HashMap lookup has to look again to find the right object. A lot of collisions will degrade the performance of a system, but they won’t lead to incorrect results. Therefore, two different hash keys has some chance to have different hash codes or have the same hash code.



### An algorithm implemented with O(1) time can not be improved faster.
An O(1) algorithm still has room for improvements, instead of lowering time complexity. We can lower the constant factor. For example, we have two algorithms that solve the same problem. The slow algorithm takes 100 steps, and the fast algorithm takes 1 steps. Although they both run in O(1), a change from the slow algorithm to the fast algorithm still makes the program faster.



### Describe hash map to non-technology person, including real-world example.
A HashMap is a data structure that is able to map certain keys to certain values. The keys and values could be anything. It does not guarantee the insertion order of elements or items into HashMap. It also cannot have duplicate keys but it can have duplicates values. For example, it’s like a dictionary of all words. And you know where exactly to go and get the meaning of the word without going every other word. The other example is if I were making a game, I might link every username to a friends list, represented by a list of string. 
