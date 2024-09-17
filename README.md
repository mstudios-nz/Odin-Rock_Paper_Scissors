# Odin-Rock_Paper_Scissors

JS Project to create a game:


GET HUMAN CHOICE
- declare a function getHumanChoice
      INPUT - use prompt method to get user input to type input rock, paper or scissors
      FUNCTION  - convert input to all lowercase (for consistency of reading)
      OUTPUT - user entry in lowercase  NB: ENTRY COULD BE INVALID AT THIS POINT (i.e. wrong word, or misspelled)


GET COMPUTER CHOICE
- declare a function getComputerChoice
    INPUT - use Math.random to generate a random number >=0, <1
    FUNCTION - if   input >=0 & < 0.33        = rock 
             - else if  input >=0.33 & <0.66  = paper   
             - else if  input >=0.66 & <1     = scissors
    OUTPUT - random computer choice in lowercase

DECLARE SCORES
- declare global variables: - humanScore
                            - computerScore
  - Initialise values to 0 
  

LOGIC - PLAY ROUND
- delcare a function playRound - to play one round of game, output message, and add score to scoreboard
    INPUT - Declare Variables - humanChoice = output of function getHumanChoice
                              - computerChoice = output of function getComputerChoice
    FUNCTION - switch: case a) humanChoice = rock  - if computerChoice = rock - result "Tie" 
                                                   - if computerChoice = paper - result "You Lose" (computerScore increment 1)
                                                   -if computerChoice = scissors - result "You Win" (humanScore increment 1)
                       case b) humanChoice = paper  (if statement per above)
                       case c) humanChoice = scissors  (if statement per above)
                       default : result "invalid entry please try again"
    OUTPUT - Result + score increment
  

LOGIC - PLAY GAME
- declare a function playGame - to play 5 rounds, update scores and declare a winner

  Loop the playRound function 5 times,
  declare highests of humanScore & computerScore wwinner,
  Reset variable values 

