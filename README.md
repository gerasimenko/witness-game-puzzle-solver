# Computer Vision Assistant for The Witness Challenge

This program solves, in real time, color puzzles (3-monitor) and triangle puzzles (maze) from The Witness challenge.

# How to Use

I tried to keep it as simple as possible, so there are no dependencies or external libraries—just standard Java library classes.

The program takes two parameters: the folder where Steam saves screenshots for The Witness, and the output folder where solved puzzles will be saved.

While running, it checks every second for a new screenshot. If one is found, it tries to detect and solve the puzzle.

Build:
```
javac Solver.java
```

Run:
```
java -Xss64m -cp . Solver "STEAM\\SCREENSHOT\\DIRECTORY\\" "OUTPUT\\DIRECTORY\\"
```
**Use double backslashes in your paths.**

The program runs in an infinite loop, so stop it manually when you're finished.

When taking a screenshot, try to align your view directly with the puzzle. Avoid top-down views; the puzzle should appear roughly square.

# How It Works

For puzzle detection, I used DFS and basic statistical analysis. 
For solving - backtracking with DFS.

## Solved Puzzle Examples

![Puzzle1](https://i.imgur.com/iniHrKR.png)
![Puzzle2](https://i.imgur.com/lPZyUzU.png)
![Puzzle3](https://i.imgur.com/E8XIJFv.png)
![Puzzle4](https://i.imgur.com/Dwi616Y.png)
![Puzzle5](https://i.imgur.com/Vxj1eH3.png)
![Puzzle6](https://i.imgur.com/n4PK9he.png)

[IMGUR](http://imgur.com/a/FEBQG)
