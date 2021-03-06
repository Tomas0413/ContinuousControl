# Learning Algorithm

The algorithm for the agent is [DDPG](https://arxiv.org/pdf/1509.02971.pdf)

* model.py file contains neural network definitions for actor and critic models
* ddpg_agent.py file implements Agent and ReplayBuffer classes
* checkpoint_actor.pth file contains model checkpoint for actor neural network
* checkpoint_critic.pth file contains model checkpoint for critic neural network

Hyperparameters (defined in ddpg_agent.py)

* BUFFER_SIZE = int(1e5)  (replay buffer size)
* BATCH_SIZE = 128        (minibatch size)
* GAMMA = 0.99            (discount factor)
* TAU = 1e-3              (for soft update of target parameters)
* LR_ACTOR = 1e-4         (learning rate of the actor)
* LR_CRITIC = 1e-4        (learning rate of the critic)
* WEIGHT_DECAY = 0        (L2 weight decay)
* UPDATE_EVERY = 1        (how many steps to take before updating target networks)

### Actor neural network

* The Actor neural network consists of three fully connected (FC) layers.
* The input has 33 channels (states)
* The input and output channels between layers are 128
* The output has 4 channels (actions)

### Critic neural network

* The Critic neural network consists of three fully connected (FC) layers.
* The input has 33 channels (states)
* The input and output channels between layers are 128, except the input for the second layer is 128 + 4 (actions) 
* The output has 1 channel

# Plot of Rewards

This chart illustrates the rewards received per episode. We consider the problem solved when the agent reaches at least +30 points over 100 episodes. In our case, it took 345 episodes to achieve this goal.

![Rewards per episode](rewards_per_episode.png)

# Ideas for Future Work

* I would like to use [Tensorboard for PyTorch](https://github.com/lanpa/tensorboardX)
* I would like train an the Version 2 Reacher environment (20 Agents)
* I would like to spend some time and compare the performance of the agent to [Distributed Distributional Deterministic Policy Gradients (D4PG)](https://openreview.net/forum?id=SyZipzbCb) algorithm
* I would like to compare the performance of the algorthm on CPU vs GPU
