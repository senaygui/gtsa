# Game Tree Search Algorithms [![Build Status](https://travis-ci.org/AdamStelmaszczyk/gtsa.svg?branch=master)](https://travis-ci.org/AdamStelmaszczyk/gtsa) [![Coverage Status](https://coveralls.io/repos/github/AdamStelmaszczyk/gtsa/badge.svg?branch=master)](https://coveralls.io/github/AdamStelmaszczyk/gtsa?branch=master)

C++ library for AI bot programming.

Usage
---

1. Specify game rules by subclassing `State` and `Move`. 
2. Choose AI algorithm (`Minimax`, `MonteCarloTreeSearch`), play by yourself (`Human`) or against external program (`Executable`).
3. Read the game state, pass it to algorithm and output the move. For local, statistically significant tests, use `Tester`.

Game examples
---

- Tic Tac Toe - [game rules](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/tic_tac_toe.md), [code example](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/tic_tac_toe.cpp).
<p><a href="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/tic_tac_toe.md"><img src="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/tic_tac_toe.gif"/></a></p>

- Isola - [game rules](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/isola.md), [code example](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/isola.cpp). 
<p><a href="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/isola.md"><img src="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/isola.gif"/></a></p>

- Connect Four - [game rules](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/connect_four.md), [code example](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/connect_four.cpp).
<p><a href="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/connect_four.md"><img src="https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/examples/connect_four.gif"/></a></p>

Implemented algorithms
---

- [NegaScout](https://en.wikipedia.org/wiki/Principal_variation_search) with [iterative deepening]( https://chessprogramming.wikispaces.com/Iterative+Deepening) and [transposition table](https://en.wikipedia.org/wiki/Transposition_table).
- [Monte Carlo tree search](https://en.wikipedia.org/wiki/Monte_Carlo_tree_search) with [UCT](
https://en.wikipedia.org/wiki/Monte_Carlo_tree_search#Exploration_and_exploitation).

Make commands
---
Execute below commands in the `cpp` directory. 
- `make` builds everything.
- `make test` runs unit tests.
- `make valgrind` runs valgrind's memory leak tests.
- `make play_isola` plays a game of Isola between two bots.

For all the commands check [`Makefile` file](https://github.com/AdamStelmaszczyk/gtsa/blob/master/cpp/Makefile).

Dependencies
---
- To build and run unit tests, `g++-4.8` and `libboost-all-dev` packages are needed.  
- To run valgrind, `valgrind` package is needed.  
- To make GIFs, `imagemagick` package is needed.

You can install all of them with `sudo apt-get install g++-4.8 libboost-all-dev valgrind imagemagick`.

Priorities of the library
---

1. Correctness.
2. Compliance with environment typical for competitions. One file submission, compiled with one invocation of `g++`.
3. Performance.

Would like to help?
---
Suggestions welcome on [Issues](https://github.com/AdamStelmaszczyk/gtsa/issues).
[Pull requests](https://github.com/AdamStelmaszczyk/gtsa/pulls) too.

I'm transferring £50 to anybody who reports an actual bug.
