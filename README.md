# recurrent-visual-attention
Based on https://github.com/kevinzakka/recurrent-visual-attention, tried the following enhancements.
1. Allow grad to flow into h_t from both baseline and RL loss
2. Reward for each time step based on cross-entropy classfication loss
