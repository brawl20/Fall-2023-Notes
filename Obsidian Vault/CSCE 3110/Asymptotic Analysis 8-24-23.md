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
	* Examples
		* ![[Pasted image 20230824132731.png]]
		* ![[Pasted image 20230824132839.png]]
			* T_a -> Average
			* T_c -> Worst (Max)
			* T_i -> Best case (Min)
		* ![[Pasted image 20230824132857.png]]
		* ![[Pasted image 20230824135627.png]]
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
	* Random-Access Machine (RAM)
		* In order to predict running time, we need a (simple) computational model: the Random-Access Machine (RAM)
			* Instructions are executed sequentially
				* No concurrent operations
			* Each basic instruction takes a constant amount of time
				* Arithmetic: add, subtract, divide, remainder, floor, ceiling, shift left/right
				* Data movement: load, store, copy
				* Control: conditional/unconditional branch, subroutine call and return
				* Loops and subroutine calls are not simple operations. That depend upon the size of the data and the contents of the subroutine. "Sort" is not a single step operation.
			* Each memory access takes exactly 1 step.
		* We measure the run time of an algorithm by counting the number of steps.
	* Running Time
		* On a particular input, number of primitive operations (steps, instructions) executed
		* Assume that all primitive operations have the same constant cost
		* If calling a subroutine, the actual case must be used
	* The RAM model of Computation
		* The worst-case (time) complexity of an algorithm is the function defined by the maximum number of steps taken on any instance of size n.
		* The best-case complexity of an algorithm is the function defined by the minimum number of steps taken on any instance of size n.
* [Asymptotic Notation]
	* Big Oh
		* ![[Pasted image 20230824141329.png]]
		* In plain English: S
	* Big Omega
		* ![[Pasted image 20230824141409.png]]
	* Big Theta
		* ![[Pasted image 20230824141441.png]]
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