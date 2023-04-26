# Smart Pong Player
Here lies a smart pong player agent made in Python and trained during more than 24 hours on more than 5000 games. It's a Reiforment Learning agent made based on the Policy Gradient algorithm. The whole process is also explained in this [blog](http://karpathy.github.io/2016/05/31/rl/). Feel free to look at it to understand more about the process.

# How to make it work ?

## Get the Requirements
- Let's start by... Installing Python. In case you haven't seen it yet, this repository is made in python.
- After that, you can clone this repository.

      git clone name
    
- Now go to the directory of your local repo and run this command in your teminal

      python -m pip install -r requirements.txt

You are now ready to enjoy your Smart Agent

## Enjoy your smart player
The main goal of the repository is to showcase how the agent is made. We've also included a main function to train and test you own agent. And if you don't have time to go through all this training stuff, you can just use our pre-made agent whose brain is save in a `.pkl` file. So you're free to use the Agent code or if you're there for examination, you'll be more interested in the demo, so just run the main program.

### Using the Agent in your own logic
All the agent workflow is detailed in the main function it's clear enough to understand.

### Training existing agent with the program
    python main.py -t [nbr-ep] path/to/the/agent/brain
where `nbr_ep` is the number of episodes you want your agent to be trained on, and `path/to/the/agent/brain` is the path to your agent's brain file.

### Evaluate your agent
    python main.py -e [nbr-ep] path/to/the/agent/brain
where `nbr_ep` is the number of episodes you want your agent to be trained on, and `path/to/the/agent/brain` is the path to your agent's brain file.

To do both training and evaluation, you have to add both `-t` and `-e`.
    python main.py -t [nbr-ep] -e [nbr-ep] path/to/the/agent/brain
If no path is specified, the program creates a new model.
