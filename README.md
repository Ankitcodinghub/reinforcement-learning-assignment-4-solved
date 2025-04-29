# reinforcement-learning-assignment-4-solved
**TO GET THIS SOLUTION VISIT:** [Reinforcement Learning Assignment 4 Solved](https://www.ankitcodinghub.com/product/reinforcement-learning-assignment-4-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;115759&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;Reinforcement Learning Assignment 4 Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
1 Introduction

The goal of this assignment is to do experiment with deep Q network (DQN), which combines the advantage of Q-learning and the neural network. In classical Q-learning methods, the action value function Q is intractable with the increase of state space and action space. DQN introduces the success of deep learning and has achieved a super-human level of play in atari games. Your goal is to implement the DQN algorithm and its improved algorithm and play with them in some classical RL control scenarios.

2 Deep Q-learning

Algorithm 1: deep Q-learning with experience replay. Initialize replay memory D to capacity N

Initialize action-value function Q with random weights h

Initialize target action-value function Q^ with weights h25h

For episode 5 1, M do

Initialize sequence s1~f gx1 and preprocessed sequence w1~wð Þs1

For t5 1,T do

With probability e select a random action at otherwise select at~argmaxaQðwð Þst ,a;hÞ

Execute action at in emulator and observe reward rt and image xt11

Set stz1~st,at,xtz1 and preprocess wtz1~wðstz1Þ

Store transition wt,at,rt,wtz1 in D

Sample random minibatch of transitions wj,aj,rj,wjz1 from D

rj if episode terminates at step jz1 Setyj~rjzc maxa0 Q^ wjz1,a0;h{ otherwise

2

Perform a gradient descent step on yj{Q wj,aj;h with respect to the network parameters h

Every C steps reset Q^~Q

End For

End For

Figure 1: Deep Q-learning with experience replay

You can refer to the original paper for the details of the DQN. “Human-level control through deep reinforcement learning.” Nature 518.7540 (2015): 529.

3 Experiment Description

• Programming language: python3

• You should compare the performance of DQN and one kind of improved DQN and test them in a classical RL control environment–MountainCar.

OPENAI gym provides this environment, which is implemented with python (https://gym.openai.com/envs/MountainCar-v0/). What’s more, gym also provides other more complex environment like atari games and mujoco.

Since the state is abstracted into car’s position, convolutional layer is not necessary in our experiment. You can get started with OPENAI gym refer to this link (https://gym.openai.com/docs/). Note that it is suggested to implement your neural network on the Tensorflow or Pytorch.

4 Report and Submission

• Your report and source code should be compressed and named after “studentID+name+assignment4”.
