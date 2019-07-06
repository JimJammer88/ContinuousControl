### Report - Continuous Control with Deep Deterministic Policy Gradients

The work desribed in this report was completed as part of the submission for the Deep Reinforcement Learning nanodegree by Udacity.


#Introduction


#Implementation Details

HyperParameter | Description | Value
------------ | ------------- | -------------  
BUFFER_SIZE | Size of the Replay buffer| 2e5
BATCH_SIZE | Size of each minibatch for gradient update| 1024
GAMMA| The discounting factor| 0.99
TAU | Soft update parameter| 1e^-3
LR_ACTOR | Learning rate of the actor | 1e^-4
LR_CRITIC | Learning rate of the critic | 1e^-4
N_TIMESTEP | Number of timesteps between learning from experiences | 20
N_GRAD_UPDATE| Number of updates performed every N_TIMESTEPS | 10
MU | Drift parameter of the OU process used to add noise to the actions | 0
THETA | Speed paramaeter of the OU process used to add noise to the actions | 0.15
SIGMA | Volatility parameter of the OU procc used to add noise to the actions | 0.2
