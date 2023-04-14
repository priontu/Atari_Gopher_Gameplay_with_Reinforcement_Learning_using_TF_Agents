# Atari_Gopher_Gameplay_with_Reinforcement_Learning_using_TF_Agents

In this project, we implement Reinforcement Learning to develop an Agent that teaches itself to play the Atari Game called Gopher. The project was developed using tensorflow, TF-Agents and OpenAI Gym.

Reinforcement learning (RL) is the area of machine learning concerned with intelligent agents that take actions in an environment in order to maximize the notion of cumulative reward.

For this project, we use the OpenAI Gym Atari environment, and we train an agent to play efficiently in this environment. The goal is to develop an agent that can exercise Human-Level Control.

The model consists of the following components:

**Agent** -- The agent is the decision-maker (bot) that interacts with the environment and learns the decisions that maximize the rewards.

**Environment** -- The environment is the space with which the agent interacts to obtain the rewards. 

**Observation space** -- This is the current state of the environment that the agent observes.

**Action space** -- This is the decision that the robot takes at each step.

**Reward** -- In this case, the score of the game, that the agent will try to maximize.

**Policy** -- A policy defines the learning agent's way of behaving at a given time. It is a mapping from perceived states of the environment to actions to be taken when in those states.

Agent's Gameplay before training (around 10-40 iterations):

![myAgentPlays_12](https://user-images.githubusercontent.com/61733487/208231015-f903159d-8aad-4fba-a4bf-f6006ea25c04.gif)

At this point the agent doesn't know much. It's trying different things and learning what works, and which actions lets it earn some rewards.

Agent's Gameplay mid-training (near 30,000 iterations):

![myAgentPlays_14 (2)](https://user-images.githubusercontent.com/61733487/208232117-5940b71a-59e6-4d17-9ba9-24d1f3875b23.gif)

The agent learned some new things -- now it knows it can earn some rewards by filling in some openings.

Agent's Gameplay after training (over 300,000 iterations):

![myAgentPlays_10](https://user-images.githubusercontent.com/61733487/208230897-9ff2efbd-7a7e-4844-aad4-29231ab353c4.gif)

At this point in the training, we have reached Human-Level Control in the Gameplay.

We can see that the Gameplay has improved. The agent has learned that it needs to protect the carrots in order to stay alive, which will let it get more rewards. Furthermore, it has discovered that rewards are earned by filling holes and greater rewards are earned by catching the Gophers. Consequently, the farmer tries to wait for the Gopher at one opening and fills all the others. Other times, it waits for a Gopher to run to the carrots from the other side and then rushes over to catch it when the Gopher is above ground. This level of strategizing is only witnessed in human gameplay.

Google Cloud Machine Configuration:

![image](https://user-images.githubusercontent.com/61733487/232129285-3307c6d3-fc24-43d1-a22b-60fd165a9404.png)

References:

[1] https://www.nature.com/articles/nature14236

[2] Hands-On Machine Learning with Scikit-Learn and TensorFlow, by Aurélien Géron
