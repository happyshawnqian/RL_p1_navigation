[//]: # (Image References)

[image1]: https://user-images.githubusercontent.com/10624937/42135619-d90f2f28-7d12-11e8-8823-82b970a54d7e.gif "Trained Agent"

# Project 1: Navigation
### Project Details
In this project, an agent is trained to navigate and collect bananas in a large, square world. A reward of +1 is obtained after collecting a yellow banana, while a reward of -1 is incurred for collecting a blue banana.
![Trained Agent][image1]
The state space consists of 37 dimensions containing  the agent's velocity and ray-based perception of objects around agent's forward direction. The agent's four discrete actions are:
- **`0`** - move forward.
- **`1`** - move backward.
- **`2`** - turn left.
- **`3`** - turn right.

The task is episodic. An average score of +13 at least must be obtained over 100 consecutive episodes in order to solve the environment.

### Getting Started
1. I am using Windows 10. First, create a `python = 3.6` environment following the Dependencies part described in [this link](https://github.com/udacity/deep-reinforcement-learning/blob/master/README.md).
2. During Step 1 creating the environment, when installing torch=0.4.0 according to the requirements.txt in `python/` folder, I was encountered a problem which can be solved following [this link](https://github.com/udacity/deep-reinforcement-learning/issues/13).
3. Download the `unityagents` dependency according to the Getting Started part stated in [this link](https://github.com/udacity/deep-reinforcement-learning/blob/master/p1_navigation/README.md).

### Instructions
Run the cells in `Navigation.ipynb` to train the agent.

### Result
The environment can be solved in 500 episodes.

### Repo Anatomy
- **Banana_Windows_x86_64/**: directory storing the Unity environment
- **Navigation.ipynb**: notebook to train the agent
- **model.py**: neural network mapping the state to the action values
- **dqn_agent.py**: the agent that interacts with environment and implements Q-Learning
- **checkpoint.pth**: the weights of the trained neural network
- **Report.pdf**: report for the project