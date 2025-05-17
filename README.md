# Scare Games

## Identifying Information: 
1. Full name: Kihoon Yoo
2. Student ID: 2480883
3. Chapman Email: kiyoo@chapman.edu
4. Course number and section: CPSC-350-04
5. Assignment or exercise number: PA5: Scare Games

## Project Description
This project implements a simulation of the Scare Games using tournament trees in C++. It supports both single-elimination and double-elimination formats, allowing monsters to compete based on their scream power. The structure of the tournaments is visualized using DOT files, and the system utilizes object-oriented design to manage competitors, matches, and progression logic effectively.

## Key Features
- Single and Double-Elimination Tournaments: Supports both standard and double-elimination formats, allowing competitors a second chance in the losers' bracket.
- Monster-Based Competition: Each competitor is represented as a Monster object with a unique name and scream power level used to determine match outcomes.
- Binary Tournament Tree Structure: Implements a tournament as a binary tree (TournamentTree), where each node (TournamentNode) represents a match between two competitors.
- Dynamic Competitor Management: Uses std::vector to manage flexible lists of participants and losers, allowing tournaments of any size.
- Automatic Bye Handling: Automatically advances competitors when there is an odd number of players in a round.
- DOT File Generation: Generates DOT files to visually represent tournament trees. These can be rendered using Graphviz for a clear graphical overview of matches.
- Command-Line Interface: Supports command-line arguments to specify the input file and tournament type.
- Object-Oriented Design: Modular and maintainable codebase with clean separation of responsibilities across classes.

## Files
1. Main.cpp
2. Monster.h
3. Monster.cpp
4. RunScareGame.cpp
5. RunScareGame.h
6. TournamentNode.h
7. TournamentTree.cpp
8. TournamentTree.h
9. DOTFileGeneratorMethod.h
10. monster.txt
11. README.md

## Known Error 
- There are no known errors in this program.

## References
- https://en.cppreference.com/w/cpp/language/operators
- https://dreampuf.github.io/GraphvizOnline/
- https://graphviz.org/doc/info/lang.html
- Received debugging help from the Chapman TLC
- Received additional debugging help from Dr.Stevens

## Instructions for compiling
- To compile:  g++ main.cpp Monster.cpp RunScareGame.cpp -o monster.exe
- To run: ./monster.exe monsters.txt single
-         ./monster.exe monsters.txt double
-     
