# Project Details

The agent is a double-jointed arm. The goal is to move to a target location.

States: 33
Actions: 4 (torque applicable to two joints)
Rewards: +0.04 for each step that the agent's hand moves toward the goal location

# Getting Started

Open ContinuousControl.ipynb Jupyter notebook, it also contains a section on how to install the necessary dependencies.

Download the Reacher environment (binary file) for your operating system and configure file_name variable (in ContinuousControl.ipynb Jupyter notebook) to point to the location of the binary file.

* Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
* Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
* Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
* Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

# Instructions

Open ContinuousControl.ipynb Jupyter notebook and execute each code block to train the agent using DDPG.
