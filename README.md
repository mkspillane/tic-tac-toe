# tic-tac-toe

Using reiforcment learning a feed forward network is trained to play tic-tac-toe.  After ~40 games the policy network
without rollouts wins 90% of the time.

![alt text](https://github.com/mkspillane/tic-tac-toe/edit/master/results.png)


The files used to do this are:
'defs_ttt.ipynb' which contains the functions that perform the rollouts for each move in training.  There are 2 rollouts
one which erases information from the previous move and another which stores previous rollouts for use in the next turn.  It also has a function to test the current model against a random player

'ttt_final.ipynb' which implements training using the second rollout method.  It records the results against random play for after each training.  It augments the data with the full dihedral symmetry group for tic-tac-toe.
