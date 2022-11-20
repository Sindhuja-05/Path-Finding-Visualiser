# Path-Finding-Visualiser
Objective of the project : Generate the most optimal path solution between two given points using A – star algorithm.

1)Overview of the project

• MAZE CREATION:
Maze is created using recursive division. This algorithm works as follows: 
        Begin with the maze's space with no walls. Call this a chamber. Divide the chamber with a randomly positioned wall (or multiple walls) where each wall contains a randomly positioned passage opening within it. Then recursively repeat the process on the sub chambers until all chambers are minimum sized. This method results in mazes with long straight walls crossing their space, making it easier to see which areas to avoid.

• A* algorithm:
        A* is a graph traversal and path search algorithm, which is often used in many fields of computer science due to its completeness, optimality, and optimal efficiency. One major practical drawback is its O(bd) space complexity, as it stores all generated nodes in memory. Thus, in practical travel-routing systems, it is generally outperformed by algorithms which can pre-process the graph to attain better performance, as well as memory-bounded approaches; however, A* is still the best solution in many cases. What A* Search Algorithm does is that at each step it picks the node according to a value-‘f’ which is a parameter equal to the sum of two other parameters – ‘g’ and ‘h’. At each step it picks the node/cell having the lowest ‘f’, and process that node/cell. We define ‘g’ and ‘h’ as simply as possible below g = the movement cost to move from the starting point to a given square on the grid, following the path generated to get there. h = the estimated movement cost to move from that given square on the grid to the final destination. This is often referred to as the heuristic, which is nothing but a kind of smart guess. We really don’t know the actual distance until we find the path, because all sorts of things can be in the way.
       
• We allow the user to create a start node(pink) and end node(red), and the walls(black) to barrier the path between the nodes. 
• If ever the path is not found a ‘Path Not Found’ Message is displayed in the dialog box. 
• There is special visualization for the path finding with multicolour display as the path progresses.

2.Description about Python Packages used

• Pygame is a free and open-source cross-platform library for the development of multimedia applications like video games using Python. It uses the Simple Direct Media Layer library and several other popular libraries to abstract the most common functions, making writing these programs a more intuitive task. Pygame is suitable to create client-side applications that can be potentially wrapped in a standalone executable.

• The priority queue is an advanced type of the queue data structure. Instead of dequeuing the oldest element, a priority queue sorts and dequeues elements based on their priorities. Priority queues are used to handle scheduling problems where some tasks are prioritized over others. The queue.PriorityQueue ClassPython provides a built-in implementation of the priority queue data structure. Since the queue.PriorityQueue class needs to maintain the order of its elements, a sorting mechanism is required every time a new element is enqueued. Python solves this by using a binary heap to implement the priority queue.

• NumPy is a Python library used for working with arrays. It also has functions for working in domain of linear algebra, fourier transform, and matrices.NumPy aims to provide an array object that is up to 50x faster than traditional Python lists. The array object in NumPy is called ndarray, it provides a lot of supporting functions that make working with ndarray very easy.
