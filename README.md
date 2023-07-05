# recurrent-visual-attention
Based on https://github.com/kevinzakka/recurrent-visual-attention, tried the following enhancements.
1. Allow grad to flow into h_t from both baseline and RL loss
2. Reward for each time step based on cross-entropy classfication loss

There are three training signal for this problem:
1. RL singal into the policy(a|s), trained with REINFORCE type objective
2. MSE Loss for the value function V(S) approximation
3. The classification loss used as reward for RL. The unique aspect is that since we are training the classifier at the same time. Our reward function changes as we train, which complicates training
