# fabulae

Simple text-based game engine, games are made by creating folders and files, without having to program.

## Usage

`./fabulae directory` where `directory` is the game directory.

Try the included tutorial `./fabulae games/tutorial`.

## Making a game

A fabulae game has a predefined structure.

```
 game/
 ├── main.txt
 ├── command1/
 ├── command2/
 ├── command3/
 └── command4/
 ...
```

The name of the game is the same as the name of the game directory, inside there should be one `main.txt` file containing the first dialogue.

Each of the subfolders will be interpreted as commands for the current dialogue.

```
 game/
 └── command1/
     ├── main.txt
     ├── command1/
     └── command2/
 ...
```

Every command follows the same file structure and has its own dialogue and commands. If the player gets to a folder without commands the game ends.
