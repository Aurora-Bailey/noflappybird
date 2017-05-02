# noflappybird

## Input

Name/end/start
  string

Mouse
  vertical position 0% - 100%

Special
  On/Off

## Output

Id
  YourId

Names
  array
    id
    name

Leaderboard
  array
    id
    place
    score

pipe
  x
  y

Bird
  array
    id
    x
    y

## Server Loop

loop birds
  update position
  check pipe collision

loop players
  send birds within proximity of player
  send pipe if pipes sent < pipes completed + 2
