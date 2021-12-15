# RL-Brain-Trajectories

Using reinforcement learning to model optimal brain state trajectories. Inspired by [Gu et al. (2017)](https://pubmed.ncbi.nlm.nih.gov/28088484/).

## Description

The complex architecture of the human brain allows us to transition among a wide array of brain states. Network control theory remains a state-of-the-art method to investigate optimal brain state transitions. Given a network of brain regions and knowledge of the network’s structural landscape, one can mathematically model patterns of inter-region activity propagated along anatomically defined edges. Inherent to this approach is the choice of controllable region sets, as collective control of these regions is used to drive desired brain state transitions, i.e., from rest to task-evoked states. As reinforcement learning (RL) and control theory are closely intertwined, an RL framework was constructed to encapsulate the problem of choosing the best set of control actions to drive regional dynamics from an initial state to a target state. Using an actor-critic algorithm, the agents’ actions were modeled as inputs to control regions and the environment was defined by rewarding the achievement of states closer to the target state, and penalizing unnecessarily expensive actions. Simulated brain states from the model were compared with trajectories with data from the Human Connectome Project. By comparing the simulated trajectories with the time series from the HCP task data, insights were gained on how brain states transition during a motor task.

## Acknowledgments

* [PyTorch-ActorCriticRL](https://github.com/vy007vikas/PyTorch-ActorCriticRL)
* [NOCAD](https://github.com/abonyilab/NOCAD)
* [NMA HCP processing code](https://colab.research.google.com/github/NeuromatchAcademy/course-content/blob/master/projects/fMRI/load_hcp_task_with_behaviour.ipynb)
