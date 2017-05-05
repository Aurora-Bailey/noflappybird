# noflappybird

## Input

1. Name/start
    * name [string]

2. Settings
    * setting [int]
    * value [int]

3. Mouse
    * vertical position [int]

4. Special
    * on/off [int]

## Output

1. Id
    * your id [int]

2. Names
    * array [arr]
       * id [int]
       * name [string]

3. Dead
    * final score [int]

4. PastPipe
    * pipe number [int]

5. Leaderboard
    * array [arr]
       * id [int]
       * place [int]
       * score [int]

6. pipe
    * type [int]
    * x [int]
    * y [int]

7. Bird
    * array [arr]
       * id [int]
       * x [int]
       * y [int]

## Server Loop

1. loop birds
    * update position
    * check pipe collision

2. loop players
    * send birds within proximity of player
    * send pipe if pipes sent < pipes completed + 2
    * 1/s send Leaderboard + your score
