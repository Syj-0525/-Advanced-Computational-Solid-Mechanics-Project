version https://git-lfs.github.com/spec/v1
oid sha256:60eed5b92f83443477d72b41a2980adb15999488f999c401c97f2228922369d5
size 12

This is a project about computational solid mechanics

The program is written in C + + language. This program is mainly used to realize preprocessing, including reading the relevant input file, storing the node and element information in the corresponding node class and element class, and accessing them by instantiating of generated object.

The program is divided into five parts, including matlab engine function, Tools function, main function, Node class, and Element class. Tools function contains some common function definitions, such as reading txt files, printing vectors, etc. Each object of the class “Node” contains information of the X- and Y-coordinates, which could be accessed as n.X, n.Y. Each object of the class “Element” represents a spring connecting the two nodes. It contain the information including the numbering of the two nodes, which can be accessed as e.node(1) and e.node(2). And matlab engine function is used to call MATLAB engine to realize mixed programming with MATLAB for visualization, such as ploting and so on. As for libeng.lib;libmat.lib;libmex.lib;libmx.lib, these four files are the static libraries that must be relied on when calling the Matlab engine. By the way, in order to realize matrix operation for convenience , the program calls foreign libraries such as boost and eigen template classes. For the sake of invoking them, it is necessary to set the relevant path in the IDE. You can open Project 1_v1 .sln solution, compile and run the main function through visual studio IDE under Windows system to obtain the result. Optionally, click Project 1_v1.exe on the x64/Release directory to run it.
