---
layout: post
title:  "Deepmind's Path to Neuro-inspired General Intelligence"
date:   2019-02-08 18:29:46 -0700
categories: thinking
---

By Jeremy Nixon [[jnixon2@gmail.com](mailto:jnixon2@gmail.com)]. Nov. 2017. Updated June 2018.

  

Overview

1.  Deepmind Paper Framing
    
2.  Deepmind Papers through Framing
    
3.  Current Frontier
    
4.  Examples of Systems Neuroscience Inspiration
    

  
  

Deepmind Papers

  

Categories of the path to date:

  

1.  Transfer Learning
    
2.  Multi-task Learning
    
3.  Tools, Environment & Datasets
    
4.  Intuitive Physics
    
5.  Reinforcement Learning
    

	1.  Model-based RL
	    
	2.  Exploration in RL
	    

7.  Applications
    
8.  Safety
    
9.  Deep Learning
    

1.  RNNs
    
2.  CNNs
    

11.  Generative Models
    
12.  Variational Inference
    
13.  Unsupervised Learning
    
14.  Representation Learning
    
15.  Attention
    
16.  Memory
    
17.  Multi-Agent Systems
    
18.  Imitation Learning
    
19.  Metalearning
    

1.  Neural Programming
    

21.  Evolution
    
22.  Game Theory
    
23.  Natural Language Processing
    
24.  Multi-Modal Learning
    
25.  General Machine Learning
    
26.  Theory
    
27.  Miscellaneous
    
