---
layout: post
title: "Google Brain Research Overview"
date:   2019-02-08
categories: intelligence
---
By Jeremy Nixon [[jnixon2@gmail.com](mailto:jnixon2@gmail.com)]. Nov. 2017. Updated June 2018.

Overview
1. Categorization of Breakthroughs / Contents
2. Major / Minor Researchers List (All appearing on papers)
3. Genealogy
4. Sorted Researchers by Paper Count


1. Deep Learning
   * Scalability and Speed
   * Convolutional Neural Networks
   * Recurrent Neural Networks
   * Privacy
   * Understanding / Theory
   * Regularization
2. Applications
   * Speech Recognition
   * Image Categorization
   * Image Captioning
   * Machine Translation
   * Natural Language Understanding
   * Multi-Modal
   * Pedestrian Detection
   * Grasp Detection
   * Go
   * Video
   * Dialogue
   * 3D Object Reconstruction
   * Speaker Verification
   * Health Care
   * Theorem Proving
   * Music
   * Pose Estimation
   * Speech Generation
   * Super Resolution
   * Chemistry
   * Robotics
      * Autonomous Vehicles
   * Physics
   * Device Placement
   * Games
   * Art
3. Unsupervised Learning
4. Attention
5. Memory
6. Transfer Learning
7. Representation Learning
8. Reinforcemnet Learning
   * Model-Based Reinforcement Learning
   * Multi-Task Learning
9. Metalearning
   * Neural Programming
   * Hyperparameter Optimization
10. Generative
    * GANs
11. Intrepretability
12. Tools, Environments &amp; Datasets
13. Adversarial Examples
14. Multi-Agent Systems
15. Variational Inference
16. Kernel Machines
17. Collaborative Filtering
18. Graphical / Relational Learning
19. Miscellaneous


