# fabulae

Text-based game engine, games are made by creating folders and text files, without having to program.

![screenshot](http://backdaniel.com/img/screenshot/fabulae.png)

## Usage

`./fabulae directory` where `directory` is the game directory.

Try the included tutorial `./fabulae tutorial`.

## Making a game

A fabulae game has a predefined structure.

```
 game/
 ├── dialog.txt
 ├── command1/
 ├── command2/
 ├── command3/
 └── command4/
 ...
```

The name of the game is the same as the name of the game directory, inside there should be one `dialog.txt` file containing the first dialog.

Each of the subfolders will become commands for the current dialog.

```
 game/
 └── command1/
     ├── dialog.txt
     ├── command1/
     └── command2/
     ...
 ...
```

Every command follows the same file structure and has its own dialog and commands. If the player gets to a folder without commands the game ends.
