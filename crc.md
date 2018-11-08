class Dice
    - Gives number from 1 - 6
        - Collaborator: game

class Player
    - Roll
    - Hold
    - Track total score
        - Collaborator: game, dice

class Computer
    - Hit until current round score is += 20
    - Track total score
        - Collaborator: dice, game

class Game
    - Choose first player
    - Play round with Player 1
    - Play round with Player 2
    - Play until score = 100
    
    Round
    - Roll dice
    - Choose to hold
        - If choose to hold, keep points
    - Get a 1, lose points
    - Display total score
        - Collaborator: player, computer, dice
