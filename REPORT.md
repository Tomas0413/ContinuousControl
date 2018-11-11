# Learning Algorithm

The algorithm for the agent is [DDPG](https://arxiv.org/pdf/1509.02971.pdf)

* model.py file contains neural network definitions for actor and critic models
* ddpg_agent.py file implements Agent, OUNoise and ReplayBuffer classes
* checkpoint_actor.pth file contains model checkpoint for actor neural network
* checkpoint_critic.pth file contains model checkpoint for critic neural network

Hyperparameters (defined in ddpg_agent.py)

* BUFFER_SIZE = int(1e6)  (replay buffer size)
* BATCH_SIZE = 128        (minibatch size)
* GAMMA = 0.99            (discount factor)
* TAU = 1e-3              (for soft update of target parameters)
* LR_ACTOR = 1e-4         (learning rate of the actor)
* LR_CRITIC = 3e-4        (learning rate of the critic)
* WEIGHT_DECAY = 0.0001   (L2 weight decay)


# Plot of Rewards

# Ideas for Future Work
