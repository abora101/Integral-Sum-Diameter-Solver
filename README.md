The main.cpp file is the actual solver.

The code works by building up the set L by inserting elements in increasing order of magnitude, and stopping a search prematurely if |T \setminus M| exceeds its maximum value, or if cycles are formed in the graph. Checking for these possibilities is able to substantially improve the runtime beyond the O(2^n) of previous bitset approaches (see "slow" code in development) central to past computational approaches. 

In essence, the code brute-forces all possibilities and intelligently eliminates those small sets which cannot form a path. An important note - the code only checks for cases when isd < sd (i.e., there is at least one nonpositive label in L), as sd was solved without the use of advanced programs. 

Final paper published in Discrete Mathematics, "On the sum and sum-diameter of paths". Share link: https://authors.elsevier.com/c/1jl4h,H-cal8f valid before Oct. 30. 
