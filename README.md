# MsPacman
by Xue Ben

use DQN model(an end to end CNN + RL agent to play visual games atomatically by computer programes) to play MsPacman-v0 on openAI

# Introduction to DQN:
   Deepmind's paper:Play Atari with Deep Reinforcement Learning 
   (http://xueshu.baidu.com/s?wd=paperuri%3A%28e50b83561733e14302a652eebda5b129%29&filter=sc_long_sign&sc_ks_para=q%3DPlaying%20Atari%20with%20Deep%20Reinforcement%20Learning&sc_us=17723823241248413730&tn=SE_baiduxueshu_c1gjeupa&ie=utf-8)
   
# Introduction to MsPacman:
  Use your agent to eat beans and play against robots(Ghosts), aming at maximize total score.
  During gaming, we only accept graph inputs just like the inputs which human get through eyes.
  https://gym.openai.com/envs/MsPacman-v0
   


# Require moduel:
  tensorflow
  gym
  cv2(from opencv)

1. cut origin shape(210, 160, 3) into (160, 160, 1) through cv2
2. create training network, 3 hidden layers, 2 fully connected layers, with one time max pooling(2x2)
3. train, save results per 100000 timesteps
