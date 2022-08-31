# Reinforcement Learning and Its Applications

In reinforcement learning (RL), an agent is trained to achieve a goal based on the feedback it receives as it interacts with an environment. It collects a number as a reward for each action it takes. Actions that help the agent achieve its goal are incentivized with higher numbers. Unhelpful actions result in a low reward or no reward.

With a learning objective of maximizing total cumulative reward, over time, the agent learns, through trial and error, to map gainful actions to situations. The better trained the agent, the more efficiently it chooses actions that accomplish its goal.

Playing games:

Go (board game) was mastered by the AlphaGo Zero software.
Atari classic video games are commonly used as a learning tool for creating and testing RL software.
StarCraft II, the real-time strategy video game, was mastered by the AlphaStar software.

Video game level design:

Video game level design determines how complex each stage of a game is and directly affects how boring, frustrating, or fun it is to play that game.
Video game companies create an agent that plays the game over and over again to collect data that can be visualized on graphs.
This visual data gives designers a quick way to assess how easy or difficult it is for a player to make progress, which enables them to find that “just right” balance between boredom and frustration faster.

Wind energy optimization:

RL models can also be used to power robotics in physical devices.
When multiple turbines work together in a wind farm, the turbines in the front, which receive the wind first, can cause poor wind conditions for the turbines behind them. This is called wake turbulence and it reduces the amount of energy that is captured and converted into electrical power.
Wind energy organizations around the world use reinforcement learning to test solutions. Their models respond to changing wind conditions by changing the angle of the turbine blades. When the upstream turbines slow down it helps the downstream turbines capture more energy.

Other examples of real-world RL include:

- Industrial robotics
- Fraud detection
- Stock trading
- Autonomous driving

## Agent
The piece of software you are training is called an agent.
It makes decisions in an environment to reach a goal.
In AWS DeepRacer, the agent is the AWS DeepRacer car and its goal is to finish * laps around the track as fast as it can while, in some cases, avoiding obstacles.
## Environment
The environment is the surrounding area within which our agent interacts.
For AWS DeepRacer, this is a track in our simulator or in real life.

## State
The state is defined by the current position within the environment that is visible, or known, to an agent.
In AWS DeepRacer’s case, each state is an image captured by its camera.
The car’s initial state is the starting line of the track and its terminal state is when the car finishes a lap, bumps into an obstacle, or drives off the track.
## Action
For every state, an agent needs to take an action toward achieving its goal.
An AWS DeepRacer car approaching a turn can choose to accelerate or brake and turn left, right, or go straight.
## Reward
Feedback is given to an agent for each action it takes in a given state.
This feedback is a numerical reward.
A reward function is an incentive plan that assigns scores as rewards to different zones on the track.
## Episode
An episode represents a period of trial and error when an agent makes decisions and gets feedback from its environment.
For AWS DeepRacer, an episode begins at the initial state, when the car leaves the starting position, and ends at the terminal state, when it finishes a lap, bumps into an obstacle, or drives off the track.

In a reinforcement learning model, an agent learns in an interactive real-time environment by trial and error using feedback from its own actions. Feedback is given in the form of rewards.
