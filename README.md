### This is AI othello AKA reversi(8×8） like Alpha Zero.
Langage is Python, and using keras of tensorflow.

#### I made it using [this book](https://www.borndigital.co.jp/book/14383.html).
- **master branch is changed 8×8 from the folder named 8_2_reversi  on zip file can download in download on that link.**
- **bitboard branch is changed bitboard from master branch for run faster than master.**
- **bitboard-develop branch is bitboard's develop branch.**

So, **bitboard-develop branch is newest** in this repository and it almost completed to change.    
But, it branch isn't faster than master branch, I can't merge bitboard branch.  
The **game.py** file in bitboard-develop branch is **twice as fast** as it in master branch.  
But, **the pv_mcts.py** file in bitboard-develop branch is about the **same or as slower** as it in master branch.  
So, the execution speed of the **self_play.py** file in the bitboard-develop branch is **also slow**.  


### Explain major files.
- **game.py** file includes a class to simply play reversi.
- **dual_network.py** file is includes a function to create dual network and save best model.
- **pv_mcts.py file** includes functions for exploring Monte Carlo trees.
- **self_play.py file** includes functions to play self-play and save lerning data.
- **train_network.py** file includes a function to learning from self-play's data.
- **evaluate_network.py** file includes  functions conparing latest and past model and evaluating.
- **train_cycle.py** file run when we want to repeat a series of learning.

