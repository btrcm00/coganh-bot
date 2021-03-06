## CO GANH with alpha-beta prunning

### Rule

- Each player has 8 chips either blue (1) or red (-1) that set up as shown below.

```
    [[-1,-1,-1,-1,-1],
    [-1, 0, 0, 0,-1],
    [ 1, 0, 0, 0,-1],
    [ 1, 0, 0, 0, 1],
    [ 1, 1, 1, 1, 1]]
```

- Players take turn to move their chips along any segments to the next empty intersection. A player who turns all other chips to his/her color wins. There are two ways to change the color of chips.

  - Turn: If a blue chip moves to an intersection with two red chips in both ends (see Fig. 1a), then the red chips are turned in blue (see Fig 1b). The red player uses the same rule to turn blue chips to red.
    ![1a](https://cdn.tgdd.vn//GameApp/1323649//Untitled-26-800x557.jpg)
    ![1b](https://cdn.tgdd.vn//GameApp/1323649//Untitled-27-800x558.jpg)
  - Dead End: When any chips are surround with the other color chips and they cannot move, they have to turn to the other color. In Fig. 2a, when chip B moves in the direction of the green arrow, A and C have to turn into red.
    ![2a](https://cdn.tgdd.vn//GameApp/1323649//chet-800x516.jpg)
    ![2b](https://cdn.tgdd.vn//GameApp/1323649//chet2-800x616.jpg)
  - Traps: A player can set up a trap to force the opponent moving chips that can advance in the game. - In leftmost figure , when the blue player says “Open” and move chip N to the green arrow direction, then the red player has to move chip M between E and N (see middle) and turn them into red (see rightmost fig). Players can move a chip to any direction to open the trap. The opponent has to move into the open position.
    ![traps1](https://cdn.tgdd.vn//GameApp/1323649//cui-800x243.jpg) - Now the blue player will move chip O into the intersection to turn three pairs A-N, K-M, and L-E to blue. Players can use this trap to change color of one, two or three pairs. It’s rare but sometime with a dead end position eight chips could be changes to the other color. Setting a trap also helps to get out a corner position. The game ends when all chips are the same color.
    ![traps2](https://cdn.tgdd.vn//GameApp/1323649//cui2-800x271.jpg)

- [More](https://www.thegioididong.com/game-app/huong-dan-cach-choi-co-ganh-co-chem-luat-choi-co-dan-gian-don-1323649)

### Play with bot

- Clone this repository and unzip.
- Type `python gameplay.py`
