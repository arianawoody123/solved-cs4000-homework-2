Download Link: https://assignmentchef.com/product/solved-cs4000-homework-2
<br>
<strong>1      Introduction</strong>

The Hamiltonian Path Problem is a classic computer science problem: Given a graph and two vertices <em>i </em>and <em>j</em>, determine whether there is a path from <em>i </em>to <em>j </em>in the graph that visits each vertex in the graph exactly once. Now, this problem is well-known to be NP-complete. I have written a solution to this problem (Hamiltonian_Path.cc) that uses the next_permutation function in C++ to generate all of the permutations (tours) of the vertices that start at vertex <em>i </em>and end in vertex <em>j</em>. This program will find a Hamiltonian Path, if it exists. Otheriwse, it will say that no such path exists. However, this program is painfully slow. On a small graph (small_graph.dat) with 5 vertices, it finds the the tour 2 0 1 3 4 from 2 to 4 in much less than a second. But, on a bigger graph (big.dat) with 13 vertices, it takes over one minute to find a solution. On bigger graphs (bigger.dat and biggest.dat), it takes much longer to solve. For example, on input

5 2 4

<ul>

 <li>: 1 2 4</li>

 <li>: 0 2 3 4</li>

 <li>: 0 1 3</li>

 <li>: 1 2 4</li>

 <li>: 0 1 3</li>

</ul>

The output of the program should be “Tour = 2 0 1 3 4”.

Your task is to make this code faster using parallel computing. Modify Hamiltonian_Path.cc using OpenMP so that

<ol>

 <li>Your modified program still produces the correct results, and</li>

 <li>It is at least 75% efficient on dat on a machine with 4 cores/processors.</li>

</ol>