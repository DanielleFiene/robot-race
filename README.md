# Robot Race
## Overview

This script simulates a robot race through a maze. It reads maze data from a CSV file, initializes the robots, and processes their movements until the race ends or the maximum number of turns is reached. It tracks each robot's moves and collisions, then outputs the results.

## Requirements

- Python 3.x
- `robot_race_functions` module (which should include functions like `read_maze`, `print_maze`, `process_maze_init`, `compute_robot_logic`, `is_race_over`, `update_maze_characters`, and `print_results`).

## How It Works

1. **Initialize the Maze and Robots**
   - Reads maze data from `maze_data_1.csv`.
   - Prints the initial maze.
   - Processes the maze to identify walls, goals, and robots.

2. **Robot Movement Simulation**
   - Iterates through turns (up to `max_turns` or until the race is over).
   - For each robot, computes its next move and appends it to the `robot_moves` deque.
   - Updates the maze and prints it after each move.

3. **Results Calculation**
   - Counts the number of moves and collisions for each robot.
   - Calculates the final scores for each robot.
   - Prints the final results.

## Parameters

- `maze_file_name`: Path to the CSV file containing the maze data.
- `seconds_between_turns`: Time interval (in seconds) between robot turns.
- `max_turns`: Maximum number of turns before the race ends.

## Execution

To run the script, ensure you have the `robot_race_functions` module and the maze data CSV file in the correct path. Simply execute the script using Python:

```bash
python robot_race.py
```

## License
