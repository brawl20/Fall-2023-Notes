* [Algorithm Analysis]
	* Goal
		* Predict the resources that an algorithm requires.
	* What kind of resources?
		* **Memory**
		* Communication Bandwidth
		* Hardware Requirements
		* **Running time**
	* Approaches
		* [[Empirical Tests]]
		* [[Mathematical Analysis]]
	* How?
		* The time taken by an algorithm depends on the input
			* Searching in a sequence of 1000 numbers takes longer than in a sequence of 3 numbers
			* Some algorithms take different amounts of time on two inputs of the same size
				* Searching in a sorted sequence
		* Input Size (Problem size)
			* Depends on the problem being studied
			* usually, number of items in the input
			* if multiplying two numbers, length of number
			* Graph algorithms: input size in terms of vertices and edges (towards the end of the course)
	* Example
		* ![[Pasted image 20230824132731.png]]
		* ![[Pasted image 20230824132839.png]]
			* T_a -> Average
			* T_c -> Worst (Max)
			* T_i -> Best case (Min)
		* ![[Pasted image 20230824132857.png]]
	* Best case analysis
		* Shortest running time for any input of size n
		* Often meaningless and is not a practical expectation to rely on (guaranteeing a lower bound on an algorithm doesn't provide any information as in the worst case, an algorithm may take years to run)
	* Worst case analysis
		* Longest running time for any input of size n
		* It guarantees that the algorithm will not take any longer
		* provides an upper bound on the running time
		* Worst case occurs often search for an item that doesn't exist
	* Average case analysis
		* Running time averaged for all possible input
		* It is hard to estimate the probability of all possible inputs.
* [Asymptotic Notation]
	* Big Oh
	* Big Omega
	* Big Theta
	* Little Oh
	* Little Omega
* [Asymptotic Dominance]
________
[Problem Solving Main Steps]
1. Problem Definition
2. Algorithm design / Algorithm specification
3. Algorithm analysis
4. Implementation
5. Testing
6. Maintenance