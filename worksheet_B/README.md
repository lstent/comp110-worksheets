Display start screen
When player presses power initiate game
Set correct word, add 11 incorrect words and 5> 11< symbol chains
Symbol chain is radomly set to dud or extra attempts
Set Player attempts left to 4

Loop until winning screen or player attempts = 0
  When player selects word
    If word is correct go to winning screen
    Else -1 attempts
  When player selects symbol chain
    If chain is dud delete the chain and an uncorrect word if word hasn't been selected already
    Else chain is deleted and attempts reset to 4
When player attempts = 0 display looser screen
