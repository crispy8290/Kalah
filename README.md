**Kalah**  
A variation to Mancala, a 2-player turn-based strategy board game.  

**Technical Specifications**  
Runs on console only.  

**Version Number**  
1.0  

**Rules**  
*Setup*  
A board is set up by having "s" number of seeds (1-12) in each "p" number of pits (2-20 total, must be even). 
There are two rows of pits (one upper and one lower), along with two stores (one left and one right).  
Player 1 owns the lower row of pits and the right store.
Player 2 owns the upper row of pits and the left store.

*Objective*  
The objective of the game is for a player to have the majority of available seeds in their own store.  

*Player Turn*  
During a player's turn, the player selects one of their own non-empty pits (by entering the index of the pit) and takes all the seeds and distributes them in a counter-clockwise order, dropping one seed at each pit (including their own store). A player does not deposit a seed into the opponent's store, and instead skips it completely. There are two special checks that occur at the end of the seed distribution. If neither of these events occur, the player's turn ends.    
1. If a player's last seed drop lands in their own store, the player takes another turn.  
2. If a player's last seed drop lands in one of their own empty pits, the player puts that last seed in their store instead, along with any seeds that are in the opponent's directly-opposing pit.  

*Special First Turn*  
The very first move in a new game will prompt the opponent to steal the move as their own first move. This is a game-balancing feature as in a perfect game, the starting player will always win.  

*Winning the Game*  
If a game-ending scenario occurs at any time, the game is terminated and a winner is determined. Win conditions are as follows:   
1. If a player's store has the the majority of available seeds, that player has won the game.  
2. If all of a player's pits are empty, the opponent moves all of seeds in their pits into their own store and the game is over. Whoever has the most seeds wins (a tie is possible).  