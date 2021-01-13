  Course		 : Concurrent and Parallel Programming
	Module		 : PDP
	Semester	 : Semester I
	Assignmnet Number: Assignment 2 OpenMP/MPI
	
	Problem Statement:consider a large two-dimensional array of size [1000,1000] filled with single digit numbers between 0 to 9, your 				  task is to implement a parallel solution using openmp and mpi that search for a two-digit number, can be hard coded. 				  the search will be horizontal, vertical, diagonal, and counter diagonal from left to right and up to down.
	
	Example 	 :we are searching for Number 44, so output is 6 times and time taken 0.000042(Varying)
Libraries Requires:	
			sudo apt-get install gcc
			sudo apt-get install libomp-dev
			sudo apt-get install libopenmpi-dev

	To Compile:     mpicc assignmnet2_OpenMP_MPI_implementation.c -o assignmnet2_OpenMP_MPI_implementation -fopenmp
	To Run    :     ./assignmnet2_OpenMP_MPI_implementation
	
	Give Input:     15 16
		        4 8 3 6 2 1 9 3 5 2 9 6 4 9 1
			6 5 8 1 4 3 3 1 4 1 4 8 6 7 7
			2 3 6 7 1 0 6 7 0 4 1 3 0 6 8
			8 7 2 6 2 5 8 1 2 7 0 2 7 7 6
			7 8 1 8 7 0 4 5 6 9 5 9 3 2 0
			3 0 1 5 1 5 4 7 0 4 2 8 5 6 6
			2 6 3 5 0 8 5 1 6 4 5 1 3 7 1
			7 1 0 3 7 0 2 4 4 6 7 4 1 2 9
			1 9 5 4 5 3 7 1 2 1 4 9 3 0 3
			2 1 3 8 7 0 9 0 0 8 1 8 2 3 9
			9 7 5 2 9 2 9 8 6 6 1 9 1 8 7
			1 3 7 9 1 0 5 9 5 0 3 1 9 4 3
			3 2 1 1 2 6 7 6 6 3 1 0 1 4 0
			7 5 9 8 5 7 9 6 9 1 9 2 0 7 7
			9 7 2 0 7 2 1 9 6 4 5 5 7 1 8
			3 7 1 4 8 7 6 8 4 9 0 6 2 0 7 	
	Output  :
			I'm thread 0 in process 0
			I'm thread 1 in process 0

			Provided thread support level: 1
			  0 - MPI_THREAD_SINGLE
			  1 - MPI_THREAD_FUNNELED
			  2 - MPI_THREAD_SERIALIZED
			  3 - MPI_THREAD_MULTIPLE

			Enter the size of the 2d Array/Size of matrix i.e Enter the Number of rows and Number of columns
			15 16
			4 8 3 6 2 1 9 3 5 2 9 6 4 9 1
			6 5 8 1 4 3 3 1 4 1 4 8 6 7 7
			2 3 6 7 1 0 6 7 0 4 1 3 0 6 8
			8 7 2 6 2 5 8 1 2 7 0 2 7 7 6
			7 8 1 8 7 0 4 5 6 9 5 9 3 2 0
			3 0 1 5 1 5 4 7 0 4 2 8 5 6 6
			2 6 3 5 0 8 5 1 6 4 5 1 3 7 1
			7 1 0 3 7 0 2 4 4 6 7 4 1 2 9
			1 9 5 4 5 3 7 1 2 1 4 9 3 0 3
			2 1 3 8 7 0 9 0 0 8 1 8 2 3 9
			9 7 5 2 9 2 9 8 6 6 1 9 1 8 7
			1 3 7 9 1 0 5 9 5 0 3 1 9 4 3
			3 2 1 1 2 6 7 6 6 3 1 0 1 4 0
			7 5 9 8 5 7 9 6 9 1 9 2 0 7 7
			9 7 2 0 7 2 1 9 6 4 5 5 7 1 8
			3 7 1 4 8 7 6 8 4 9 0 6 2 0 7

			The Inputed Matrix by the User is
			4  8  3  6  2  1  9  3  5  2  9  6  4  9  1  6  
			5  8  1  4  3  3  1  4  1  4  8  6  7  7  2  3  
			6  7  1  0  6  7  0  4  1  3  0  6  8  8  7  2  
			6  2  5  8  1  2  7  0  2  7  7  6  7  8  1  8  
			7  0  4  5  6  9  5  9  3  2  0  3  0  1  5  1  
			5  4  7  0  4  2  8  5  6  6  2  6  3  5  0  8  
			5  1  6  4  5  1  3  7  1  7  1  0  3  7  0  2  
			4  4  6  7  4  1  2  9  1  9  5  4  5  3  7  1  
			2  1  4  9  3  0  3  2  1  3  8  7  0  9  0  0  
			8  1  8  2  3  9  9  7  5  2  9  2  9  8  6  6  
			1  9  1  8  7  1  3  7  9  1  0  5  9  5  0  3  
			1  9  4  3  3  2  1  1  2  6  7  6  6  3  1  0  
			1  4  0  7  5  9  8  5  7  9  6  9  1  9  2  0  
			7  7  9  7  2  0  7  2  1  9  6  4  5  5  7  1  
			8  3  7  1  4  8  7  6  8  4  9  0  6  2  0  7  

			The Two digit search value is 44
			Time Taken For the execution is 0.000042
			Count of Number of Occurances of the Search Value i.e Two digit number is 6


