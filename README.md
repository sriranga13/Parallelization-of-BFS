# CUDA_ParallelProcessing_BFS
# Goal of this project is to analyze the performance of BFS by implementing it in 3 different approaches in parallel processing.

The repository consists of source code files for three different approaches for implementation of BFS.
Below are the different approaches
1) Work
2) Edge
3) Vertex

The source code for these approaches in written in CUDA C language.
The serial approach of implementing BFS is written in C++ language. It is implemented without parallel processing.
To generate the graph of different sizes a random graph generator has been implemented in C++.

Steps for execution on Tesla server:
1) g++ -o <any-name> random_graph_generator.cpp
  
2) ./random <input-name> <n> <m>
n – no. of vertices
m – no. of edges
  
3) g++ -o serial serial_bfs.cpp

4) ./serial input 5 9

5) ./run.sh parallel_BFS_vertex

6) ./parallel_BFS_vertex input 5 9

Steps 5 and 6 only need to be changed for the remaining two approaches according to their name.
  
The source codes contains the timer to calculate the time taken for execution of each program.
