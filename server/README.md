# noflappybird

## Input

1. Name/end/start
  * string

2. Settings
  * set
  * value

3. Mouse
  * vertical position 0% - 100%

4. Special
  * On/Off

## Output

1. Id
  * YourId

2. Names
  * array
    * id
    * name

3. Dead
  * Final score

4. Leaderboard
  * array
    * id
    * place
    * score

5. pipe
  * x
  * y

6. Bird
  * array
    * id
    * x
    * y

## Server Loop

1. loop birds
  * update position
  * check pipe collision

2. loop players
  * send birds within proximity of player
  * send pipe if pipes sent < pipes completed + 2
  * 1/s send Leaderboard + your score