28.  Neuroscience
    

  
Papers:
  
 
1.  Transfer Learning  
[DARLA: Improving Zero-Shot Transfer In Reinforcement Learning](https://arxiv.org/pdf/1707.08475.pdf)  
[PathNet: Evolution Channels Gradient Descent in Super Neural Networks](https://arxiv.org/pdf/1701.08734.pdf)  
[Matching Networks for One Shot Learning](https://arxiv.org/abs/1606.04080)  
[Progressive Neural Networks](https://arxiv.org/pdf/1606.04671.pdf)  
[Sim-to-Real Robot Learning from Pixels with Progressive Nets](https://arxiv.org/pdf/1610.04286.pdf)  
[Successor Features for Transfer in Reinforcement Learning](https://arxiv.org/pdf/1606.05312.pdf)  
2.  Multi-Task Learning  
[Multi-task Self-Supervised Visual Learning](https://arxiv.org/pdf/1708.07860.pdf)  
[The Intentional Unintentional Agent: Learning to Solve Many Continuous Control Tasks Simultaneously](https://arxiv.org/pdf/1707.03300.pdf)  
[Distral: Robust Multitask Reinforcement Learning](https://arxiv.org/pdf/1707.04175.pdf)  
[Emergence of Locomotion Behaviors in Rich Environments](https://arxiv.org/pdf/1707.02286.pdf)  
[Reinforcement Learning with Unsupervised Auxiliary Tasks](https://arxiv.org/pdf/1611.05397.pdf)  
[Learning to Navigate in Complex Environments](https://arxiv.org/pdf/1611.03673.pdf)  
[Learning and Transfer of Modulated Locomotor Controllers](https://arxiv.org/pdf/1610.05182.pdf)  
[Multi-Task Sequence to Sequence Learning](https://arxiv.org/pdf/1511.06114v3.pdf)  
[Learning by Playing - Solving Sparse Reward Tasks from Scratch](https://arxiv.org/abs/1802.10567)  
[Unicorn: Continual Learning with a Universal, Off-policy Agent](https://arxiv.org/abs/1802.08294)  
[Progress & Compress: A Scalable Framework for Continual Learning](https://arxiv.org/abs/1805.06370)  
3.  Tools, Environments, Evaluation & Datasets  
[Starcraft II: A New Challenge for Reinforcement Learning](https://arxiv.org/pdf/1708.04782.pdf)  
[DeepMind Lab](https://arxiv.org/pdf/1612.03801.pdf)  
[The Kinetics Human Action Video Dataset](https://arxiv.org/pdf/1705.06950.pdf)  
[An approximation of the Universal Intelligence Measure](https://arxiv.org/pdf/1109.5951v2.pdf)  
[Psychlab: A Psychology Laboratory for Deep Reinforcement Learning](https://arxiv.org/abs/1801.08116)  
[Deepmind Control Suite](https://arxiv.org/pdf/1801.00690v1.pdf)  
[Quo Vadis, Action Recognition? A New Model and the Kinetics Dataset](https://arxiv.org/pdf/1705.07750.pdf)  
4.  Intuitive Physics  
[Position-Velocity Encoders for Unsupervised Learning of Structured State Representations](https://arxiv.org/pdf/1705.09805.pdf)  
[Learning to Perform Physics Experiments via Deep Reinforcement Learning](https://arxiv.org/pdf/1611.01843.pdf)  
[Continuous Control with Deep Reinforcement Learning](https://arxiv.org/pdf/1509.02971v2.pdf)  
5.  Reinforcement Learning (Papers with a pure RL focus)  
[Model-Based RL]  
[Learning Model-Based Planning from Scratch]  
[Recurrent Environment Simulators](https://arxiv.org/pdf/1704.02254.pdf)  
[Structure Learning in Motor Control: A Deep Reinforcement Learning Model  
[Imagination-Augmented Agents for Deep Reinforcement Learning]  
[Continuous Deep Q-Learning with Model-based Acceleration](https://arxiv.org/abs/1603.00748)  
[Skip Context Tree Switching](http://proceedings.mlr.press/v32/bellemare14.pdf)  
[Bayes-Adaptive Simulation-Based Search with Value Function Approximation](http://www0.cs.ucl.ac.uk/staff/d.silver/web/Publications_files/bafa.pdf)  
[Learning and Querying Fast Generative Models for Reinforcement Learning](https://arxiv.org/abs/1802.03006)  
6.  Exploration in RL  
[Count-Based Exploration with Neural Density Models](https://arxiv.org/pdf/1703.01310.pdf)  
[Unifying Count-Based Exploration and Intrinsic Motivation](https://arxiv.org/abs/1606.01868)  
[Deep Exploration via Bootstrapped DQN](https://arxiv.org/abs/1602.04621)  
[Variational Intrinsic Control](https://arxiv.org/pdf/1611.07507.pdf)  
[Learning to Search with MCTSnets](https://arxiv.org/abs/1802.04697v1)  
[Observe and Look Further: Achieving Consistent Performance on Atari](https://arxiv.org/abs/1805.11593)  
[A Distributional Perspective on Reinforcement Learning](https://arxiv.org/pdf/1707.06887.pdf)  
[FeUdal Networks for Hierarchical Reinforcement Learning]  
[Combining Policy Gradient and Q-Learning](https://arxiv.org/pdf/1611.01626.pdf)  
[Strategic Attentive Writer for Learning Macro-Actions](https://arxiv.org/pdf/1606.04695.pdf)  
[Safe and Efficient Off-Policy Reinforcement Learning](https://arxiv.org/abs/1606.02647)  
[Deep Reinforcement Learning for Robotic Manipulation with Asynchronous Off-Policy Updates](https://arxiv.org/pdf/1610.00633.pdf)  
[Thompson Sampling is Asymptotically Optimal in General Environments](https://arxiv.org/pdf/1602.07905.pdf)  
[Asynchronous Methods for Deep Reinforcement Learning](https://arxiv.org/abs/1602.01783)  
[Dueling Network Architectures for Deep Reinforcement Learning](https://arxiv.org/abs/1511.06581)  
[Increasing the Action Gap: New Operators for Reinforcement Learning](https://arxiv.org/abs/1512.04860)  
[Deep Reinforcement Learning with Double Q-Learninghttps://arxiv.org/abs/1509.06461](https://arxiv.org/abs/1509.06461)  
[Policy Distillation](https://arxiv.org/pdf/1511.06295.pdf)  
[Universal Value Function Approximators](http://proceedings.mlr.press/v37/schaul15.pdf)  
[Human-level Control through Deep Reinforcement Learning](https://storage.googleapis.com/deepmind-media/dqn/DQNNaturePaper.pdf)  
[Learning Continuous Control Policies by Stochastic Value Gradients](https://arxiv.org/pdf/1510.09142v1.pdf)  
[Fictitious Self-Play in Extensive Form Games](http://proceedings.mlr.press/v37/heinrich15.pdf)  
[Toward Minimax Off-policy Value Estimation](http://proceedings.mlr.press/v38/li15b.html)  
[Massively Parallel Methods for Deep Reinforcement Learning](https://arxiv.org/pdf/1507.04296.pdf)  
[Compress and Control](https://arxiv.org/pdf/1411.5326v1.pdf)  
[Deterministic Policy Gradient Algorithms](http://proceedings.mlr.press/v32/silver14.pdf)  
[Playing Atari with Deep Reinforcement Learning](https://arxiv.org/pdf/1312.5602v1.pdf)  
[Reinforcement Learning, Efficient Coding, and the Statistics of Natural Tasks](http://www.sciencedirect.com/science/article/pii/S2352154615001151)  
[Rainbow: Combining Improvements in Deep Reinforcement Learning](https://arxiv.org/abs/1710.02298)  
[Path Consistency Learning in Tsallis Entropy Regularized MDPs](https://arxiv.org/abs/1802.03501)  
[More Robust Doubly Robust Off-Policy Evaluation](https://arxiv.org/abs/1802.03493)  
[IMPALA: Scalable Distributed Deep-RL with Importance Weighted Actor-Learner Architectures](https://arxiv.org/abs/1802.01561)  
[Mis&Match - Agent Curricula for Reinforcement Learning](https://arxiv.org/abs/1806.01780)  
[Vector-based Navigation Using Grid-Like Representations in Artificial Agents](https://www.nature.com/articles/s41586-018-0102-6.epdf)?  
[Kickstarting Deep Reinforcement Learning](https://arxiv.org/abs/1803.03835)  
13.  Applications  
14.  Go  
[Mastering the Game of Go with Deep Neural Networks and Tree Search](https://storage.googleapis.com/deepmind-media/alphago/AlphaGoNaturePaper.pdf)  
[More Evaluation in Go using Deep Convolutional Neural Networks]  
[Mastering the Game of Go Without Human Knowledge](https://www.nature.com/articles/nature24270.epdf)?  
15.  Poker  
[Smooth UCT Search in Computer Poker](http://www0.cs.ucl.ac.uk/staff/d.silver/web/Publications_files/smooth_uct.pdf)  
16.  Fairness  
[Path-Specific Counterfactual Fairness](https://arxiv.org/pdf/1802.08139.pdf)  
[Safety / Security]  
[Reinforcement Learning with a Corrupted Reward Channel]  
[Safely Interruptible Agents]  
[AI Safety Gridworlds](https://arxiv.org/abs/1711.09883)  
[Adversarial Risk and the Dangers of Evaluating Against Weak Attacks](https://arxiv.org/abs/1802.05666)  
[Safe Exploration in Continuous Action Spaces](https://arxiv.org/abs/1801.08757)  
[Measuring and Avoiding Side Effects Using Relative Reachability](https://arxiv.org/abs/1806.01186)  
19.  Deep Learning  
[Recurrent Neural Networks]  
[Sequential Neural Models with Stochastic Layers]  
[Memory-Efficient Backpropagation Through Time](https://arxiv.org/abs/1606.03401)  
[Adaptive Computation Time for Recurrent Neural Networks](https://arxiv.org/abs/1603.08983)  
[Grid Long-Short Term Memory](https://arxiv.org/pdf/1507.01526v3.pdf)  
[Order Matters: Sequence to Sequence for Sets](https://arxiv.org/pdf/1511.06391v3.pdf)  
20.  Convolutional Neural Networks  
[Exploiting Cyclic Symmetry in Convolutional Neural Networks](https://arxiv.org/abs/1602.02660)  
[Spatial Transformer Networks](https://arxiv.org/pdf/1506.02025.pdf)  
[Very Deep Convolutional Networks for Large Scale Image Recognition](https://arxiv.org/pdf/1409h.1556v6.pdf)  
[Pooling is Neither Necessary Nor Sufficient for Appropriate Deformation Stability in CNNs](https://arxiv.org/abs/1804.04438)  
[Noisy Networks for Exploration](https://arxiv.org/pdf/1706.10295.pdf)  
[Sobolev Training for Neural Networks](https://arxiv.org/abs/1706.04859)  
[Decoupled Neural Interfaces using Synthetic Gradients](https://arxiv.org/pdf/1608.05343.pdf)  
[Understanding Synthetic Gradients and Decoupled Neural Interfaces](https://arxiv.org/pdf/1703.00522.pdf)  
[Simple and Scalable Predictive Uncertainty Estimation using Deep Ensembles](https://arxiv.org/pdf/1612.01474.pdf)  
[Overcoming Catastrophic Forgetting in Neural Networks](https://arxiv.org/pdf/1612.00796.pdf)  
[Local Minima in Training of Neural Networks](https://arxiv.org/pdf/1611.06310.pdf)  
[Learning Values Across Many Orders of Magnitude](https://arxiv.org/abs/1602.07714)  
[MuProp: Unbiased Backpropagation for Stochastic Neural Networks](https://arxiv.org/pdf/1511.05176v2.pdf)  
[ACDC: A Structured Efficient Linear Layer](https://arxiv.org/pdf/1511.05946v3.pdf)  
[Natural Neural Networks](https://arxiv.org/pdf/1507.00210.pdf)  
[Gradient Estimation Using Stochastic Computation Graphs](https://arxiv.org/pdf/1506.05254v1.pdf)  
[Weight Uncertainty in Neural Networks](http://proceedings.mlr.press/v37/blundell15.pdf)  
[Stochastic Backpropagation and Approximate Inference in Deep Generative Models](https://arxiv.org/abs/1401.4082)  
[On the Importance of Single Directions for Generalization](https://arxiv.org/abs/1803.06959)  
27.  Variational Inference  
[Filtering Variational Objectives](https://arxiv.org/pdf/1705.09279.pdf)  
[Variational Inference for Monte Carlo Objectives](https://arxiv.org/abs/1602.06725)  
[Variational Inference with Normalizing Flows](https://arxiv.org/pdf/1505.05770.pdf)  
[Variational Information Maximization for Intrinsically Motivated Reinforcement Learning]  
[Neural Variational Inference and Learning in Belief Networks](https://arxiv.org/pdf/1402.0030v2.pdf)  
[Distribution Matching in Variational Infeence](https://arxiv.org/abs/1802.06847)  
29.  Generative Models  
[The Cramer Distance as a Solution to Biased Wasserstein Gradients](https://arxiv.org/pdf/1705.10743.pdf)  
[Variational Approaches for Auto-Encoding Generative Adversarial Networks](https://arxiv.org/pdf/1706.04987.pdf)  
[Comparison of Maximum Likelihood and GAN-based training of Real NVPs](https://arxiv.org/pdf/1705.05263.pdf)  
[Parallel Multiscale Autoregressive Density Estimation](https://arxiv.org/pdf/1703.03664.pdf)  
[Conditional Image Generation with PixelCNN Decoders](https://arxiv.org/pdf/1606.05328.pdf)  
[WaveNet: A Generative Model for Raw Audio](https://arxiv.org/pdf/1609.03499.pdf)  
[Video Pixel Networks](https://arxiv.org/pdf/1610.00527.pdf)  
[Learning in Implicit Generative Models](https://arxiv.org/pdf/1610.03483.pdf)  
*Connecting Generative Adversarial Networks and Actor-Critic Methods]  
[Pixel Recurrent Neural Networks](https://arxiv.org/abs/1601.06759)  
[One-Shot Generalization in Deep Generative Models](https://arxiv.org/abs/1603.05106)  
[A Test of Relative Similarity for Model Selection in Generative Models](https://arxiv.org/pdf/1511.04581.pdf)  
[DRAW: A Recurrent Neural Network for Image Generation]  
[Semi-Supervised Learning with Deep Generative Models](https://arxiv.org/abs/1406.5298)  
[Deep AutoRegressive Networks](https://arxiv.org/abs/1310.8499)  
[A Note on the Evaluation of Generative Models](https://arxiv.org/pdf/1511.01844v2.pdf)  
[Parallel WaveNet: Fast High-Fidelity Speech Synthesis (WaveRNN)](https://arxiv.org/abs/1711.10433)  
[Efficient Neural Audio synthesis](https://arxiv.org/abs/1802.08435)  
[Learning and Querying Fast Generative Models for Reinforcement Learning](https://arxiv.org/abs/1802.03006)  
[Unsupervised Learning]  
[of 3D Structure from Image](https://arxiv.org/pdf/1607.00662.pdf)  
[Early Visual Concept Learning with Unsupervised Deep Learning (beta-VAE)](https://arxiv.org/pdf/1606.05579.pdf)  
[Neural Scene Representation and Rendering](http://science.sciencemag.org/content/360/6394/1204)  
[Spectral Inference Networks: Unifying Spectral Methods with Deep Learning](https://arxiv.org/abs/1806.02215)  
32.  Representation Learning  
[SCAN: Learning Abstract Hierarchical Compositional Visual Concepts](https://arxiv.org/pdf/1707.03389.pdf)  
[Towards Conceptual Compression](https://arxiv.org/abs/1604.08772)  
[Neural Discrete Representation Learning]  
[Disentangling by Factorising](https://arxiv.org/abs/1802.05983)  
[Associative Compression Networks for Representation Learning](https://arxiv.org/abs/1804.02476)  
35.  Attention  
[Attend, Infer, Repeat: Fast Scene Understanding with Generative Models](https://arxiv.org/pdf/1603.08575.pdf)  
[Reasoning about Entailment with Neural Attention]  
[Multiple Object Recognition with Visual Attention](https://arxiv.org/pdf/1412.7755v2.pdf)  
[Recurrent Models of Visual Attention](https://arxiv.org/abs/1406.6247)  
38.  Memory  
[Neural Episodic Control](https://arxiv.org/pdf/1703.01988.pdf)  
[Generative Temporal Models With Memory](https://arxiv.org/pdf/1702.04649.pdf)  
[Scaling Memory-Augmented Neural Networks with Sparse Reads and Writes](https://arxiv.org/pdf/1610.09027.pdf)  
[Model-Free Episodic Control](https://arxiv.org/abs/1606.04460)  
[One-Shot Learning with Memory-Augmented Neural Networks](https://arxiv.org/abs/1605.06065)  
[Associative Long Short-Term Memory](https://arxiv.org/abs/1602.03032)  
[Prioritized Experience Replay](https://arxiv.org/pdf/1511.05952v3.pdf)  
[Sample Efficient Actor-Critic with Experience Replay](https://arxiv.org/pdf/1611.01224.pdf)  
[Algorithms with Hierarchical Attentive Memory](https://arxiv.org/abs/1602.03218)  
[Estimation with Bounded Memory](http://www.ijcai.org/Proceedings/15/Papers/470.pdf)  
[Memory-based Parameter Adaptation](https://arxiv.org/abs/1802.10542)  
41.  Multi-Agent Systems  
[Value Decomposition Networks For Cooperative Multi-Agent Learning](https://arxiv.org/pdf/1706.05296.pdf)  
[Learning to Communicate with Deep Multi-Agent Reinforcement Learning]  
[A Unified Game-Theoretic Approach to Multiagent Reinforcement Learning  
][Machine Theory of Mind](https://arxiv.org/abs/1802.07740)  
44.  Imitation Learning  
[Robust Imitation of Diverse Behaviors](https://arxiv.org/pdf/1707.02747.pdf)  
[Learning Human Behaviors from Motion Capture by Adversarial Imitation](https://arxiv.org/abs/1707.02201)  
[Leveraging Demonstrations for Deep Reinforcement Learning on Robotics Problems with Sparse Rewards](https://arxiv.org/pdf/1707.08817.pdf)  
[Reinforcement and Imitation Learning for Diverse Visuomotor Skills](https://arxiv.org/abs/1802.09564)  
[Playing Hard Exploration Games by Watching Youtube](https://arxiv.org/abs/1805.11592)  
47.  Metalearning  
48.  Neural Programming  
[Hybrid Computing Using a Neural Network with Dynamic External Memory](https://www.nature.com/articles/nature20101.epdf?author_access_token=ImTXBI8aWbYxYQ51Plys8NRgN0jAjWel9jnR3ZoTv0MggmpDmwljGswxVdeocYSurJ3hxupzWuRNeGvvXnoO8o4jTJcnAyhGuZzXJ1GEaD-Z7E6X_a9R-xqJ9TfJWBqz)  
[Programmable Agents]  
[Neural Programmer-Interpreters](https://arxiv.org/pdf/1511.06279v3.pdf)  
[Neural Random-Access Machines](https://arxiv.org/pdf/1511.06392v3.pdf)  
[Neural Turing Machines](https://arxiv.org/abs/1410.5401)  
[Learning Explanatory Rules from Noisy Data](https://arxiv.org/abs/1711.04574)  
[Synthesizing Programs for Images using Reinforced Adversarial Learning (SPIRAL)](https://arxiv.org/abs/1804.01118)  
[Learning to learn by gradient descent by gradient descent](https://arxiv.org/abs/1606.04474)  
[  
[Hierarchical Representations for Efficient Architecture Search](https://arxiv.org/pdf/1711.00436.pdf)  
[Population Based Training of Neural Networks](https://arxiv.org/abs/1711.09846)  
[Meta-Gradient Reinforcement Learning](https://arxiv.org/abs/1805.09801)  
53.  Evolution  
[Convolution by Evolution](https://arxiv.org/pdf/1606.02580.pdf)  
56.  Game Theory  
[Learning Nash Equilibrium for General-Sum Markov Games from Batch Data](https://arxiv.org/pdf/1606.08718.pdf)  
[The Mechanics of n-Player Differentiable Games]  
[Symmetric Decomposition of Asymmetric Games](https://www.nature.com/articles/s41598-018-19194-4)  
[A Generalised Method for Empirical Game Theoretic Analysis](https://arxiv.org/abs/1803.06376)  
[Inequity Aversion Resolves Intertemporal Social Dilemmas](https://arxiv.org/abs/1803.08884)  
59.  Natural Language Processing  
[Generative and Discriminative Text Classification with Recurrent Neural Networks](https://arxiv.org/pdf/1703.01898.pdf)  
[Learning to Compose Words Into Sentences with Reinforcement Learning](https://arxiv.org/pdf/1611.09100.pdf)  
[Reference-Aware Language Models](https://arxiv.org/pdf/1611.01628.pdf)  
[The Neural Noisy Channel](https://arxiv.org/pdf/1611.02554.pdf)  
[Latent Predictor Networks for Code Generation](https://arxiv.org/pdf/1603.06744.pdf)  
[Learning the Curriculum with Bayesian Optimization for Task-Specific Word Representation Learning](https://arxiv.org/pdf/1605.03852.pdf)  
[Semantic Parsing with Semi-Supervised Sequential Autoencoders](https://arxiv.org/pdf/1609.09315.pdf)  
[On the State of the Art of Evaluation in Neural Language Models](https://arxiv.org/abs/1707.05589)  
[Teaching Machines to Read and Comprehend](https://arxiv.org/pdf/1506.03340v1.pdf)  
[Dependency Recurrent Neural Language Models for Sentence Completion](http://cs.nyu.edu/~mirowski/pub/MirowskiVlachos_ACL2015_DependencyTreeRNN.pdf)  
[Towards End-to-End Speech Recognition with Recurrent Neural Networks](http://proceedings.mlr.press/v32/graves14.pdf)  
[Learning Word Embeddings Efficiently with Noise-Contrastive Estimation](http://papers.nips.cc/paper/5165-learning-word-embeddings-efficiently-with-noise-contrastive-estimation.pdf)  
[The NarrativeQA Reading Comprehension Challenge](https://arxiv.org/abs/1712.07040v1)  
[Learning to Follow Language Instructions with Adversarial Reward Induction](https://arxiv.org/abs/1806.01946)  
61.  Multi-Modal  
[Look, Listen and Learn](https://arxiv.org/pdf/1705.08168.pdf)  
[End-to-end Optimization of Goal-Driven and Visually Grounded Dialogue Systems](https://arxiv.org/pdf/1703.05423.pdf)  
[GuessWhat?! Visual Object Discovery through Multi-Modal Dialogue](https://arxiv.org/pdf/1611.08481.pdf)  
[Grounded Language Learning in a Simulated 3D World](https://arxiv.org/pdf/1706.06551.pdf)  
[Understanding Grounded Language Learning Agents]  
[Objects that Sound](https://arxiv.org/abs/1712.06651)  
62.  General Machine Learning  
[The Concrete Distribution: A Continuous Relaxation of Discrete Random Variables](https://arxiv.org/pdf/1611.00712.pdf)  
[Learning Deep Nearest Neighbor Representations Using Differentiable Boundary Trees](https://arxiv.org/pdf/1702.08833.pdf)  
[Unit Tests for Stochastic Optimization](https://arxiv.org/pdf/1312.6055v3.pdf)  
[Bayesian Hierarchical Community Discovery](http://papers.nips.cc/paper/5048-bayesian-hierarchical-community-discovery.pdf)  
[Implicit Reparameterization Gradients](https://arxiv.org/abs/1805.08498)  
63.  Cleaning up the Neighborhood: A Full Classification for Adversarial Partial Monitoring  
[[https://arxiv.org/abs/1805.09247](https://arxiv.org/abs/1805.09247)  
65.  Theory  
66.  Online Learning with Gated Linear Networks  
[[https://arxiv.org/abs/1712.01897v1](https://arxiv.org/abs/1712.01897v1)  
68.  Miscellaneous  
[Generalized Probability Smoothing](https://arxiv.org/abs/1712.02151)  
[Agents and Devices: A Relative Definition of Agency](https://arxiv.org/abs/1805.12387)  
69.  Neuroscience  
[The Successor representation in human reinforcement learning](http://www.biorxiv.org/content/biorxiv/early/2017/07/04/083824.full.pdf)  
[Dorsal Hippocampus Contributes to Model-Based Planning](https://www.nature.com/articles/nn.4613.epdf?author_access_token=OfuqRzRgBmFKQdGE1Qw7FdRgN0jAjWel9jnR3ZoTv0N3IprbEH8EVdPgVTpPLVjgaMNMGW_KprBhEEIm7f1drNjI5FB2fds3h58n3XEtMJPC3kLK1Pp3J2_Qb45cy7uk)  
[Neuroscience-Inspired Artificial Intelligence](http://www.cell.com/neuron/fulltext/S0896-6273(17)30509-3)  
[Computations Underlying Social Hierarchy Learning: Distinct Neural Mechanism for Updating and Representing Self-Relevant Information](http://www.cell.com/neuron/pdf/S0896-6273(16)30802-9.pdf)  
[Dorsal Anterior Cingulate Cortex and the Value of Control](https://www.nature.com/articles/nn.4384.epdf?author_access_token=dq-w7RyWLn3z-0m4nbyTW9RgN0jAjWel9jnR3ZoTv0N7RVyemANPvboWSepiJaSAsTFiGqyORVbog9B6IjN113kC9aqMAEoNVCCfdRA4gLVJXcy4e1klhW0KiKS5F1gp)  
[Semantic Representations in the Temporal Pole Predict False Memories](http://www.pnas.org/content/113/36/10180.abstract)  
[Towards an Integration of Deep Learning and Neuroscience](http://www.biorxiv.org/content/early/2016/06/13/058545)  
[What Learning Systems do Intelligent Agents Need? Complementary Learning systems Theory Updated](http://www.cell.com/trends/cognitive-sciences/fulltext/S1364-6613(16)30043-2)  
[Neural Mechanisms of Hierarchical Planning in a Virtual Subway Network]  
[Predictive Representations can Link Model-Based Reinforcement Learning to Model-Free Mechanisms](https://www.biorxiv.org/content/early/2016/10/27/083857)  
[Hippocampal place cells construct reward related sequences through unexplored space](https://elifesciences.org/articles/06063)  
[A Probabilistic Approach to Demixing Odors](http://www.nature.com/neuro/journal/v20/n1/full/nn.4444.html)  
[Approximate Hubel-Wiesel Modules and the Data Structures of Neural Computation](https://arxiv.org/pdf/1512.08457v1.pdf)  
[The Future of Memory: Remembering, Imagining, and the Brain](http://static1.1.sqspcdn.com/static/f/1096238/22043246/1361990370157/FutureMemory--Neuron12.pdf?token=b5gB3ycz3e%2BmKnQQCW3%2FvwZyHwE%3D)  
[Is the Brain a Good Model for Machine Intelligence?](http://www.gatsby.ucl.ac.uk/~demis/TuringSpecialIssue(Nature2012).pdf)  
[Evidence Integration in Model-Based Tree Search](http://www.pnas.org/content/112/37/11708.full.pdf)  
[(Commentary on0 Building Machines that Learn and Think for Themselves](https://www.cambridge.org/core/journals/behavioral-and-brain-sciences/article/building-machines-that-learn-and-think-for-themselves/E28DBFEC380D4189FB7754B50066A96F)  
[Prefrontal Cortex as a Meta-Reinforcement Learning System](https://www.nature.com/articles/s41593-018-0147-8)  


Current Frontier:

1.  Hierarchical planning
    
2.  Imagination-based planning with generative models
    
3.  Unsupervised Learning
    
4.  Memory and one-shot learning
    
5.  Abstract Concepts
    
6.  Continual and Transfer Learning
    

  

Emphasis on systems neuroscience - using the brain as inspiration for the structure and function of algorithms.

  

[Neuroscience Inspired Artificial Intelligence](http://sci-hub.cc/10.1016/j.neuron.2017.06.011)

Examples of previous success of neuro-inspiration:

-   Reinforcement Learning
    

-   Inspired by animal learning
    
-   TD Learning came out of animal behavior research.
    
-   Second-order conditioning (Conditional Stimulus) (Sutton and Barto, 1981)
    

-   Deep Learning.
    

-   Convolutional Neural Networks. Visual Cortex (V1)
    

-   Uses hierarchical structure (successive processing layers)
    
-   Neurons in the early visual systems responds strongly to specific patterns of light (say, precisely oriented bars) but hardly responds to many other patterns.
    
-   Gabor functions describe the weights in V1 cells.
    
-   Nonlinear Transduction
    
-   Divisive Normalization
    

-   Word / Sentence Vectors - Distributed Embeddings
    

-   Parallel Distributed Processing in the brain for representation and computation
    

-   Dropout
    

-   Stochasticity in neurons that fire with` Poisson-like statistics (Hinton 2012)
    

-   Attention
    

-   Applying attention to memory
    
-   Thought - it doesn’t make much sense to train an attention model over a static image, rather than over a time series. With a time series, bringing attention to changing aspects of the input makes sense.
    

-   Multiple Memory Systems
    

-   Episodic Memory
    

-   Experience Replay
    
-   Especially for one shot experiences
    

-   Working Memory
    

-   LSTM - gating allows for conditioning on current state
    

-   Long-term Memory
    

-   External Memory
    
-   Gating in LSTM
    

-   Continual Learning
    

-   Elastic weight consolidation for slowing down learning on weights that are important for previous tasks.
    

  

Examples of future success:

-   Intuitive Understanding of Physics
    

-   Need to understand space, number, objectness
    
-   Need to disentangle representations for transfer. (Dude, I feel so stolen from)
    

-   Efficient Learning (Learning from few examples)
    
-   Transfer Learning
    

-   Transferring generalized knowledge gained in one context to novel domains
    
-   Concept representations for transfer
    

-   No direct evidence of concept representations in brains
    

-   Imagination and Planning
    

-   Toward model-based RL
    
-   Internal model of the environment
    

-   Model needs to include compositional / disentangled representations for flexibility
    

-   Implementing a forecasted-based method of action selection
    
-   Monte-carlo Tree Search as simulation based planning
    
-   In rat brains, we observe ‘preplay’ where rats imagine the likely future experience - measured by comparing neural activations at preplay to activations during the activity
    
-   Generalization + Transfer in human planning
    
-   Hierarchical Planning
    

-   Virtual Brain Analytics
    
