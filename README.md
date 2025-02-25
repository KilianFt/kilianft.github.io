# Kilian Freitag
I am interest in exploring the intersection of human and machines in various way, mainly from a learning-based perspective. That includes
- Robotics
- Reinforcement Learning
- Interactive Learning
- Human-Computer Interfaces

Currently pursuing a PhD at Chalmers. I am always happy to discuss ideas, reach out at:  
tamino [at] chalmers [dot] se

## Research
### Curriculum learning for complex rewards in RL
We had a mobile robot learning problem where we wanted to optimize several conflicting reward terms at the same time and wanted to investigate if a reward curriculum could help Reinforcement Learning to find better policies. Further, we propose a mechanism to automatically determine when to best switch from one curriculum phase to the next. To better understand the generality of the approach, we test it on a modified version of DeepMind Control Suite with a penalty for large actions. We find that a reward curriculum helps the most when the penalty conflicts with the task objective.  
[[Paper](https://arxiv.org/abs/2410.16790)]

### Interactive training of Human-Computer Interfaces
Human-computer interfaces are traditionally trained by collecting supervised data. We investigated if online learning in interactive settings enhances performance and can help mitigate distributional shift in EMG interfaces. Thus we proposed learning such interfaces in a game setting with iterative RL. In extensive experiments we show that it indeed significantely enhances performance. More details and videos can be found here:  
[[Full Paper](https://arxiv.org/abs/2411.13327)], [[ICML Workshop](https://openreview.net/forum?id=pJv1QJBhiN#all)] [[Project page](https://sites.google.com/view/bionic-limb-rl)]

An extension of this work is LIFT, contrastive Learning Interfaces From Teacher, where we relax the assumption that humans act ideal. In order to do so we formulate pseudo-intent labeling as a Bayesian inference problem which is guided by some optimal "teacher" policy. In simulation we show that this method is much more robust to suboptimal behavior that naive copy-the-teacher training.  
[[Paper](https://openreview.net/forum?id=qmmF8YAr5a)], [[Code](https://github.com/KilianFt/LIFT)]

## Past projects
### Chalmers Formula Student
We build a driverless racing setup from scratch in one year, which was ROS-based with dockerized nodes to simplify depoyment. I mainly focused on the system architecture, path planning and control. Overall, is was quite successful as we reached the 4th position in dynamic events when competing against teams with several years of development. Here an example of our fastest lap:  
{% include youtube.html id="sQ7gVgm-L28" %}

### Human-following mobile robot
The idea of this project was to develop a mobile robot that can follow a human on a construction side as assistant. For this, we developed a setup in ROS where legs are detected with a lidar and a human is detected with a camera. We then fused this information to track a person and follow it. It was part of a bigger project about collaborative robotics and BIM on construction sites.
[[Paper](https://www.mdpi.com/2218-6581/10/1/2)]
