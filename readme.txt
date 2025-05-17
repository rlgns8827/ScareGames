Kihoon Yoo
2486883
kiyoo@chapman.edu 
CPSC-350-04
PA 5 : Scare Games

List of source files:
-Main.cpp
-Monster.h
-Monster.cpp
-RunScareGame.cpp
-RunScareGame.h
-TournamentNode.h
-TournamentTree.cpp
-TournamentTree.h
-DOTFileGeneratorMethod.h
-monster.txt

Notable Compiling Errors:
-undefined reference to 'Monster::operator!='
-no match for ‘operator==’ or operator<
-class TournamentTree<T> has no member named 'buildTreeRecursive'
-no matching function for call to 'saveTreeAsDot'
-‘std::vector<Monster*>’ has no member named ‘push_back’

References:
    DOTFileGeneratorMethods.cpp - Utility used to output tournament trees as DOT files (Provided in the assignment)
    https://en.cppreference.com/w/cpp/language/operators
    https://dreampuf.github.io/GraphvizOnline/?engine=dot#digraph%20TournamentTree%20%7B%0D%0A%20%20%20%20node0%20%5Blabel%3D%22Sulley%2C%20(Power%3A%20120)%22%5D%3B%0D%0A%20%20%20%20node1%20%5Blabel%3D%22Sulley%2C%20(Power%3A%20120)%22%5D%3B%0D%0A%20%20%20%20node2%20%5Blabel%3D%22Sulley%2C%20(Power%3A%20120)%22%5D%3B%0D%0A%20%20%20%20node3%20%5Blabel%3D%22Sulley%2C%20(Power%3A%20120)%22%5D%3B%0D%0A%20%20%20%20node4%20%5Blabel%3D%22Sulley%2C%20(Power%3A%20120)%22%5D%3B%0D%0A%20%20%20%20node3%20-%3E%20node4%3B%0D%0A%20%20%20%20node5%20%5Blabel%3D%22Mike%2C%20(Power%3A%20115)%22%5D%3B%0D%0A%20%20%20%20node3%20-%3E%20node5%3B%0D%0A%20%20%20%20node2%20-%3E%20node3%3B%0D%0A%20%20%20%20node6%20%5Blabel%3D%22Randall%2C%20(Power%3A%20100)%22%5D%3B%0D%0A%20%20%20%20node7%20%5Blabel%3D%22Randall%2C%20(Power%3A%20100)%22%5D%3B%0D%0A%20%20%20%20node6%20-%3E%20node7%3B%0D%0A%20%20%20%20node8%20%5Blabel%3D%22Art%2C%20(Power%3A%2080)%22%5D%3B%0D%0A%20%20%20%20node6%20-%3E%20node8%3B%0D%0A%20%20%20%20node2%20-%3E%20node6%3B%0D%0A%20%20%20%20node1%20-%3E%20node2%3B%0D%0A%20%20%20%20node9%20%5Blabel%3D%22Johnny%2C%20(Power%3A%20110)%22%5D%3B%0D%0A%20%20%20%20node10%20%5Blabel%3D%22TerryAndTerri%2C%20(Power%3A%2085)%22%5D%3B%0D%0A%20%20%20%20node11%20%5Blabel%3D%22TerryAndTerri%2C%20(Power%3A%2085)%22%5D%3B%0D%0A%20%20%20%20node10%20-%3E%20node11%3B%0D%0A%20%20%20%20node12%20%5Blabel%3D%22Squishy%2C%20(Power%3A%2075)%22%5D%3B%0D%0A%20%20%20%20node10%20-%3E%20node12%3B%0D%0A%20%20%20%20node9%20-%3E%20node10%3B%0D%0A%20%20%20%20node13%20%5Blabel%3D%22Johnny%2C%20(Power%3A%20110)%22%5D%3B%0D%0A%20%20%20%20node14%20%5Blabel%3D%22Johnny%2C%20(Power%3A%20110)%22%5D%3B%0D%0A%20%20%20%20node13%20-%3E%20node14%3B%0D%0A%20%20%20%20node15%20%5Blabel%3D%22Chet%2C%20(Power%3A%2095)%22%5D%3B%0D%0A%20%20%20%20node13%20-%3E%20node15%3B%0D%0A%20%20%20%20node9%20-%3E%20node13%3B%0D%0A%20%20%20%20node1%20-%3E%20node9%3B%0D%0A%20%20%20%20node0%20-%3E%20node1%3B%0D%0A%20%20%20%20node16%20%5Blabel%3D%22Mike%2C%20(Power%3A%20115)%22%5D%3B%0D%0A%20%20%20%20node17%20%5Blabel%3D%22Johnny%2C%20(Power%3A%20110)%22%5D%3B%0D%0A%20%20%20%20node18%20%5Blabel%3D%22Johnny%2C%20(Power%3A%20110)%22%5D%3B%0D%0A%20%20%20%20node17%20-%3E%20node18%3B%0D%0A%20%20%20%20node19%20%5Blabel%3D%22Randall%2C%20(Power%3A%20100)%22%5D%3B%0D%0A%20%20%20%20node20%20%5Blabel%3D%22Randall%2C%20(Power%3A%20100)%22%5D%3B%0D%0A%20%20%20%20node19%20-%3E%20node20%3B%0D%0A%20%20%20%20node21%20%5Blabel%3D%22TerryAndTerri%2C%20(Power%3A%2085)%22%5D%3B%0D%0A%20%20%20%20node19%20-%3E%20node21%3B%0D%0A%20%20%20%20node17%20-%3E%20node19%3B%0D%0A%20%20%20%20node16%20-%3E%20node17%3B%0D%0A%20%20%20%20node22%20%5Blabel%3D%22Mike%2C%20(Power%3A%20115)%22%5D%3B%0D%0A%20%20%20%20node23%20%5Blabel%3D%22Mike%2C%20(Power%3A%20115)%22%5D%3B%0D%0A%20%20%20%20node24%20%5Blabel%3D%22Mike%2C%20(Power%3A%20115)%22%5D%3B%0D%0A%20%20%20%20node23%20-%3E%20node24%3B%0D%0A%20%20%20%20node25%20%5Blabel%3D%22Art%2C%20(Power%3A%2080)%22%5D%3B%0D%0A%20%20%20%20node23%20-%3E%20node25%3B%0D%0A%20%20%20%20node22%20-%3E%20node23%3B%0D%0A%20%20%20%20node26%20%5Blabel%3D%22Chet%2C%20(Power%3A%2095)%22%5D%3B%0D%0A%20%20%20%20node27%20%5Blabel%3D%22Squishy%2C%20(Power%3A%2075)%22%5D%3B%0D%0A%20%20%20%20node26%20-%3E%20node27%3B%0D%0A%20%20%20%20node28%20%5Blabel%3D%22Chet%2C%20(Power%3A%2095)%22%5D%3B%0D%0A%20%20%20%20node26%20-%3E%20node28%3B%0D%0A%20%20%20%20node22%20-%3E%20node26%3B%0D%0A%20%20%20%20node16%20-%3E%20node22%3B%0D%0A%20%20%20%20node0%20-%3E%20node16%3B%0D%0A%7D%0D%0A%0D%0A
    https://graphviz.org/doc/info/lang.html
    https://chatgpt.com/

Instructions for compiling:
    To compile: g++ main.cpp Monster.cpp RunScareGame.cpp -o monster.exe
    To run: ./monster.exe monsters.txt single
            ./monster.exe monsters.txt double
            