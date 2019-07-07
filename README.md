# Continuous Control

Continuous Control assignment for the Deep Reinforcement Learning nanodegree.

This repository contains the code required to train an agent to solve the Multi Agent Reacher Environment provided by Udacity.

The notebook is saved with outputs from the training I have undertaken. The model weights are also stored in the repository.


##  Dependencies 

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:

    - **_Twenty (20) Agents_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Place the file in the main folder of this repository, and unzip (or decompress) the file. 

3. Run `Continuous_Control.ipynb` to  train the agents.

## Files

1. Continuous_control.ipynb Thy ipython notebook loads the environment and controls the training of the agent.

2. multi_agent_benchmark.py This file defines the Agent class for multi-agent training and the Replay Buffer class.

3. model.py The classes Actor and Critic extend PyTorch.NN.Module and defines actor and critic networks respectively.

4. Report.md The project report

5. actor_solved.pth Pickled file created using torch.save(). This stores the model weights of the actor at the point at which the episode is solved.

6. critic_solved.pth Pickled file created using torch.save(). This stores the model weights of the critic at the point at which the episode is solved.

7. actor_final.pth Pickled file created using torch.save(). This stores the model weights of the actor at the point at which training terminates(after 400 episodes).

8. critic_final.pth Pickled file created using torch.save(). This stores the model weights of the critic at the point at which training terminates(after 400 episodes).

9. Run_Trained_Agent.ipynb - Loads the trained actor network and runs the agent in the environment.


