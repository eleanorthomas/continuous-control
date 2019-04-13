### Report for Project 2 - Continuous Control

## Learning Algorithm

The learning algorithm used was a Deep Deterministic Policy Gradient (DDPG) using an Actor-Critic model with underlying neural networks, each using two fully connected layers, with 256 and 128 units for the first and second layer, respectively, and relu activation functions.

The hyperparameters used to train the agent were as follows:
- BUFFER_SIZE = int(1e5)  (replay buffer size)
- BATCH_SIZE = 1280       (minibatch size)
- GAMMA = 0.99            (discount factor)
- TAU = 1e-3              (for soft update of target parameters)
- LR_ACTOR = 1e-4         (learning rate of the actor)
- LR_CRITIC = 1e-3        (learning rate of the critic)
- WEIGHT_DECAY = 0        (L2 weight decay)

## Plot of Rewards

The following is a plot of the rewards for the trained agent showing the X episodes it took to solve the problem. Over the last X episodes, the average score was X:

![alt text](plot_of_rewards.png "Plot of Rewards")

## Ideas for Future Work

The initial implementation took substantial time to solve the task. Further optimization of hyperparameters could result in a quicker solution. This solution could also be extended to the multi-agent task, and was ultimately adapted as a starting place for the Collaboration and Competition task.


