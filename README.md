# Deep Reinforcement Learning
This module implementes basic deep reinforcement learning algorithms including DDPG[1] and TRPO[2] on a variety of environments, including OpenAI gym envs and a few new envs based on Open Dynamics Engine(ODE). In the case of learning with task contexts, the network takes manually defined or automatically detected feature(from Wave 7) as part of inputs. 
We're working on extending deep reinforcement learning methods to multi-task learning and transfer learning, trying to have learning agent automatically figure out the proper modules of policies for sharing among different tasks, and therefore improve learning performance.

## Prerequisites:
* Python 2.7
* Tensorflow 1.0(with GPU configuration)
* gym
* Scipy, Numpy
* ODE (Optional for ode based environments)

## Algorithms:
* TRPO 
* DDPG
* TODO: other baseline algorithms, including CMA-ES, REINFORCE, etc.
## Environment:
Besides exsiting environments from OpenAI Gym, a few more are implemented based on Open Dynamics Engine(ODE), including cartpole, pendulum, etc.

## Usage:
To run the experiment, simple run the code
    python ddpg_main.py
    python trpo_main.py
Hyperparameters can be tuned in utils/paras.py

## Reference:
[1] Schulman, John, et al. "Trust region policy optimization." Proceedings of the 32nd International Conference on Machine Learning (ICML-15). 2015.
[2] Lillicrap, Timothy P., et al. "Continuous control with deep reinforcement learning." arXiv preprint arXiv:1509.02971 (2015).
