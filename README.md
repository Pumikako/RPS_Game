# Rock Paper Scissors

A Python bootcamp mini project: a text-based Rock Paper Scissors tournament played against the computer in a Jupyter notebook.

## Rules

- Choose `rock`, `paper`, or `scissors`.
- The computer randomly selects its move.
- Rock beats scissors, scissors beat paper, and paper beats rock.
- The first side to win three rounds wins the tournament.
- Ties award no points; another round follows.
- Enter `x` and press Enter at a move prompt to leave the game. This also works when retrying an invalid move.

## Features

- Input validation, ignoring capitalization and surrounding spaces.
- Round numbers, player and computer moves, and tournament scores.
- ASCII drawings for all nine matchups, displayed line by line with a short delay.
- Win and lose conditions, plus final scores.
- State reset when a new tournament starts.

## Requirements

- Python 3.
- Jupyter Notebook, JupyterLab, or Visual Studio Code with the Python and Jupyter extensions and a configured Python kernel.

The game uses Python's standard-library modules `random` and `time`; it needs no additional game libraries.

## How to play

1. Open `main.ipynb` and select a Python kernel.
2. Execute the setup and function-definition cells in order, above the game-launch cell.
3. Run one cell containing `play_game()` to start a tournament.
4. Enter your move in the input field and press Enter.
5. Run the launch cell again to start a fresh tournament.

Avoid running every launch cell consecutively if the notebook contains multiple examples of `play_game()`.

## Code organization

The project keeps its data and functions in one notebook:

- `choices`: available moves.
- `game_stats`: current round, player wins, computer wins, and game-over status.
- `animations`: ASCII drawings indexed by matchup.
- `reset_game()`: restores the initial state.
- `player_choice()` and `computer_choice()`: obtain the moves.
- `comparing_moves()`: determines the round result and displays its drawing.
- `game_state()`: updates scores and advances the round.
- `game_over()`: checks whether either side has reached three wins.
- `display_status()` and `show_animation()`: display game information.
- `play_game()`: connects the functions and runs the tournament.

## Current scope

The supported entry point is `play_game()`, which runs the tournament. The menu and separate game modes are work in progress. The current `single_game()` implementation also repeats rounds until three wins; it does not yet provide a one-round match.

## Project files

- `main.ipynb`: the game notebook described here.
- `README.md`: rules, setup instructions, and project overview.

This project practices lists, dictionaries, functions, conditionals, `while` and `for` loops, modules, input validation, and documentation.
