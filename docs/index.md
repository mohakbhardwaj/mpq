
<!-- Filler text
 -->
 
## <center> Overview </center>

<p> Model-free Reinforcement Learning (RL) works well when experience can be collected cheaply and model based RL is effective when system dynamics can be modeled accurately. However, both assumptions can be violated in real world problems such as robotics, where querying the system can be expensive and real world dynamics can be difficult to model. In contrast to RL, Model Predictive Control (MPC) algorithms use a simulator to optimize a simple policy class online, constructing a closed-loop controller that can effectively contend with real-world dynamics. MPC performance is usually limited by factors such as model bias and the limited horizon of optimization. In this work, we present a novel theoretical connection between information theoretic MPC and entropy regularized RL and develop a Q-learning algorithm that can leverage biased models. We validate the proposed algorithm on sim-to-sim continuous control tasks and compare it against information theoretic MPC and soft Q-Learning, where we demonstrate faster learning with much fewer system interactions (a few minutes with real system parameters) and better performance compared to MPC and soft Q-Learning even in the presence of sparse rewards </p>



<!-- We present an approach to RL that leverages the complementary properties of model-free reinforcement learning and model-based optimal control. Our proposed method views MPC as a way to simultaneously approximate and optimize a local Q function via simulation, and Q-learning as a way to improve MPC using real-world data. We focus on the paradigm of entropy regularized reinforcement learning where the aim is to learn a stochastic policy that minimizes the cost-to-go as well as KL divergence with respect to a prior policy. This has been explored in RL and Inverse RL for its better sample efficiency and exploratory properties. We discuss how this formulation of reinforcement learning has deep connections to information theoretic stochastic optimal control where the objective is to find control inputs that minimize the cost while staying close to the passive dynamics of the system. This helps in both injecting domain knowledge into the controller as well as mitigating issues caused by over optimizing the biased estimate of the current cost due to model error and the shorter horizon. We explore this connection in depth and derive an infinite horizon information theoretic model predictive control algorithm based on Williams et al. (2017). We test our approach called Model Predictive Q-Learning (MPQ) on simulated continuous control tasks a. </p> -->


## <center> Video of Experiments </center>

<center> <iframe width="640" height="480" src="https://www.youtube.com/embed/OO3obHJEk8w" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> </center>