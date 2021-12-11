# UCSD FA21 CSE291(5) Deep RL Course Project

The code is based on [Adversarial Policies: Attacking Deep Reinforcement Learning](https://arxiv.org/abs/1905.10615) and [adversarial-policies](https://github.com/HumanCompatibleAI/adversarial-policies).
An off-the-shelf development environment has been build at docker image xuanchenlu/cse291:latest

To reproduce the results:
1. Setup the docker image on DSMLP 
2. Check out correct branch to reproduce
3. An example of training command is ``python -m aprl.train with env_name=multicomp/SumoHumans-v0 paper seed=[seed] num_env=[num] total_timesteps=40000000``, which will automatically use the reward design in the branch.
4. An example of evalution command is ``python -m aprl.score_agent with env_name=multicomp/SumoHumans-v0 agent_b_type=ppo2 agent_b_path=[path_to_weight] render=True``
5. Please refer to code for detailed usage of training and scoring. 
