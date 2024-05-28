# Skid Isolation Game AI 🎮

## Introduction 🌟

Skid Isolation is a two-player turn-based game played on a 7-by-7 grid. Each player has a piece that moves like a queen in chess, and after each move, the squares traversed are blocked, becoming unusable for the rest of the game. The objective is to force the opponent into a position where they cannot make a move.

This project aims to develop an AI agent capable of playing Skid Isolation optimally, using search algorithms and heuristics to determine the best moves.

## Goals 🎯

The primary goal of this project is to develop an AI agent that:

    Implements efficient search algorithms to explore game states.
    Uses a heuristic function to evaluate game positions.
    Applies strategies like minimax with alpha-beta pruning to make optimal moves.
    Operates within a reasonable time frame, ensuring moves are made within 2 seconds.

## Work Done 🛠️

### Search Algorithms

    Minimax Algorithm: The AI evaluates possible game states by considering all feasible moves for both players, aiming to determine the optimal strategy.
    Alpha-Beta Pruning: Enhances the minimax algorithm by eliminating branches that do not affect the final decision, reducing computational overhead.

### Heuristic Function

A heuristic function evaluates the desirability of game states based on:

    The number of available moves for the player.
    The number of available moves for the opponent.

This function helps the AI make informed decisions at each move.

### Iterative Deepening

    Iterative Deepening: The AI incrementally increases the depth of its search until the time limit is reached, allowing for effective time management and thorough exploration of game states.

## Results 📊

The AI agent was tested against other agents with varying strategies and search depths. Key outcomes include:

    Performance: The AI completed moves within 2 seconds.
    Effectiveness: It defeated other agents, which searched the game tree up to 8 moves deep, more than 70% of the time.
    Potential Improvements: The performance could be enhanced by incorporating a specialized dictionary for endgame and opening states, though the current approach avoids storing game states in memory.

## How to Run the Game 🕹️

`git clone (https://github.com/bhushanap/gameAI_Isolation)`

Play the Game: Open isolation.html in a Javascript compatible browser to start playing Skid Isolation.

## Usage 📝

Grid size:
    `What should the size of the square grid be?`
Search tree nodes:
    `How deep should the search tree before AI makes a move. Larger numbers will make the computer slow but will result in a more competitive opponent.`
v/s AI or player?:
    ```AI: Choose to play against the AI agent and see if you can outmaneuver it.
    Player: Two human players compete to win.```
AI to go first?:
    ```AI first: If AI should make the first move
    AI second: If human player should make the first move```


## Contributing 🤝

Feel free to fork this repository, submit issues, and send pull requests. Contributions are welcome to improve the AI's strategy, performance, and overall game experience.
