# tic-tac-toe

Using reiforcment learning a feed forward network is trained to play tic-tac-toe.  After ~40 games the policy network
without rollouts wins 90% of the time as player 1 and 50% of the time as player 2. 

The files used to do this are:
'defs' which contains the functions that perform the rollouts for each move in training.  There are 2 rollouts
one which erases information from the previous move and another which stores previous rollouts for use in the next turn.

'alpha_ttt' which implements training using the first rollout method

'alpha_ttt_2' which implements training using the second rollout method
