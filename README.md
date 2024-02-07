## Overview
### Introduction
Artificial intelligence (AI) development has been increasing significantly in recent years, driven 
by advances in machine learning algorithms and hardware capabilities. While there are many 
different possible applications for AI, our team is particularly interested in implementing it in 
soccer. Sport is an important part of human culture, where we learn to test our physical limits and 
work as a team.

In soccer, the arrangement of 11 players on the field, known as the formation, is developed over 
years of playing and practicing. Formations like 4-4-2 (4 defenders, 4 midfielders, and 2 forwards) 
and 4-3-3 are chosen based on a team's strengths, weaknesses, and tactical objectives, as well as 
the strengths and weaknesses of their opponent. Deciding on the best strategy for each game is 
extremely challenging for coaches, as there is no formula for success. However, with machine 
learning, AI could teach themselves to play soccer. We believe that in future AI with machine 
learning configured with data on a team's and its opponents' strengths and weaknesses could 
provide effective statistical assistance to coaches by running thousands or even millions of 
simulated matches in the background.

While there is rapid growth in developing AI with different machine learning algorithms in sport. 
In this project we are going to dive into implementing machine learning on robot soccer playing, 
and simulate a real-world competitive soccer match.

### Objective
The main task of the project is to design and develop an AI self-teaching robot that is able to learn 
to play soccer in a virtual environment, and to create a virtual environment for training and 
simulation that accurately replicates the rules and dynamics of a real-world soccer match. To train 
the AI self-teaching robot using reinforcement learning or another suitable machine learning 
algorithm. lastly to enable the AI self-teaching robot to work as a team with other robots to simulate 
a competitive soccer match in the virtual environment.

While the sub task is to identify the most effective training method by experimenting with different 
algorithms and settings, based on the performance of the robots in the virtual environment. and to 
demonstrate the capabilities of the AI self-teaching robot and the effectiveness of the training 
method through simulations of real-world soccer matches in the virtual environment

### Proposed Solution
Our proposed solution for a robot in a soccer game is to use visual feedback and planning and 
control systems to enable the robot to interact with and understand its environment, additionally a 
virtual physical environment to allow them to perform visual soccer matches.

The visual feedback system for our robot will use image processing and classification for visual 
navigation, allowing the robot to avoid obstacles and stay within bounds. It will also use object 
detection to recognize and track objects such as the ball, teammates, and opponents, enabling the 
robot to perform tasks related to these objects. Additionally, we will use localization and Kalman 
filter to determine the position of objects and estimate the robot's location in the map over time.
To enable the robot to make decisions and take actions based on the data provided by the visual 
feedback system, we will need to use path planning and motion control methods. To perform self teaching tasks, our proposed method is to use machine learning to train the robot to make decisions 
and take actions based on data, additionally reinforcement learning algorithms to adapt to changing 
environments and goals.

To perform a soccer match simulation, we will need to build a virtual physical environment and 
model. The environment should include models of a soccer pitch with two goals at each end, 
football and the soccer playing robot. In addition, to build the intelligent systems and behaviors 
for the players into the simulation, we will need an AI platform with AI-related features and tools. 
This platform should provide tools for developing and training the robot, as well as features for 
building and running simulations.

By combining the above approaches, our proposed solution will enable a robot to navigate and 
interact with its environment effectively in a soccer game, allowing it to perform training in 
simulation to achieve its goals.

**Assumption**

The following assumptions have been made in order to simplify the model and make it more 
manageable:
- The player and the ball are rigid bodies.
- The sense of vision and hearing is simulated by rays emitting from the body.
- The player and ball motion and movement is limited to forward, backward, and 
rotation only, and is constrained to a 2D horizontal plane.
- No offside, penalties or concern 
- There are walls to limit the ball and robot to stay in the field
- There is no effect of wind or air resistance in the environment.
  
Additionally, we assume that the project has the necessary resources and computer power to 
develop the AI self-teaching robot and create the virtual environment for training and simulation. 

**Basic simulation platform**

Throughout the design process, we have identified an open-source project called ML-Agents[1] as 
a suitable starting point for our soccer project, which uses reinforcement learning algorithms to 
achieve self-teaching soccer playing. The project utilizes the Unity game engine to create a visual 
simulation and the Unity ML-Agents toolkit and PyTorch library to develop the model and 
reinforcement learning algorithm. 
We believe that this existing project, which provides a basic 2v2 soccer game, is well-suited to our 
needs and can serve as the foundation for our goal. Our approach involves building upon this 2v2 
learning environment and experimenting with our own learning algorithms, with the ultimate goal 
of expanding the game to a more complex 5v5 model featuring two teams of 5 robots trained by 
different algorithms, In addition, we plan to enhance the performance of the robots by assigning 
them positions such as goalie, attacker, and defender