1. Deep Learning
   * Scalability and Speed
      * [Large Scale Distributed Deep Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40565.pdf)
      * [Multiframe Deep Neural Networks for Acoustic Modeling](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40810.pdf)
      * [Asynchronous Stochastic Optimization for Sequence Training of Deep Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42248.pdf)
      * [Tensorflow: Large-Scale Machine Learning on Heterogeneous Distributed Systems](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45166.pdf)
      * [Distilling the Knowledge in a Neural Network](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44873.pdf)
      * [Deep Networks with Large Output Spaces](https://arxiv.org/pdf/1412.7479.pdf)
      * [TensorFlow: A System for Large-Scale Machine Learning](https://www.usenix.org/system/files/conference/osdi16/osdi16-abadi.pdf)
      * [Revisiting Distributed Synchronous SGD](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45187.pdf)
      * [Depthwise Separable Convolutions for Neural Machine Translation](https://arxiv.org/abs/1706.03059)
      * [Large Scale Distributed Neural Network Training Through Online Distillation](https://openreview.net/pdf?id=rkr1UDeC-)
      * [Deep Gradient Compression: Reducing the Communication Bandwidth for Distributed Training](https://openreview.net/pdf?id=SkhQHMW0W)
   * Convolutional Neural Networks
      * [Going Deeper with Convolutions [Inception]](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43022.pdf)
      * [Rethinking the Inception Architecture for Computer Vision](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44903.pdf)
      * [Inception-v4, Inception-ResNet and the Impact of Residual Connections on Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45169.pdf)
      * [Towards Understanding the Invertibility of Convolutional Neural Networks](https://arxiv.org/pdf/1705.08664.pdf)
   * Recurrent Neural Networks
      * [Sequence to Sequence Learning with Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43155.pdf)
      * [Sequence Discriminative Distributed Training of Long Short-Term Memory Recurrent Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42547.pdf)
      * [Recurrent Neural Network Regularization [Also, Language Modeling]](https://arxiv.org/abs/1409.2329)
      * [Semi-supervised Sequence Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44267.pdf)
      * [Learning to Execute](https://research.google.com/pubs/pub45474.html)
      * [An Empirical Exploration of Recurrent Network Architectures](https://research.google.com/pubs/pub45473.html)
      * [A Simple Way to Initialize Recurrent Networks of Rectified Linear Units](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44961.pdf)
      * [Using Fast Weights to Attend to the Recent Past](https://arxiv.org/pdf/1610.06258.pdf)
      * [Unsupervised Pre-training for Sequence to Sequence Learning](https://arxiv.org/pdf/1611.02683.pdf)
      * [Order Matters: Sequence to Sequence for Sets](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44871.pdf)
      * [Multi-Task Sequence to Sequence Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44928.pdf)
      * [Generating Sentences from a Continuous Space](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45404.pdf)
      * [Exponential expressivity in deep neural networks through transient chaos](https://arxiv.org/pdf/1606.05340.pdf)
      * [An Online Sequence-to-Sequence Model Using Partial Conditioning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45167.pdf)
      * [A Neural Transducer](https://arxiv.org/pdf/1511.04868.pdf)
      * [Tuning Recurrent Neural Networks with Reinforcement Learning](https://openreview.net/pdf?id=Syyv2e-Kx)
      * [Sequence Tutor: Conservative Fine-Tuning of Sequence Generation Models with KL-control](https://arxiv.org/pdf/1611.02796.pdf)
      * [SGD Learns the Conjugate Kernel Class of the Network](https://arxiv.org/pdf/1702.08503.pdf)
      * [Learning Hierarchical Information Flow with Recurrent Neural Modules](https://arxiv.org/pdf/1706.05744.pdf)
      * [Latent Sequence Decompositions](https://arxiv.org/pdf/1610.03035.pdf)
      * [Capacity and Trainability in Recurrent Neural Networks](https://openreview.net/pdf?id=BydARw9ex)
      * [Initialization Matters: Orthogonal Predictive State Recurrent Neural Networks](https://openreview.net/pdf?id=HJJ23bW0b)
   * Privacy
      * [Deep Learning with Differential Privacy](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45428.pdf)
      * [Semi-Supervised Knowledge Transfer for Deep Learning from Private Training Data](https://arxiv.org/pdf/1610.05755.pdf)
      * [Glimmers: Resolving the Privacy / Trust Quagmire](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46128.pdf)
      * [Scalable Private Learning with PATE](https://arxiv.org/pdf/1802.08908.pdf)
      * [Learning Differentially Private Recurrent Language Models [Also, Language Modeling]](https://openreview.net/pdf?id=BJ0hF1Z0b)
   * Understanding / Theory
      * [Qualitatively Characterizing Neural Network Optimization Problems](https://arxiv.org/pdf/1412.6544.pdf)
      * [Toward Deeper Understanding of Neural Networks: The Power of Initialization and a Dual View on Expressivity](https://arxiv.org/pdf/1602.05897.pdf)
      * [Understanding Deep Learning Requires Re-Thinking Generalization](https://arxiv.org/pdf/1611.03530.pdf)
      * [Sharp Minima Can Generalize for Deep Nets](https://arxiv.org/pdf/1703.04933.pdf)
      * [On the Expressive Power of Deep Neural Networks](https://arxiv.org/pdf/1606.05336.pdf)
      * [Nonlinear Random Matrix Theory for Deep Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46342.pdf)
      * [Mean Field Residual Networks: On the Edge of Chaos](http://papers.nips.cc/paper/6879-mean-field-residual-networks-on-the-edge-of-chaos.pdf)
      * [Identity Matters in Deep Learning](https://arxiv.org/pdf/1611.04231.pdf)
      * [Geometry of Neural Network Loss Surfaces via Random Matrix Theory](http://proceedings.mlr.press/v70/pennington17a/pennington17a.pdf)
      * [Explaining the Learning Dynamics of Direct Feedback Alignment](https://openreview.net/pdf?id=HkXKUTVFl)
      * [Deep Information Propagation](https://openreview.net/pdf?id=H1W1UN9gg)
      * [The Emergence of Spectral Universality in Deep Networks](https://arxiv.org/pdf/1802.09979.pdf)
      * [Sensitivity and Generalization in Neural Networks: An Empirical Study](https://arxiv.org/pdf/1802.08760.pdf)
      * [Gradient Descent with identity initialization efficiently learns positive definite linear transformations by deep residual networks](https://arxiv.org/pdf/1802.06093.pdf)
      * [Deep Neural Networks as Gaussian Processes](https://openreview.net/pdf?id=B1EA-M-0Z)
      * [A Bayesian Perspective on Generalization and Stochastic Gradient Descent](https://openreview.net/pdf?id=BJij4yg0Z)
   * Regularization
      * [Adding Gradient Noise Improves Learning for Very Deep Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45137.pdf)
      * [Surprising Properties of Dropout in Deep Networks](http://www.phillong.info/publications/HL17_deep_dropout.pdf)
      * [Regularizing Neural Networks by Penalizing Confident Output Distributions](https://arxiv.org/pdf/1701.06548.pdf)
      * [A Unified Approach to Adaptive Regularization in Online and Stochastic Optimization](https://arxiv.org/pdf/1706.06569.pdf)
    * [Training Highly Multiclass Classifiers](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41872.pdf)
    * [Random Walk Initialization for Training Very Deep Feedforward Networks](https://arxiv.org/pdf/1412.6558.pdf)
    * [Learning Factored Representations in a Deep Mixture of Experts](https://arxiv.org/pdf/1312.4314.pdf)
    * [Training Deep Neural Networks on Noisy Labels with Bootstrapping](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43273.pdf)
    * [Convolutional, Long Short-Term Memory, Fully Connected Deep Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43455.pdf)
    * [Reward Augmented Maximum Likelihood for Neural Structured Prediction](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45580.pdf)
    * [MuProp: Unbiased Backpropagation for Stochastic Neural Networks](https://arxiv.org/pdf/1511.05176v3.pdf)
    * [Chained predictions using convolutional neural networks](https://research.google.com/pubs/pub45945.html)
    * [Training a Subsampling Mechanism in Expectation](https://openreview.net/pdf?id=BJBkkaNYe)
    * [Resurrecting the Sigmoid in deep learning through dynamical isometry: theory and practice](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46341.pdf)
    * [Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer](https://openreview.net/pdf?id=B1ckMDqlg)
    * [On Blackbox Backpropagation and Jacobian Sensing](https://research.google.com/pubs/pub46347.html)
    * [Deep Value Networks Learn to Evaluate and Iteratively Refine Structured Outputs](https://arxiv.org/pdf/1703.04363.pdf)
    * [Critical Hyper-Parameters: No Random, No Cry](https://arxiv.org/pdf/1706.03200.pdf)
    * [Distilling a Neural Network into a Soft Decision Tree](https://arxiv.org/pdf/1711.09784.pdf)
    * [Categorical Reparameterization with Gumbel-Softmax](https://arxiv.org/pdf/1611.01144.pdf)
    * [Training Confidence-Calibrated Classifiers For Detecting Out-of-Distribution Samples](https://openreview.net/pdf?id=ryiAv2xAZ)
    * [Fidelity-Weighted Learning](https://openreview.net/pdf?id=B1X0mzZCW)
    * [Don’t Decay the Learning Rate, Increase the Batch Size](https://openreview.net/pdf?id=B1Yy1BxCZ)
2. Applications
   * Speech Recognition
      * [Deep Neural Networks for Acoustic Modeling in Speech Recognition](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38131.pdf)
      * [Application of Pre-trained Deep Neural Networks to Large Vocabulary Speech Recognition](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38130.pdf)
      * [On Rectified Linear Units for Speech Processing](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40811.pdf)
      * [Multilingual Acoustic Models Using Distributed Deep Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40807.pdf)
      * [An Empirical Study of Learning Rates in DNNs for Speech Recognition](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40808.pdf)
      * [Word Embeddings for Speech Recognition](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42543.pdf)
      * [Autoregressive product of multi-frame predictions can improve the accuracy of hybrid models](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42947.pdf)
      * [Learning the Speech Front-end with Raw Waveform CLDNNs](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43960.pdf)
      * [Acoustic Modeling for Google Home](http://www.cs.cmu.edu/~chanwook/MyPapers/b_li_interspeech_2017.pdf)
      * [Multilingual Speech Recognition With a Single End-to-End Model](https://arxiv.org/pdf/1711.01694.pdf)
      * [An Analysis of Incorporating an External Language Model into a Sequence-to-Sequence Model](https://arxiv.org/pdf/1712.01996.pdf)
   * Image Classification
      * [Using Web Co-occurrence Statistics for Improving Image Categorization](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42244.pdf)
      * [The Unreasonable Effectiveness of Noisy Data for Fine-Grained Recognition](https://arxiv.org/pdf/1511.06789.pdf)
   * Image Captioning
      * [Grounded Compositional Semantics for Finding and Describing Images with Sentences](https://nlp.stanford.edu/~socherr/SocherKarpathyLeManningNg_TACL2013.pdf)
      * [Show and Tell: A Neural Image Caption Generator](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43274.pdf)
      * [Learning Semantic Relationships for Better Action Retrieval in Images](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43443.pdf)
   * Machine Translation
      * [Exploiting Similarities among Languages for Machine Translation](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44931.pdf)
      * [Addressing the Rare Word Problem in Neural Machine Translation](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44929.pdf)
      * [Google’s Neural Machine Translation System: Bridging the Gap between Human and Machine Translation](https://arxiv.org/abs/1609.08144)
      * [Sequence-to-Sequence Models Can Directly Translate Foreign Speech](https://arxiv.org/pdf/1703.08581.pdf)
      * [Massive Exploration of Neural Machine Translation Architectures](https://arxiv.org/pdf/1703.03906.pdf)
   * Natural Language Understanding
      * [Efficient Estimation of Word Representations in Vector Space](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41224.pdf)
      * [Distributed Representations of Words and Their Compositionality](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44876.pdf)
      * [Zero-Shot Learning by Convex Combination of Semantic Embeddings](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42371.pdf)
      * [Distributed Representations of Sentences and Documents](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44930.pdf)
      * [Sentence Compression by Deletion with LSTMs](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43852.pdf)
      * [Grammar as a Foreign Language](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43799.pdf)
      * [BilBOWA: Fast Bilingual Distributed Representations without Word Alignments](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45190.pdf)
      * [Multilingual Language Processing From Bytes](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45170.pdf)
      * [Exploring the Limits of Language Modeling](https://arxiv.org/pdf/1602.02410.pdf)
      * [Towards better decoding and language model integration in sequence to sequence models](https://arxiv.org/pdf/1612.02695.pdf)
      * [Learning to Skim Text](https://arxiv.org/pdf/1704.06877.pdf)
      * [Get To The Point: Summarization with Pointer-Generator Networks](https://arxiv.org/pdf/1704.04368.pdf)
      * [Generating Wikipedia by Summarizing Long Sequences](https://openreview.net/pdf?id=Hyg0vbWC-)
      * [An Efficient Framework for Learning Sentence Representations](https://openreview.net/pdf?id=rJvJXZb0W)
   * Multi-Modal
      * [DeViSE: A Deep Visual-Semantic Embedding Model](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41869.pdf)
      * [Modulating Early Visual Processing by Language](https://arxiv.org/pdf/1707.00683.pdf)
      * [Context-aware Captions from Context-agnostic Supervision](http://openaccess.thecvf.com/content_cvpr_2017/papers/Vedantam_Context-Aware_Captions_From_CVPR_2017_paper.pdf)
      * [Better Text Understanding Through Image-To-Text Transfer](https://arxiv.org/pdf/1705.08386.pdf)
   * Pedestrian Detection
      * [Real Time Pedestrian Detection with Deep Network Cascades](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43850.pdf)
      * [Pedestrian Detection with a Large Field-Of-View Deep Network](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43849.pdf)
   * Grasp Detection
      * [Real-Time Grasp Detection Using Convolutional Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43875.pdf)
   * Go
      * [Move Evaluation in Go Using Deep Convolutional Neural Networks](https://arxiv.org/pdf/1412.6564.pdf)
      * [Mastering the game of Go with deep neural networks and tree search](https://www.nature.com/articles/nature16961)
   * Video
      * [Beyond Short Snippets: Deep Networks for Video Classification](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43793.pdf)
   * Dialogue
      * [A Neural Conversational Model](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44925.pdf)
      * [Smart Reply: Automated Response Suggestion for Email](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45189.pdf)
      * [Adversarial Evaluation of Dialogue Models](https://arxiv.org/pdf/1701.08198.pdf)
      * [Generating High-Quality and Informative Conversation Responses with Sequence-to-Sequence Models](https://arxiv.org/pdf/1701.03185.pdf)
   * 3D Object Reconstruction
      * [Perspective Transformer Nets: Learning Single-View 3D Object Reconstruction without 3D Supervision](https://arxiv.org/pdf/1612.00814.pdf)
   * Speaker Verification
      * [End-to-End Text-Dependent Speaker Verification](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44681.pdf)
   * Health Care
      * [Development and Validation of a Deep Learning Algorithm for Detection of Diabetic Retinopathy in Retinal Fundus Photographs](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45732.pdf)
   * Theorem Proving
      * [DeepMath - Deep Sequence Models for Premise Selection](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45402.pdf)
      * [Deep Network Guided Proof Search](https://arxiv.org/pdf/1701.06972.pdf)
   *  Music
      * [Audio Deepdream: Optimizing Raw Audio with Convolutional Networks](https://18798-presscdn-pagely.netdna-ssl.com/ismir2016/wp-content/uploads/sites/2294/2016/08/ardila-audio.pdf)
      * [Generating Music by Fine-Tuning Recurrent Neural Networks with Reinforcement Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45871.pdf)
      * [Neural Audio Synthesis of Musical Notes with WaveNet Autoencoders](https://arxiv.org/pdf/1704.01279.pdf)
   * Pose Estimation
      * [Towards Accurate Multi-person Pose Estimation in the Wild](https://arxiv.org/pdf/1701.01779.pdf)
   * Speech Generation
      * [Tacotron: Towards End-to-End Speech Synthesis](https://arxiv.org/pdf/1703.10135.pdf)
      * [RNN Approaches to Text Normalization: A Challenge](https://arxiv.org/pdf/1611.00068.pdf)
      * [On Using Backpropagation for Speech texture Generation and Voice Cnversion](https://arxiv.org/pdf/1712.08363.pdf)
      * [Natural TTS Synthesis by Conditioning Wavenet on Mel Spectrogram Prediction [Tacotron 2]](https://arxiv.org/pdf/1712.05884.pdf)
   * Super Resolution
      * [Pixel Recursive Super Resolution](https://arxiv.org/pdf/1702.00783.pdf)
   * Chemistry
      * [Neural Message Passing for Quantum Chemistry](https://arxiv.org/pdf/1704.01212.pdf)
   * Robotics
      * Autonomous Vehicles
         * [Learning with Proxy Supervision for End-To-End Visual Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45985.pdf)
         * [Learning Robotic Manipulation of Granular Media](https://arxiv.org/pdf/1709.02833.pdf)
         * [Learning hand-eye coordination for robotic grasping with deep learning and large-scale data collection](https://drive.google.com/file/d/0B0mFoBMu8f8BaHYzOXZMdzVOalU/view)
         * [End-to-End Learning of Semantic Grasping](https://arxiv.org/pdf/1707.01932.pdf)
         * [Cognitive Mapping and Planning for Visual Navigation](https://arxiv.org/pdf/1702.03920.pdf)
         * [Using Simulation and Domain Adaptation to Improve Efficiency of Deep Robotic Grasping](https://arxiv.org/pdf/1709.07857.pdf)
   * Physics
      * [Accelerating Eulerian Fluid Simulation with Convolutional Networks](https://arxiv.org/pdf/1607.03597.pdf)
   * Device Placement
      * [Device Placement Optimization with Reinforcement Learning](https://arxiv.org/pdf/1706.04972.pdf)
      * [A Hierarchical Model for Device Placement](https://openreview.net/pdf?id=Hkc-TeZ0W)
   * Games
      * [Can Deep Reinforcement Learning Solve Erdos-Selfridge-Spencer Games?](https://arxiv.org/pdf/1711.02301.pdf)
   * Art
      * [A Neural Representation of Sketch Drawings](https://arxiv.org/pdf/1704.03477.pdf)
3. Unsupervised Learning
   * [Building High-level Features Using Large Scale Unsupervised Learning](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38115.pdf)
   * [Towards Principled Unsupervised Learning](https://arxiv.org/pdf/1511.06440.pdf)
   * [Time-Contrastive Networks: Self-Supervised Learning from Video](https://arxiv.org/pdf/1704.06888.pdf)
   * [Stochastic Variational Video prediction [Also, Model-Based RL]](https://arxiv.org/pdf/1710.11252.pdf)
   * [Short and Deep: Sketching Neural Networks](https://openreview.net/pdf?id=r1br_2Kge)
   * [Geometry-Based Next Frame Prediction from Monocular Video](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45984.pdf)
   * [Decomposing Motion and Content for Natural Video Sequence Prediction](https://sites.google.com/a/umich.edu/rubenevillegas/iclr2017)
   * [Cross-View Training for Semi-Supervised Learning](https://openreview.net/forum?id=BJubPWZRW)
4. Attention
   * [On Learning Where to Look](https://arxiv.org/pdf/1405.5488.pdf)
   * [Pointer Networks](https://arxiv.org/pdf/1506.03134.pdf)
   * [Attention for Fine-Grained Categorization](https://arxiv.org/pdf/1412.7054.pdf)
   * [Listen, Attend and Spell](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44926.pdf)
   * [Collective Entity Resolution with Multi-Focal Attention](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45395.pdf)
   * [Attend, Infer, Repeat: Fast Scene Understanding with Generative Models](https://arxiv.org/pdf/1603.08575.pdf)
   * [Online and Linear-Time Attention by Enforcing Monotonic Alignments](https://research.google.com/pubs/pub46110.html)
   * [Learning Hard Alignments with Variational Inference [Hard Attention]](https://arxiv.org/pdf/1705.05524.pdf)
   * [Efficient Attention using a Fixed-Size Memory Representation](https://arxiv.org/pdf/1707.00110.pdf)
   * [Attention is All You Need](https://arxiv.org/pdf/1706.03762.pdf)
   * [An Analysis of “Attention” in Sequence-to-Sequence Models](http://www.isca-speech.org/archive/Interspeech_2017/pdfs/0232.PDF)
   * [Monotonic Chunkwise Attention](https://openreview.net/pdf?id=Hko85plCW)
5. Memory
   * [Learning to Remember Rare Events](https://openreview.net/pdf?id=SJTQLdqlg)
6. Transfer Learning
   * [Net2Net: Accelerating Learning via Knowledge Transfer](https://arxiv.org/pdf/1511.05641.pdf)
   * [Domain Separation Networks](https://arxiv.org/pdf/1608.06019.pdf)
   * [Unsupervised Pixel-Level Domain Adaptation with Generative Adversarial Networks](https://arxiv.org/pdf/1612.05424.pdf)
   * [PathNet: Evolution Channels Gradient Descent in Super Neural networks](https://arxiv.org/pdf/1701.08734.pdf)
   * [One Model to Learn Them All](https://arxiv.org/pdf/1706.05137.pdf)
   * [Exploring the structure of a real-time, arbitrary neural artistic stylization network](https://arxiv.org/pdf/1705.06830.pdf)
   * [A Brief Study of In-Domain Transfer and Learning from Fewer Samples using a Few Simple Priors](https://arxiv.org/pdf/1707.03979.pdf)
7. Representation Learning
   * [SVCCA: Singular Vector Canonical Correlation Analysis for Deep Learning Dynamics and Interpretability](https://arxiv.org/pdf/1706.05806.pdf)
   * [A Learned Representation for Artistic Style](https://arxiv.org/pdf/1610.07629.pdf)
   * [Learning Latent Permutations with Gumbel-Sinkhorn Networks](https://openreview.net/pdf?id=Byt3oJ-0W)
8. Reinforcemnet Learning
   * Model-Based Reinforcement Learning
      * [Unsupervised Learning for Physical Interaction through Video Prediction [Also, Robotics]](https://arxiv.org/pdf/1605.07157.pdf)
      * [Continuous Deep Q-Learning with Model-based Acceleration](http://proceedings.mlr.press/v48/gu16.pdf)
      * [Value Prediction Network](https://arxiv.org/pdf/1707.03497.pdf)
      * [Learning to Generate Long-term Future via Hierarchical Prediction](https://arxiv.org/pdf/1704.05831.pdf)
      * [Discrete Sequential Prediction of Continuous Actions for Deep RL](https://arxiv.org/pdf/1705.05035.pdf)
      * [Deep Visual Foresight for Planning Robot Motion [Also, Robotics]](https://arxiv.org/pdf/1610.00696.pdf)
      * [Temporal Difference Models: Model-Free Deep RL for Model-Based Control](https://openreview.net/pdf?id=Skw0n-W0Z)
      * [Learning Unsupervised Latent Dynamics Models for Multi-task Continuous Control from Pixels](https://drive.google.com/file/d/1HWDyhEUpVgAiSSQtEYEGb6EIeY8YQay8/view)
   * Multi-Task Learning
      * [Zero-Shot Task Generalization with Multi-Task Deep Reinforcement Learning](https://arxiv.org/pdf/1706.05064.pdf)
   * [Unsupervised Perceptual Rewards for Imitation Learning](https://openreview.net/pdf?id=Byf3mmNFl)
   * [Trust-PCL: An Off-Policy Trust Region Method for Continuous Control](https://arxiv.org/pdf/1707.01891.pdf)
   * [Robust Adversarial Reinforcement Learning [Also, Multi-Agent Systems]](https://arxiv.org/pdf/1703.02702.pdf)
   * [REBAR: Low-Variance, unbiased gradient estimates for discrete latent variable models](https://arxiv.org/pdf/1703.07370.pdf)
   * [Q-Prop: Sample Efficient Policy Gradient with an Off-Policy Critic](https://arxiv.org/pdf/1611.02247.pdf)
   * [Particle Value Functions](https://openreview.net/pdf?id=BJyBKyHKg)
   * [Path Integral Guided Policy Search [Also, Robotics]](https://arxiv.org/pdf/1610.00529.pdf)
   * [Interpolated Policy Gradient: Merging On-Policy and Off-Policy Gradient Estimation for Deep Reinforcement Learning](https://arxiv.org/pdf/1706.00387.pdf)
   * [Improving Policy Gradient by Exploring Under-Appreciated Rewards](https://openreview.net/pdf?id=ryT4pvqll)
   * [Deep Reinforcement Learning for Robotic Manipulation with Asynchronous Off-Policy Updates](https://arxiv.org/pdf/1610.00633.pdf)
   * [Collective Robot Reinforcement Learning with Distributed Asynchronous Guided Policy Search](https://arxiv.org/pdf/1610.00673.pdf)
   * [Changing Model Behavior at Test Time Using Reinforcement Learning](https://arxiv.org/pdf/1702.07780.pdf)
   * [Bridging the Gap Between Value and Policy Based Reinforcement Learning](https://arxiv.org/pdf/1702.08892.pdf)
   * [A comparative study of counterfactual estimators](https://arxiv.org/pdf/1704.00773.pdf)
   * [PRM-RL: Long Range Robotic Navigation Tasks by Combining Reinforcement Learning and Sampling-based Planning](https://arxiv.org/pdf/1710.03937.pdf)
   * [Path consistency Learning in Tsallis Entropy Regularized MDPs](https://arxiv.org/abs/1802.03501)
   * [Leave No Trace: Learning to Reset for Safe and Autonomous Reinforcement Learning](https://openreview.net/pdf?id=S1vuO-bCW)
   * [Deep Bayesian Bandits Showdown](https://openreview.net/pdf?id=SyYe6k-CW)
9. Metalearning
   * Neural Programming
      * [Reinforcement Learning Neural Turing Machines](https://research.google.com/pubs/pub45478.html)
      * [Neural Random-Access Machines](https://research.google.com/pubs/pub45472.html)
      * [Neural Programmer: Inducing Latent Programs with Gradient Descent](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44927.pdf)
      * [Neural GPUs Learn Algorithms](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45139.pdf)
      * [Learning a Natural Language Interface with Neural Programmer](https://arxiv.org/pdf/1611.08945.pdf)
   * Hyperparameter Optimization
      * [Toward Optimal Run Racing: Application to Deep Learning Calibration](https://arxiv.org/pdf/1706.03199.pdf)
      * [Searching for Activation Functions](https://arxiv.org/pdf/1710.05941.pdf)
      * [Neural Optimizer Search with Reinforcement Learning](https://arxiv.org/pdf/1709.07417.pdf)
      * [Neural Combinatorial Optimization with Reinforcement Learning](https://openreview.net/pdf?id=Bk9mxlSFx)
      * [Neural Architecture Search with Reinforcement Learning](https://arxiv.org/pdf/1611.01578.pdf)
      * [Large-Scale Evolution of Image Classifiers](https://arxiv.org/pdf/1703.01041.pdf)
      * [Searching for Activation Functions](https://arxiv.org/pdf/1710.05941.pdf)
    * [Learned Optimizers that Scale and Generalize](https://arxiv.org/pdf/1703.04813.pdf)
    * [HyperNetworks](https://openreview.net/pdf?id=rkpACe1lx)
    * [Supervised Learning of Unsupervised Learning Rules](http://metalearning.ml/papers/metalearn17_metz.pdf)
    * [MorphNet: Fast & Simple Resource-Constrained Structure Learning of Deep Networks](https://arxiv.org/pdf/1711.06798.pdf)
    * [A Meta-Learning Perspective on Cold-Start Recommendations for Items](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46346.pdf)
    * [Meta-Learning for Semi-Supervised Few-Shot Classification](https://openreview.net/pdf?id=HJcSzz-CZ)
    * [Generalizing Hamiltonian Monte Carlo with Neural Networks](https://openreview.net/pdf?id=B1n8LexRZ)
10. Generative
    * GANs
       * [Improved Generator Objectives for GANs](https://arxiv.org/pdf/1612.02780.pdf)
       * [Unrolled Generative Adversarial Networks](https://openreview.net/pdf?id=BydrOIcle)
       * [Improving Image Generative Models with Human Interactions](https://arxiv.org/pdf/1709.10459.pdf)
       * [Conditional Image Synthesis with Auxiliary Classifier GANs](https://arxiv.org/pdf/1610.09585.pdf)
       * [Are GANs Created Equal? A Large-Scale Study](https://arxiv.org/pdf/1711.10337.pdf)
       * [AdaGAN: Boosting Generative Models](https://arxiv.org/pdf/1701.02386.pdf)
       * [MaskGAN: Better Text Generation Via Filling in the _____](https://openreview.net/pdf?id=ByOExmWAb)
       * [Many Paths to Equilibrium: GANs Do Not Need to Decrease a Divergence at Every Step](https://openreview.net/pdf?id=ByQpn1ZA-)
    * [Experiments in Handwriting with a Neural Network](https://distill.pub/2016/handwriting/)
    * [From optimal transport to generative modeling: the VEGAN cookbook](https://arxiv.org/pdf/1705.07642.pdf)
    * [Density Estimation Using Real NVP](https://arxiv.org/pdf/1605.08803.pdf)
    * [A Neural Representation of Sketch Drawings](https://arxiv.org/pdf/1704.03477.pdf)
    * [Wasserstein Auto-Encoders](https://arxiv.org/pdf/1711.01558.pdf)
    * [Stochastic Variational Video Prediction](https://openreview.net/pdf?id=rk49Mg-CW)
    * [Latent Constraints: Learning to Generate Conditionally From Unconditional Generative Models](https://openreview.net/pdf?id=Sy8XvGb0-)
11. Intrepretability
    * [Deconvolution and Checkerboard Artifacts](https://distill.pub/2016/deconv-checkerboard/)
    * [Visualizing Dataflow Graphs of Deep Learning Models in Tensorflow](http://idl.cs.washington.edu/files/2018-TensorFlowGraph-VAST.pdf)
    * [Towards A Rigorous Science of Interpretable Machine Learning](https://arxiv.org/pdf/1702.08608.pdf)
    * [The (Un)reliability of Saliency Methods](https://arxiv.org/pdf/1711.00867.pdf)
    * [Input Switched Affine Networks: An RNN Architecture Designed for Interpretability [Also, Recurrent Neural Networks]](https://arxiv.org/pdf/1611.09434.pdf)
    * [VisualBackProp: Efficient Visualization of CNNs](https://arxiv.org/abs/1611.05418)
    * [Learning How to Explain Neural Networks: PatternNet and PatternAttribution](https://openreview.net/pdf?id=Hkn7CBaTW)
    * [Beyond Word Importance: Contextual Decomposition to Extract Interactions from LSTMs [Also, Recurrent Neural Networks]](https://openreview.net/pdf?id=rkRwGg-0Z)
12. Tools, Environments &amp; Datasets
    * [One Billion Word Benchmark for Measuring Progress in Statistical Language Modeling](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41880.pdf)
13. Adversarial Examples
    * [Intriguing Properties of Neural Networks](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42503.pdf)
    * [Explaining and Harnessing Adversarial Examples](https://arxiv.org/pdf/1412.6572.pdf)
    * [Virtual Adversarial Training for Semi-Supervised Text Classification](https://research.google.com/pubs/pub45403.html)
    * [The Space of Transferable Adversarial Examples](https://arxiv.org/pdf/1704.03453.pdf)
    * [Adversarial Examples in the Physical World](https://arxiv.org/pdf/1607.02533.pdf)
    * [Adversarial Training Methods for Semi-Supervised Text Classification](https://arxiv.org/pdf/1605.07725.pdf)
    * [Adversarial Machine Learning at Scale](https://arxiv.org/pdf/1611.01236.pdf)
    * [Thermometer Encoding: One Hot Way to Resist Adversarial Examples](https://openreview.net/pdf?id=S18Su--CW)
    * [Intriguing Properties of Adversarial Examples](https://arxiv.org/pdf/1711.02846.pdf)
    * [Ensemble Adversarial Training: Attacks and Defences](https://openreview.net/pdf?id=rkZvSe-RZ)
    * [Adversarial Spheres](https://arxiv.org/pdf/1801.02774.pdf)
14. Multi-Agent Systems
    * [Learning to Protect Communications with Adversarial Neural Cryptography](https://arxiv.org/pdf/1610.06918.pdf)
    * [Adversarial Autoencoders](https://arxiv.org/pdf/1511.05644.pdf)
    * [XGAN: Unsupervised Image-To-Image Translation for Many-To-Many Mappings](https://arxiv.org/pdf/1711.05139.pdf)
    * [Supervision via Competition: Robot Adversaries for Learning Tasks](https://arxiv.org/pdf/1610.01685.pdf)
15. Variational Inference
    * [Variational Boosting: Iteratively Refining Posterior Approximations](https://arxiv.org/pdf/1611.06585.pdf)
    * [Reducing Reparameterization Gradient Variance](https://arxiv.org/pdf/1705.07880.pdf)
    * Filtering Variational Objectives
16. Kernel Machines
    * [Fastfood - Approximating Kernel Expansions in Loglinear Time](http://www-cs.stanford.edu/~quocle/LeSarlosSmola_ICML13.pdf)
    * [Random Features for Compositional Kernels](https://arxiv.org/pdf/1703.07872.pdf)
    * [The Geometry of Random Features](http://storage.googleapis.com/pub-tools-public-publication-data/pdf/70a89b15f9b160dd10248de8862d1584f03ddc22.pdf)
17. Collaborative Filtering
    * [Local Collaborative Ranking](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42242.pdf)
18. Graphical / Relational Learning
    * [Large-Scale Object Classification Using Label Relation Graphs](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42854.pdf)
    * [Graph Searching Games and Width Measures for Directed Graphs](http://drops.dagstuhl.de/opus/volltexte/2015/4902/pdf/2.pdf)
    * [Graph Partition Neural Networks for Semi-Supervised Classification](https://arxiv.org/pdf/1803.06272.pdf)
19. Miscellaneous
    * [Tensorflow: Learning Functions at Scale](https://dl.acm.org/citation.cfm?id=2976746)
    * [Deep Learning Games](https://papers.nips.cc/paper/6315-deep-learning-games.pdf)
    * [Tangent: Automatic Differentiation Using Source Code Transformation in Python](https://arxiv.org/pdf/1711.02712.pdf)
    * [ExtDict: Extensible Dictionaries for Data and Platform-Aware Large Scale Learning](http://www.aceslab.org/sites/default/files/main_0.pdf)
    * [Dynamic Routing between Capsules](https://research.google.com/pubs/pub46351.html)
    * [Climbing a Shaky Ladder: Better ADaptive Risk Estimation](https://arxiv.org/pdf/1706.02733.pdf)
    * [Avoiding Discrimination through Causal Reasoning](https://arxiv.org/pdf/1706.02744.pdf)
    * [Who Said What: Modeling Individual Labelers Improves Classification](https://arxiv.org/pdf/1703.08774.pdf)
    * [Matrix Capsules with EM Routing](https://openreview.net/pdf?id=HJWLfGWRb)
    * [Graph sketching-based Space-efficient Data Clustering](http://storage.googleapis.com/pub-tools-public-publication-data/pdf/7174df3a5627e483b5d120d8edb5843fa593577e.pdf)

Major Researchers [10+ Papers / Founding]
   * Jeff Dean
   * Samy Bengio
   * Geoffrey Hinton
   * ~~Andrew Ng~~
   * Quoc Le
   * Greg Corrado
   * Vincent Vanhoucke
   * Yoran Singer
   * Ian Goodfellow
   * ~~Tomas Mikolov~~
   * ~~Ilya Sutskever~~
   * ~~Oriol Vinyals~~
   * ~~Marc’ Aurelio Ranzato~~
   * Christian Szegedy
   * Navdeep Jaitly
   * Mohammad Norouzi
   * Lukasz Kaiser
   * Jonathon Shlens

Minor Researchers
   * Rajat Monga
   * Kai Chen
   * Matthieu Devin
   * Mark Mao
   * Andrew Senior
   * Paul Tucker
   * Ke Yang
   * Patrick Nguyen
   * Dumitru Erhan
   * Eugene Ie
   * Andrew Rabinovich
   * Jon Shlens
   * Yoram Singer
   * Ciprian Chelba
   * Mike Schuster
   * Qi Ge
   * Thorsten Brants
   * Tamas Sarlos
   * Georg Heigold
   * Andrea Frome
   * Maya Gupta
   * David Sussillo
   * Dragonir Anguelov
   * Alexander Toshev
   * Andrew Dai
   * Anelia Angelova
   * Alex Krizhevsky
   * Lucasz Kaiser
   * Terry Koo
   * Slav Petrov
   * Tara Sainath
   * Hasim Sak
   * Pierre Sermanet
   * Esteban Real
   * Peter Liu
   * Sergey Levine
   * Amit Daniely
   * Roy Frostig
   * Martin Abadi
   * Zhifeng Chen
   * Yonghui Wu
   * Dale Schuurmans
   * Jianmin Chen
   * Rafal Jozefowicz
   * Sergey Ioffe
   * Honglak Lee
   * Manjunath Kudlur
   * Karol Kurach
   * Minh-Thang Luong
   * John Nahm
   * Alexander Alemi
   * Jascha Sohl-Dckstein
   * Noam Shazeer
   * David Ha
   * Shan Carter
   * Chris Olah
   * Ignacio Moreno
   * Douglas Eck
   * Natasha Jaques
   * Shixiang Gu
   * Konstantinos Bousmalis
   * Francois Chollet
   * Geoffrey Irving
   * Amarnag Subramanya
   * Michael Ringgaard
   * Fernando Pereira
   * Adam Roberts
   * Cinjon Resnick
   * Anjuli Kannan
   * Ryan Adams
   * David Dohan
   * Luke Metz
   * Kelvin Xu
   * Jan Chorowski
   * Colin Raffel
   * Dieterich Lawson
   * George Papandreou
   * Kevin Murphy
   * Jonathan Tompson
   * Olivier Bousquet
   * Sylvain Gelly
   * Olivier Teytaud
   * Damien Vincent
   * Eric Jang
   * Jasmine Hsu
   * Been Kim
   * Bart van Merrienboer
   * Alexander Wiltschko
   * Dan Moldovan
   * Yuxuan Wang
   * RJ Skerry-Ryan
   * James Davidson
   * Ron Weiss
   * Jan Chorowski
   * Yonghui Wu
   * Zhifeng Chen
   * Kunal Talwar
   * Barret Zoph
   * Maithra Raghu
   * Justin Gilmer
   * Jeffrey Pennington
   * Samuel Schoenholz
   * Gabriel Pereyra
   * George Tucker
   * Vineet Gupta
   * Ryan Dahl
   * Azalia Mirhoseini
   * Andy Davis
   * Ashish Vaswani
   * Krzysztof Maziarz
   * Vikas Sindhwani
   * Irwan Bello
   * Hugo Larochelle
   * Vijay Vasudevan
   * Hieu Pham
   * Jesse Engel
   * Denny Britz
   * Anna Goldie
   * Connor Schenck
   * Ruben Villegas
   * Yuliang Zou
   * Sungryull Sohn
   * Danijar Hafner
   * Alex Irpan
   * James Davidson
   * Chung-Cheng Chiu
   * Kevin Swersky
   * Olga Wichrowska
   * Jakob Forester
   * Andrew Lampinen
   * David So
   * Fred Bertsch
   * Reza Mahjourian
   * Yasaman Bahri
   * Ofir Nachum
   * Melody Guan
   * Julian Ibarz
   * Benoit Steiner
   * Rasmus Larsen
   * Ethan Holly
   * Gal Chechik
   * Augustus Odena
   * Christopher Olah
   * Jasmine Collins
   * Michal Jastrzebski
   * Philip Haeusser
   * Mario Lucic
   * Richard Sproat
   * Alexey Kurakin
   * Takeru Miyato
   * Kristofer Schlachter
   * Tomer Koren
   * Ayush Sekhari
   * Matthew Kelcey
   * Laura Downs

Genealogy
Founding Teams
   * Jeff Dean
   * Samy Bengio
   * Geoffrey Hinton
   * ~~Andrew Ng~~
   * Quoc Le
   * Greg Corrado
   * Vincent Vanhoucke
   * Yoran Singer
   * Ian Goodfellow
   * ~~Tomas Mikolov~~
   * ~~Rajat Monga~~
   * Kai Chen (Brain NY)
   * Matthieu Devin
   * Mark Mao
   * ~~Marc’ Aurelio Ranzato (Brain NY)~~
   * Andrew Senior
   * Paul Tucker
   * Ke Yang
   * Patrick Nguyen
   * Yoram Singer
   * Dzmitry Bahdanau

In the early days, the exploration was mainly in scaling deep learning and discovering new applications to speech recognition, image categorization and language modeling.

Tensorflowers: Mart´ın Abadi, Ashish Agarwal, Paul Barham, Eugene Brevdo, Zhifeng Chen, Craig Citro, Greg S. Corrado, Andy Davis, Jeffrey Dean, Matthieu Devin, Sanjay Ghemawat, Ian Goodfellow, Andrew Harp, Geoffrey Irving, Michael Isard, Yangqing Jia, Rafal Jozefowicz, Lukasz Kaiser, Manjunath Kudlur, Josh Levenberg, Dan Mane, Rajat Monga, Sherry Moore, Derek Murray, ´ Chris Olah, Mike Schuster, Jonathon Shlens, Benoit Steiner, Ilya Sutskever, Kunal Talwar, Paul Tucker, Vincent Vanhoucke, Vijay Vasudevan, Fernanda Viegas, Oriol Vinyals, Pete Warden, Martin Wattenberg, Martin Wicke, Yuan Yu, and Xiaoqiang Zheng

Massive acceleration of Brain papers into ICLR 2016… Tensorflowers start making their way onto papers.

Noisy Counts (Scraped)

[29, 'Oriol Vinyals'],
[27, 'Samy Bengio'],
[23, 'Ilya Sutskever'],
[20, 'Navdeep Jaitly'],
[16, 'Sergey Levine'],
[14, 'Mohammad Norouzi'],1
[14, 'Ian Goodfellow'],
[13, 'Lukasz Kaiser'],
[13, 'Jonathon Shlens'],
[12, 'Vincent Vanhoucke'],
[10, 'Quoc Le'],
[10, 'Geoffrey Hinton'],
[9, 'Dumitru Erhan'],
[8, 'Shixiang Gu'],
[8, 'Rajat Monga'],
[8, 'Honglak Lee'],
[8, 'Greg Corrado'],
[8, 'Christian Szegedy'],
[8, 'Andrew Senior'],
[7, 'Yoram Singer'],
[7, 'Tomas Mikolov'],
[7, 'Sylvain Gelly'],
[7, 'Olivier Bousquet'],
[7, 'Karol Kurach'],
[7, 'Georg Heigold'],
[7, 'Anelia Angelova'],
[6, 'Zhifeng Chen'],
[6, 'Rafal Jozefowicz'],
[6, 'Ofir Nachum'],
[6, 'Matthieu Devin'],
[6, 'Martin Abadi'],
[6, 'James Davidson'],
[6, 'Dieterich Lawson'],
[6, 'Dale Schuurmans'],
[5, 'Yonghui Wu'],
[5, 'Yonghui Wu'],
[5, 'Tara Sainath'],
[5, 'Mike Schuster'],
[5, 'Manjunath Kudlur'],
[5, 'Kevin Murphy'],
[5, 'Justin Gilmer'],
[5, 'George Tucker'],
[5, 'Douglas Eck'],
[4, 'Pierre Sermanet'],
[4, 'Noam Shazeer'],
[4, 'Maithra Raghu'],
[4, 'Kunal Talwar'],
[4, 'Kelvin Xu'],
[4, 'Kai Chen'],
[4, 'Jeff Dean'],
[4, 'Jan Chorowski'],
[4, 'Geoffrey Irving'],
[4, 'David Sussillo'],
[4, 'David Ha'],
[4, 'Colin Raffel'],
[4, 'Chris Olah'],
[4, 'Andrea Frome'],
[4, 'Amit Daniely'],
[4, 'Alexander Toshev'],
[3, 'Vikas Sindhwani'],
[3, 'Vijay Vasudevan'],
[3, 'Tomer Koren'],
[3, 'Paul Tucker'],
[3, 'Patrick Nguyen'],
[3, 'Olivier Teytaud'],
[3, 'Natasha Jaques'],
[3, 'Konstantinos Bousmalis'],
[3, 'Julian Ibarz'],
[3, 'Jonathan Tompson'],
[3, 'Jeffrey Pennington'],
[3, 'Hasim Sak'],
[3, 'Denny Britz'],
[3, 'Damien Vincent'],
[3, 'Benoit Steiner'],
[3, 'Barret Zoph'],
[3, 'Azalia Mirhoseini'],
[3, 'Augustus Odena'],
[3, 'Andy Davis'],
[3, 'Andrew Rabinovich'],
[3, 'Alex Krizhevsky'],
[2, 'Vineet Gupta'],
[2, 'Sergey Ioffe'],
[2, 'Ryan Dahl'],
[2, 'Ruben Villegas'],
[2, 'Roy Frostig'],
[2, 'Peter Liu'],
[2, 'Melody Guan'],
[2, 'Luke Metz'],
[2, 'Ke Yang'],
[2, 'Jianmin Chen'],
[2, 'Irwan Bello'],
[2, 'Hugo Larochelle'],
[2, 'Hieu Pham'],
[2, 'Fred Bertsch'],
[2, 'Francois Chollet'],
[2, 'Esteban Real'],
[2, 'Eric Jang'],
[2, 'Cinjon Resnick'],
[2, 'Been Kim'],
[2, 'Ashish Vaswani'],
[2, 'Anna Goldie'],
[2, 'Anjuli Kannan'],
[2, 'Andrew Dai'],
[2, 'Amarnag Subramanya'],
[2, 'Alexey Kurakin'],
[2, 'Adam Roberts'],
[1, 'Yuxuan Wang'],
[1, 'Yuliang Zou'],
[1, 'Yasaman Bahri'],
[1, 'Thorsten Brants'],
[1, 'Terry Koo'],
[1, 'Tamas Sarlos'],
[1, 'Takeru Miyato'],
[1, 'Sungryull Sohn'],
[1, 'Slav Petrov'],
[1, 'Shan Carter'],
[1, 'Ryan Adams'],
[1, 'Richard Sproat'],
[1, 'Reza Mahjourian'],
[1, 'Rasmus Larsen'],
[1, 'RJ Skerry-Ryan'],
[1, 'Qi Ge'],
[1, 'Philip Haeusser'],
[1, 'Olga Wichrowska'],
[1, 'Michal Jastrzebski'],
[1, 'Mark Mao'],
[1, 'Krzysztof Maziarz'],
[1, 'Kristofer Schlachter'],
[1, 'Kevin Swersky'],
[1, 'Jesse Engel'],
[1, 'Jasmine Hsu'],
[1, 'Jasmine Collins'],
[1, 'Ignacio Moreno'],
[1, 'George Papandreou'],
[1, 'Gal Chechik'],
[1, 'Gabriel Pereyra'],
[1, 'Fernando Pereira'],
[1, 'Eugene Ie'],
[1, 'Ethan Holly'],
[1, 'David Dohan'],
[1, 'Danijar Hafner'],
[1, 'Dan Moldovan'],
[1, 'Connor Schenck'],
[1, 'Ciprian Chelba'],
[1, 'Chung-Cheng Chiu'],
[1, 'Christopher Olah'],
[1, 'Ayush Sekhari'],
[1, 'Andrew Ng'],
[1, 'Andrew Lampinen'],
[1, 'Alex Irpan'],

