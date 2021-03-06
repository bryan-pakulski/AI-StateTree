# StateTree
A C++ data structure (essentially a standard tree, but with features needed for state systems)

### Features:
* Add / Delete Nodes
* Trim Duplicate subtrees
* Breadth First Search
* Iterative Deepening Depth First Search
* Hamming distance between data points

### Initialisation and usage

* Include header file in project
* Initialise State tree with type
* Add nodes

![image](images/Initialise.png?raw=true)

Which should result in output as follows:

![image](images/Output.png?raw=true)

### TODO:
* Different search options BFS, DFS, IDDFS for tree (BFS done, IDDFS done, only DFS left)

### NOTE:
when using struct data types make sure to include an operator overload for " == " i.e. A state tree of type struct st (see below for structure type)

![image](images/Structs.png?raw=true)

Will need a overload operator like this in order for the library to function:

![image](images/Overload.png?raw=true)

This also applies to the hamming distance function, if you are using structs you must overload the ^ operator and return the data value of struct1 ^ struct2 in order for the function to work correctly, standard data types will work fine;

![image](images/hammingdistance.png?raw=true)
