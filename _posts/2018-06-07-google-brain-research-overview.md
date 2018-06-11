---
layout: post
title:  "Google Brain Research Overview"
date:   2018-06-07 05:02:46 -0700
categories: machinelearning
---

By Jeremy Nixon [[jnixon2@gmail.com](mailto:jnixon2@gmail.com)]. Nov 2017.

Overview

1. Categorization of Breakthroughs / Contents

2. Major / Minor Researchers List (All appearing on papers)

3. Genealogy

4. Sorted Researchers by Paper Count

1. Deep Learning

    1. Scalability and Speed

    2. Convolutional Neural Networks

    3. Recurrent Neural Networks

    4. Privacy

    5. Understanding / Theory

    6. Regularization

2. Applications

    7. Speech Recognition

    8. Image Categorization

    9. Image Captioning

    10. Machine Translation

    11. Natural Language Understanding

    12. Multi-Modal

    13. Pedestrian Detection

    14. Grasp Detection

    15. Go

    16. Video

    17. Dialogue

    18. 3D Object Reconstruction

    19. Speaker Verification

    20. Health Care

    21. Theorem Proving

    22. Music

    23. Pose Estimation

    24. Speech Generation

    25. Super Resolution

    26. Chemistry

    27. Robotics

        1. Autonomous Vehicles

    28. Physics

    29. Device Placement

    30. Games

    31. Art

3. Unsupervised Learning

4. Attention

5. Memory

6. Transfer Learning

7. Representation Learning

8. Reinforcement Learning

    32. Model-Based Reinforcement Learning

    33. Multi-Task Learning

9. Metalearning

    34. Neural Programming

    35. Hyperparameter Optimization

10. Generative

    36. GANs

11. Interpretability

12. Tools, Environments & Datasets

13. Adversarial Examples

14. Multi-Agent Systems

15. Variational Inference

16. Kernel Machines

17. Collaborative Filtering

18. Graphical / Relational Learning

19. Miscellaneous

1. Deep Learning

    1. Scalability and Speed

        1. Large Scale Distributed Deep Networks
            1. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40565.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40565.pdf)

        2. Multiframe Deep Neural Networks for Acoustic Modeling

            2. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40810.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40810.pdf)

        3. Asynchronous Stochastic Optimization for Sequence Training of Deep Neural Networks

            3. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42248.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42248.pdf)

        4. Tensorflow: Large-Scale Machine Learning on Heterogeneous Distributed Systems

            4. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45166.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45166.pdf)

        5. Distilling the Knowledge in a Neural Network

            5. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44873.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44873.pdf)

        6. Deep Networks with Large Output Spaces

            6. [https://arxiv.org/pdf/1412.7479.pdf](https://arxiv.org/pdf/1412.7479.pdf)

        7. TensorFlow: A System for Large-Scale Machine Learning

            7. [https://www.usenix.org/system/files/conference/osdi16/osdi16-abadi.pdf](https://www.usenix.org/system/files/conference/osdi16/osdi16-abadi.pdf)

        8. Revisiting Distributed Synchronous SGD

            8. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45187.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45187.pdf)

        9. Depthwise Separable Convolutions for Neural Machine Translation

            9. [https://arxiv.org/abs/1706.03059](https://arxiv.org/abs/1706.03059)

        10. Large Scale Distributed Neural Network Training Through Online Distillation

            10. [https://openreview.net/pdf?id=rkr1UDeC-](https://openreview.net/pdf?id=rkr1UDeC-)

        11. Deep Gradient Compression: Reducing the Communication Bandwidth for Distributed Training

            11. https://openreview.net/pdf?id=SkhQHMW0W

    2. Convolutional Neural Networks

        12. Going Deeper with Convolutions [Inception]

            12. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43022.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43022.pdf)

        13. Rethinking the Inception Architecture for Computer Vision

            13. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44903.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44903.pdf)

        14. Inception-v4, Inception-ResNet and the Impact of Residual Connections on Learning

            14. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45169.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45169.pdf)

        15. Towards Understanding the Invertibility of Convolutional Neural Networks

            15. https://arxiv.org/pdf/1705.08664.pdf

    3. Recurrent Neural Networks

        16. Sequence to Sequence Learning with Neural Networks

            16. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43155.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43155.pdf)

        17. Sequence Discriminative Distributed Training of Long Short-Term Memory Recurrent Neural Networks

            17. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42547.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42547.pdf)

        18. Recurrent Neural Network Regularization [Also, Language Modeling]

            18. [https://arxiv.org/abs/1409.2329](https://arxiv.org/abs/1409.2329)

        19. Semi-supervised Sequence Learning

            19. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44267.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44267.pdf)

        20. Learning to Execute

            20. [https://research.google.com/pubs/pub45474.html](https://research.google.com/pubs/pub45474.html)

        21. An Empirical Exploration of Recurrent Network Architectures

            21. [https://research.google.com/pubs/pub45473.html](https://research.google.com/pubs/pub45473.html)

        22. A Simple Way to Initialize Recurrent Networks of Rectified Linear Units

            22. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44961.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44961.pdf)

        23. Using Fast Weights to Attend to the Recent Past

            23. [https://arxiv.org/pdf/1610.06258.pdf](https://arxiv.org/pdf/1610.06258.pdf)

        24. Unsupervised Pre-training for Sequence to Sequence Learning

            24. [https://arxiv.org/pdf/1611.02683.pdf](https://arxiv.org/pdf/1611.02683.pdf)

        25. Order Matters: Sequence to Sequence for Sets

            25. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44871.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44871.pdf)`

        26. Multi-Task Sequence to Sequence Learning

            26. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44928.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44928.pdf)

        27. Generating Sentences from a Continuous Space

            27. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45404.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45404.pdf)

        28. Exponential expressivity in deep neural networks through transient chaos

            28. [https://arxiv.org/pdf/1606.05340.pdf](https://arxiv.org/pdf/1606.05340.pdf)

        29. An Online Sequence-to-Sequence Model Using Partial Conditioning

            29. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45167.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45167.pdf)

        30. A Neural Transducer

            30. [https://arxiv.org/pdf/1511.04868.pdf](https://arxiv.org/pdf/1511.04868.pdf)

        31. Tuning Recurrent Neural Networks with Reinforcement Learning

            31. [https://openreview.net/pdf?id=Syyv2e-Kx](https://openreview.net/pdf?id=Syyv2e-Kx)

        32. Sequence Tutor: Conservative Fine-Tuning of Sequence Generation Models with KL-control

            32. [https://arxiv.org/pdf/1611.02796.pdf](https://arxiv.org/pdf/1611.02796.pdf)

        33. SGD Learns the Conjugate Kernel Class of the Network	

            33. [https://arxiv.org/pdf/1702.08503.pdf](https://arxiv.org/pdf/1702.08503.pdf)

        34. Learning Hierarchical Information Flow with Recurrent Neural Modules

            34. [https://arxiv.org/pdf/1706.05744.pdf](https://arxiv.org/pdf/1706.05744.pdf)

        35. Latent Sequence Decompositions

            35. [https://arxiv.org/pdf/1610.03035.pdf](https://arxiv.org/pdf/1610.03035.pdf)

        36. Capacity and Trainability in Recurrent Neural Networks

            36. [https://openreview.net/pdf?id=BydARw9ex](https://openreview.net/pdf?id=BydARw9ex)

        37. Initialization Matters: Orthogonal Predictive State Recurrent Neural Networks

            37. https://openreview.net/pdf?id=HJJ23bW0b

    4. Privacy

        38. Deep Learning with Differential Privacy

            38. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45428.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45428.pdf)

        39. Semi-Supervised Knowledge Transfer for Deep Learning from Private Training Data

            39. [https://arxiv.org/pdf/1610.05755.pdf](https://arxiv.org/pdf/1610.05755.pdf)

        40. Glimmers: Resolving the Privacy / Trust Quagmire

            40. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46128.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46128.pdf)

        41. Scalable Private Learning with PATE

            41. [https://arxiv.org/pdf/1802.08908.pdf](https://arxiv.org/pdf/1802.08908.pdf)

        42. Learning Differentially Private Recurrent Language Models [Also, Language Modeling]

            42. https://openreview.net/pdf?id=BJ0hF1Z0b

    5. Understanding / Theory

        43. Qualitatively Characterizing Neural Network Optimization Problems

            43. [https://arxiv.org/pdf/1412.6544.pdf](https://arxiv.org/pdf/1412.6544.pdf)

        44. Toward Deeper Understanding of Neural Networks: The Power of Initialization and a Dual View on Expressivity

            44. [https://arxiv.org/pdf/1602.05897.pdf](https://arxiv.org/pdf/1602.05897.pdf)

        45. Understanding Deep Learning Requires Re-Thinking Generalization

            45. [https://arxiv.org/pdf/1611.03530.pdf](https://arxiv.org/pdf/1611.03530.pdf)

        46. Sharp Minima Can Generalize for Deep Nets

            46. [https://arxiv.org/pdf/1703.04933.pdf](https://arxiv.org/pdf/1703.04933.pdf)

        47. On the Expressive Power of Deep Neural Networks

            47. [https://arxiv.org/pdf/1606.05336.pdf](https://arxiv.org/pdf/1606.05336.pdf)

        48. Nonlinear Random Matrix Theory for Deep Learning

            48. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46342.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46342.pdf)

        49. Mean Field Residual Networks: On the Edge of Chaos

            49. [http://papers.nips.cc/paper/6879-mean-field-residual-networks-on-the-edge-of-chaos.pdf](http://papers.nips.cc/paper/6879-mean-field-residual-networks-on-the-edge-of-chaos.pdf)

        50. Identity Matters in Deep Learning

            50. [https://arxiv.org/pdf/1611.04231.pdf](https://arxiv.org/pdf/1611.04231.pdf)

        51. Geometry of Neural Network Loss Surfaces via Random Matrix Theory

            51. [http://proceedings.mlr.press/v70/pennington17a/pennington17a.pdf](http://proceedings.mlr.press/v70/pennington17a/pennington17a.pdf)

        52. Explaining the Learning Dynamics of Direct Feedback Alignment

            52. [https://openreview.net/pdf?id=HkXKUTVFl](https://openreview.net/pdf?id=HkXKUTVFl)

        53. Deep Information Propagation

            53. [https://openreview.net/pdf?id=H1W1UN9gg](https://openreview.net/pdf?id=H1W1UN9gg)

        54. The Emergence of Spectral Universality in Deep Networks

            54. [https://arxiv.org/pdf/1802.09979.pdf](https://arxiv.org/pdf/1802.09979.pdf)

        55. Sensitivity and Generalization in Neural Networks: An Empirical Study

            55. [https://arxiv.org/pdf/1802.08760.pdf](https://arxiv.org/pdf/1802.08760.pdf)

        56. Gradient Descent with identity initialization efficiently learns positive definite linear transformations by deep residual networks

            56. [https://arxiv.org/pdf/1802.06093.pdf](https://arxiv.org/pdf/1802.06093.pdf)

        57. Deep Neural Networks as Gaussian Processes

            57. [https://openreview.net/pdf?id=B1EA-M-0Z](https://openreview.net/pdf?id=B1EA-M-0Z)

        58. A Bayesian Perspective on Generalization and Stochastic Gradient Descent

            58. [https://openreview.net/pdf?id=BJij4yg0Z](https://openreview.net/pdf?id=BJij4yg0Z)

    6. Regularization

        59. Adding Gradient Noise Improves Learning for Very Deep Networks

            59. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45137.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45137.pdf)

        60. Surprising Properties of Dropout in Deep Networks

            60. [http://www.phillong.info/publications/HL17_deep_dropout.pdf](http://www.phillong.info/publications/HL17_deep_dropout.pdf)

        61. Regularizing Neural Networks by Penalizing Confident Output Distributions

            61. [https://arxiv.org/pdf/1701.06548.pdf](https://arxiv.org/pdf/1701.06548.pdf)

        62. A Unified Approach to Adaptive Regularization in Online and Stochastic Optimization

            62. https://arxiv.org/pdf/1706.06569.pdf

    7. Training Highly Multiclass Classifiers

        63. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41872.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41872.pdf)

    8. Random Walk Initialization for Training Very Deep Feedforward Networks

        64. [https://arxiv.org/pdf/1412.6558.pdf](https://arxiv.org/pdf/1412.6558.pdf)

    9. Learning Factored Representations in a Deep Mixture of Experts

        65. [https://arxiv.org/pdf/1312.4314.pdf](https://arxiv.org/pdf/1312.4314.pdf)

    10. Training Deep Neural Networks on Noisy Labels with Bootstrapping

        66. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43273.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43273.pdf)

    11. Convolutional, Long Short-Term Memory, Fully Connected Deep Neural Networks

        67. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43455.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43455.pdf)

    12. Reward Augmented Maximum Likelihood for Neural Structured Prediction

        68. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45580.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45580.pdf)

    13. MuProp: Unbiased Backpropagation for Stochastic Neural Networks

        69. [https://arxiv.org/pdf/1511.05176v3.pdf](https://arxiv.org/pdf/1511.05176v3.pdf)

    14. Chained predictions using convolutional neural networks

        70. [https://research.google.com/pubs/pub45945.html](https://research.google.com/pubs/pub45945.html)

    15. Training a Subsampling Mechanism in Expectation

        71. [https://openreview.net/pdf?id=BJBkkaNYe](https://openreview.net/pdf?id=BJBkkaNYe)

    16. Resurrecting the Sigmoid in deep learning through dynamical isometry: theory and practice

        72. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46341.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46341.pdf)

    17. Outrageously Large Neural Networks: The Sparsely-Gated Mixture-of-Experts Layer

        73. [https://openreview.net/pdf?id=B1ckMDqlg](https://openreview.net/pdf?id=B1ckMDqlg)

    18. On Blackbox Backpropagation and Jacobian Sensing

        74. [https://research.google.com/pubs/pub46347.html](https://research.google.com/pubs/pub46347.html)

    19. Deep Value Networks Learn to Evaluate and Iteratively Refine Structured Outputs

        75. [https://arxiv.org/pdf/1703.04363.pdf](https://arxiv.org/pdf/1703.04363.pdf)

    20. Critical Hyper-Parameters: No Random, No Cry

        76. [https://arxiv.org/pdf/1706.03200.pdf](https://arxiv.org/pdf/1706.03200.pdf)

    21. Distilling a Neural Network into a Soft Decision Tree

        77. [https://arxiv.org/pdf/1711.09784.pdf](https://arxiv.org/pdf/1711.09784.pdf)

    22. Categorical Reparameterization with Gumbel-Softmax

        78. [https://arxiv.org/pdf/1611.01144.pdf](https://arxiv.org/pdf/1611.01144.pdf)

    23. Training Confidence-Calibrated Classifiers For Detecting Out-of-Distribution Samples

        79. [https://openreview.net/pdf?id=ryiAv2xAZ](https://openreview.net/pdf?id=ryiAv2xAZ)

    24. Fidelity-Weighted Learning

        80. [https://openreview.net/pdf?id=B1X0mzZCW](https://openreview.net/pdf?id=B1X0mzZCW)

    25. Don’t Decay the Learning Rate, Increase the Batch Size

        81. https://openreview.net/pdf?id=B1Yy1BxCZ

2. Applications

    26. Speech Recognition

        82. Deep Neural Networks for Acoustic Modeling in Speech Recognition

            63. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38131.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38131.pdf)

        83. Application of Pre-trained Deep Neural Networks to Large Vocabulary Speech Recognition

            64. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38130.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38130.pdf)

        84. On Rectified Linear Units for Speech Processing

            65. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40811.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40811.pdf)

        85. Multilingual Acoustic Models Using Distributed Deep Neural Networks

            66. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40807.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40807.pdf)

        86. An Empirical Study of Learning Rates in DNNs for Speech Recognition

            67. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40808.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/40808.pdf)

        87. Word Embeddings for Speech Recognition

            68. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42543.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42543.pdf)

        88. Autoregressive product of multi-frame predictions can improve the accuracy of hybrid models

            69. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42947.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42947.pdf)

        89. Learning the Speech Front-end with Raw Waveform CLDNNs

            70. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43960.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43960.pdf)

        90. Acoustic Modeling for Google Home

            71. [http://www.cs.cmu.edu/~chanwook/MyPapers/b_li_interspeech_2017.pdf](http://www.cs.cmu.edu/~chanwook/MyPapers/b_li_interspeech_2017.pdf)

        91. Multilingual Speech Recognition With a Single End-to-End Model

            72. [https://arxiv.org/pdf/1711.01694.pdf](https://arxiv.org/pdf/1711.01694.pdf)

        92. An Analysis of Incorporating an External Language Model into a Sequence-to-Sequence Model

            73. https://arxiv.org/pdf/1712.01996.pdf

    27. Image Classification

        93. Using Web Co-occurrence Statistics for Improving Image Categorization

            74. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42244.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42244.pdf)

        94. The Unreasonable Effectiveness of Noisy Data for Fine-Grained Recognition

            75. [https://arxiv.org/pdf/1511.06789.pdf](https://arxiv.org/pdf/1511.06789.pdf)

    28. Image Captioning

        95. Grounded Compositional Semantics for Finding and Describing Images with Sentences

            76. [https://nlp.stanford.edu/~socherr/SocherKarpathyLeManningNg_TACL2013.pdf](https://nlp.stanford.edu/~socherr/SocherKarpathyLeManningNg_TACL2013.pdf)

        96. Show and Tell: A Neural Image Caption Generator

            77. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43274.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43274.pdf)

        97. Learning Semantic Relationships for Better Action Retrieval in Images

            78. https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43443.pdf

    29. Machine Translation

        98. Exploiting Similarities among Languages for Machine Translation

            79. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44931.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44931.pdf)

        99. Addressing the Rare Word Problem in Neural Machine Translation

            80. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44929.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44929.pdf)

        100. Google’s Neural Machine Translation System: Bridging the Gap between Human and Machine Translation

            81. [https://arxiv.org/abs/1609.08144](https://arxiv.org/abs/1609.08144)

        101. Sequence-to-Sequence Models Can Directly Translate Foreign Speech

            82. [https://arxiv.org/pdf/1703.08581.pdf](https://arxiv.org/pdf/1703.08581.pdf)

        102. Massive Exploration of Neural Machine Translation Architectures

            83. https://arxiv.org/pdf/1703.03906.pdf

    30. Natural Language Understanding

        103. Efficient Estimation of Word Representations in Vector Space

            84. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41224.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41224.pdf)

        104. Distributed Representations of Words and Their Compositionality

            85. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44876.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44876.pdf)

        105. Zero-Shot Learning by Convex Combination of Semantic Embeddings

            86. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42371.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42371.pdf)

        106. Distributed Representations of Sentences and Documents

            87. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44930.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44930.pdf)

        107. Sentence Compression by Deletion with LSTMs

            88. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43852.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43852.pdf)

        108. Grammar as a Foreign Language

            89. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43799.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43799.pdf)

        109. BilBOWA: Fast Bilingual Distributed Representations without Word Alignments

            90. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45190.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45190.pdf)

        110. Multilingual Language Processing From Bytes

            91. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45170.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45170.pdf)

        111. Exploring the Limits of Language Modeling

            92. [https://arxiv.org/pdf/1602.02410.pdf](https://arxiv.org/pdf/1602.02410.pdf)

        112. Towards better decoding and language model integration in sequence to sequence models

            93. [https://arxiv.org/pdf/1612.02695.pdf](https://arxiv.org/pdf/1612.02695.pdf)

        113. Learning to Skim Text

            94. [https://arxiv.org/pdf/1704.06877.pdf](https://arxiv.org/pdf/1704.06877.pdf)

        114. Get To The Point: Summarization with Pointer-Generator Networks

            95. [https://arxiv.org/pdf/1704.04368.pdf](https://arxiv.org/pdf/1704.04368.pdf)

        115. Generating Wikipedia by Summarizing Long Sequences

            96. [https://openreview.net/pdf?id=Hyg0vbWC-](https://openreview.net/pdf?id=Hyg0vbWC-)

        116. An Efficient Framework for Learning Sentence Representations

            97. https://openreview.net/pdf?id=rJvJXZb0W

    31. Multi-Modal

        117. DeViSE: A Deep Visual-Semantic Embedding Model

            98. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41869.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41869.pdf)

        118. Modulating Early Visual Processing by Language

            99. [https://arxiv.org/pdf/1707.00683.pdf](https://arxiv.org/pdf/1707.00683.pdf)

        119. Context-aware Captions from Context-agnostic Supervision

            100. [http://openaccess.thecvf.com/content_cvpr_2017/papers/Vedantam_Context-Aware_Captions_From_CVPR_2017_paper.pdf](http://openaccess.thecvf.com/content_cvpr_2017/papers/Vedantam_Context-Aware_Captions_From_CVPR_2017_paper.pdf)

        120. Better Text Understanding Through Image-To-Text Transfer

            101. https://arxiv.org/pdf/1705.08386.pdf

    32. Pedestrian Detection

        121. Real Time Pedestrian Detection with Deep Network Cascades

            102. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43850.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43850.pdf)

        122. Pedestrian Detection with a Large Field-Of-View Deep Network

            103. https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43849.pdf

    33. Grasp Detection

        123. Real-Time Grasp Detection Using Convolutional Neural Networks

            104. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43875.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43875.pdf)

    34. Go

        124. Move Evaluation in Go Using Deep Convolutional Neural Networks

            105. [https://arxiv.org/pdf/1412.6564.pdf](https://arxiv.org/pdf/1412.6564.pdf)

        125. Mastering the game of Go with deep neural networks and tree search

            106. https://www.nature.com/articles/nature16961

    35. Video

        126. Beyond Short Snippets: Deep Networks for Video Classification

            107. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43793.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/43793.pdf)

    36. Dialogue

        127. A Neural Conversational Model

            108. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44925.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44925.pdf)

        128. Smart Reply: Automated Response Suggestion for Email

            109. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45189.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45189.pdf)

        129. Adversarial Evaluation of Dialogue Models

            110. [https://arxiv.org/pdf/1701.08198.pdf](https://arxiv.org/pdf/1701.08198.pdf)

        130. Generating High-Quality and Informative Conversation Responses with Sequence-to-Sequence Models

            111. https://arxiv.org/pdf/1701.03185.pdf

    37. 3D Object Reconstruction

        131. [https://arxiv.org/pdf/1612.00814.pdf](https://arxiv.org/pdf/1612.00814.pdf)

    38. Speaker Verification

        132. End-to-End Text-Dependent Speaker Verification

            112. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44681.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44681.pdf)

    39. Health Care

        133. Development and Validation of a Deep Learning Algorithm for Detection of Diabetic Retinopathy in Retinal Fundus Photographs

            113. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45732.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45732.pdf)

    40. Theorem Proving

        134. DeepMath - Deep Sequence Models for Premise Selection

            114. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45402.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45402.pdf)

        135. Deep Network Guided Proof Search

            115. https://arxiv.org/pdf/1701.06972.pdf

    41. Music

        136. Audio Deepdream: Optimizing Raw Audio with Convolutional Networks

            116. https://18798-presscdn-pagely.netdna-ssl.com/ismir2016/wp-content/uploads/sites/2294/2016/08/ardila-audio.pdf

        137. Generating Music by Fine-Tuning Recurrent Neural Networks with Reinforcement Learning

            117. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45871.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45871.pdf)

        138. Neural Audio Synthesis of Musical Notes with WaveNet Autoencoders

            118. https://arxiv.org/pdf/1704.01279.pdf

    42. Pose Estimation

        139. Towards Accurate Multi-person Pose Estimation in the Wild

            119. [https://arxiv.org/pdf/1701.01779.pdf](https://arxiv.org/pdf/1701.01779.pdf)

    43. Speech Generation

        140. Tacotron: Towards End-to-End Speech Synthesis

            120. [https://arxiv.org/pdf/1703.10135.pdf](https://arxiv.org/pdf/1703.10135.pdf)

        141. RNN Approaches to Text Normalization: A Challenge

            121. [https://arxiv.org/pdf/1611.00068.pdf](https://arxiv.org/pdf/1611.00068.pdf)

        142. On Using Backpropagation for Speech texture Generation and Voice Cnversion

            122. [https://arxiv.org/pdf/1712.08363.pdf](https://arxiv.org/pdf/1712.08363.pdf)

        143. Natural TTS Synthesis by Conditioning Wavenet on Mel Spectrogram Prediction [Tacotron 2]

            123. https://arxiv.org/pdf/1712.05884.pdf

    44. Super Resolution

        144. Pixel Recursive Super Resolution

            124. [https://arxiv.org/pdf/1702.00783.pdf](https://arxiv.org/pdf/1702.00783.pdf)

    45. Chemistry

        145. Neural Message Passing for Quantum Chemistry

            125. [https://arxiv.org/pdf/1704.01212.pdf](https://arxiv.org/pdf/1704.01212.pdf)

    46. Robotics

        146. Autonomous Vehicles

            126. Learning with Proxy Supervision for End-To-End Visual Learning

                1. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45985.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45985.pdf)

        147. Learning Robotic Manipulation of Granular Media

            127. [https://arxiv.org/pdf/1709.02833.pdf](https://arxiv.org/pdf/1709.02833.pdf)

        148. Learning hand-eye coordination for robotic grasping with deep learning and large-scale data collection

            128. [https://drive.google.com/file/d/0B0mFoBMu8f8BaHYzOXZMdzVOalU/view](https://drive.google.com/file/d/0B0mFoBMu8f8BaHYzOXZMdzVOalU/view)

        149. End-to-End Learning of Semantic Grasping

            129. [https://arxiv.org/pdf/1707.01932.pdf](https://arxiv.org/pdf/1707.01932.pdf)

        150. Cognitive Mapping and Planning for Visual Navigation

            130. [https://arxiv.org/pdf/1702.03920.pdf](https://arxiv.org/pdf/1702.03920.pdf)

        151. Using Simulation and Domain Adaptation to Improve Efficiency of Deep Robotic Grasping

            131. https://arxiv.org/pdf/1709.07857.pdf

    47. Physics

        152. Accelerating Eulerian Fluid Simulation with Convolutional Networks

            132. [https://arxiv.org/pdf/1607.03597.pdf](https://arxiv.org/pdf/1607.03597.pdf)

    48. Device Placement

        153. Device Placement Optimization with Reinforcement Learning

            133. [https://arxiv.org/pdf/1706.04972.pdf](https://arxiv.org/pdf/1706.04972.pdf)

        154. A Hierarchical Model for Device Placement

            134. [https://openreview.net/pdf?id=Hkc-TeZ0W](https://openreview.net/pdf?id=Hkc-TeZ0W)

    49. Games

        155. Can Deep Reinforcement Learning Solve Erdos-Selfridge-Spencer Games?

            135. [https://arxiv.org/pdf/1711.02301.pdf](https://arxiv.org/pdf/1711.02301.pdf)

    50. Art

        156. A Neural Representation of Sketch Drawings

            136. https://arxiv.org/pdf/1704.03477.pdf

3. Unsupervised Learning

    51. Building High-level Features Using Large Scale Unsupervised Learning

        157. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38115.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/38115.pdf)

    52. Towards Principled Unsupervised Learning

        158. [https://arxiv.org/pdf/1511.06440.pdf](https://arxiv.org/pdf/1511.06440.pdf)

    53. Time-Contrastive Networks: Self-Supervised Learning from Video

        159. [https://arxiv.org/pdf/1704.06888.pdf](https://arxiv.org/pdf/1704.06888.pdf)

    54. Stochastic Variational Video prediction [Also, Model-Based RL]

        160. [https://arxiv.org/pdf/1710.11252.pdf](https://arxiv.org/pdf/1710.11252.pdf)

    55. Short and Deep: Sketching Neural Networks

        161. [https://openreview.net/pdf?id=r1br_2Kge](https://openreview.net/pdf?id=r1br_2Kge)

    56. Geometry-Based Next Frame Prediction from Monocular Video

        162. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45984.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45984.pdf)

    57. Decomposing Motion and Content for Natural Video Sequence Prediction

        163. [https://sites.google.com/a/umich.edu/rubenevillegas/iclr2017](https://sites.google.com/a/umich.edu/rubenevillegas/iclr2017)

    58. Cross-View Training for Semi-Supervised Learning

        164. https://openreview.net/forum?id=BJubPWZRW

4. Attention

    59. On Learning Where to Look

        165. [https://research.google.com/pubs/pub45477.html](https://research.google.com/pubs/pub45477.html)

    60. Pointer Networks

        166. [https://arxiv.org/pdf/1506.03134.pdf](https://arxiv.org/pdf/1506.03134.pdf)

    61. Attention for Fine-Grained Categorization

        167. [https://arxiv.org/pdf/1412.7054.pdf](https://arxiv.org/pdf/1412.7054.pdf)

    62. Listen, Attend and Spell

        168. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44926.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44926.pdf)

    63. Collective Entity Resolution with Multi-Focal Attention

        169. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45395.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45395.pdf)

    64. Attend, Infer, Repeat: Fast Scene Understanding with Generative Models

        170. [https://arxiv.org/pdf/1603.08575.pdf](https://arxiv.org/pdf/1603.08575.pdf)

    65. Online and Linear-Time Attention by Enforcing Monotonic Alignments

        171. [https://research.google.com/pubs/pub46110.html](https://research.google.com/pubs/pub46110.html)

    66. Learning Hard Alignments with Variational Inference [Hard Attention]

        172. [https://arxiv.org/pdf/1705.05524.pdf](https://arxiv.org/pdf/1705.05524.pdf)

    67. Efficient Attention using a Fixed-Size Memory Representation

        173. [https://arxiv.org/pdf/1707.00110.pdf](https://arxiv.org/pdf/1707.00110.pdf)

    68. Attention is All You Need

        174. [https://arxiv.org/pdf/1706.03762.pdf](https://arxiv.org/pdf/1706.03762.pdf)

    69. An Analysis of "Attention" in Sequence-to-Sequence Models

        175. [http://www.isca-speech.org/archive/Interspeech_2017/pdfs/0232.PDF](http://www.isca-speech.org/archive/Interspeech_2017/pdfs/0232.PDF)

    70. Monotonic Chunkwise Attention

        176. https://openreview.net/pdf?id=Hko85plCW

5. Memory

    71. Learning to Remember Rare Events

        177. https://openreview.net/pdf?id=SJTQLdqlg

6. Transfer Learning

    72. Net2Net: Accelerating Learning via Knowledge Transfer

        178. [https://arxiv.org/pdf/1511.05641.pdf](https://arxiv.org/pdf/1511.05641.pdf)

    73. Domain Separation Networks

        179. [https://arxiv.org/pdf/1608.06019.pdf](https://arxiv.org/pdf/1608.06019.pdf)

    74. Unsupervised Pixel-Level Domain Adaptation with Generative Adversarial Networks

        180. [https://arxiv.org/pdf/1612.05424.pdf](https://arxiv.org/pdf/1612.05424.pdf)

    75. PathNet: Evolution Channels Gradient Descent in Super Neural networks

        181. [https://arxiv.org/pdf/1701.08734.pdf](https://arxiv.org/pdf/1701.08734.pdf)

    76. One Model to Learn Them All

        182. [https://arxiv.org/pdf/1706.05137.pdf](https://arxiv.org/pdf/1706.05137.pdf)

    77. Exploring the structure of a real-time, arbitrary neural artistic stylization network

        183. [https://arxiv.org/pdf/1705.06830.pdf](https://arxiv.org/pdf/1705.06830.pdf)

    78. A Brief Study of In-Domain Transfer and Learning from Fewer Samples using a Few Simple Priors

        184. https://arxiv.org/pdf/1707.03979.pdf

7. Representation Learning

    79. SVCCA: Singular Vector Canonical Correlation Analysis for Deep Learning Dynamics and Interpretability

        185. [https://arxiv.org/pdf/1706.05806.pdf](https://arxiv.org/pdf/1706.05806.pdf)

    80. A Learned Representation for Artistic Style

        186. [https://arxiv.org/pdf/1610.07629.pdf](https://arxiv.org/pdf/1610.07629.pdf)

    81. Learning Latent Permutations with Gumbel-Sinkhorn Networks

        187. https://openreview.net/pdf?id=Byt3oJ-0W

8. Reinforcement Learning

    82. Model-Based Reinforcement Learning

        188. Unsupervised Learning for Physical Interaction through Video Prediction [Also, Robotics]

            137. [https://arxiv.org/pdf/1605.07157.pdf](https://arxiv.org/pdf/1605.07157.pdf)

        189. Continuous Deep Q-Learning with Model-based Acceleration

            138. [http://proceedings.mlr.press/v48/gu16.pdf](http://proceedings.mlr.press/v48/gu16.pdf)

        190. Value Prediction Network

            139. [https://arxiv.org/pdf/1707.03497.pdf](https://arxiv.org/pdf/1707.03497.pdf)

        191. Learning to Generate Long-term Future via Hierarchical Prediction

            140. [https://arxiv.org/pdf/1704.05831.pdf](https://arxiv.org/pdf/1704.05831.pdf)

        192. Discrete Sequential Prediction of Continuous Actions for Deep RL

            141. [https://arxiv.org/pdf/1705.05035.pdf](https://arxiv.org/pdf/1705.05035.pdf)

        193. Deep Visual Foresight for Planning Robot Motion [Also, Robotics]

            142. [https://arxiv.org/pdf/1610.00696.pdf](https://arxiv.org/pdf/1610.00696.pdf)

        194. Temporal Difference Models: Model-Free Deep RL for Model-Based Control

            143. [https://openreview.net/pdf?id=Skw0n-W0Z](https://openreview.net/pdf?id=Skw0n-W0Z)

    83. Multi-Task Learning

        195. Zero-Shot Task Generalization with Multi-Task Deep Reinforcement Learning

            144. [https://arxiv.org/pdf/1706.05064.pdf](https://arxiv.org/pdf/1706.05064.pdf)

    84. Unsupervised Perceptual Rewards for Imitation Learning

        196. [https://openreview.net/pdf?id=Byf3mmNFl](https://openreview.net/pdf?id=Byf3mmNFl)

    85. Trust-PCL: An Off-Policy Trust Region Method for Continuous Control

        197. [https://arxiv.org/pdf/1707.01891.pdf](https://arxiv.org/pdf/1707.01891.pdf)

    86. Robust Adversarial Reinforcement Learning [Also, Multi-Agent Systems]

        198. [https://arxiv.org/pdf/1703.02702.pdf](https://arxiv.org/pdf/1703.02702.pdf)

    87. REBAR: Low-Variance, unbiased gradient estimates for discrete latent variable models

        199. [https://arxiv.org/pdf/1703.07370.pdf](https://arxiv.org/pdf/1703.07370.pdf)

    88. Q-Prop: Sample Efficient Policy Gradient with an Off-Policy Critic

        200. [https://arxiv.org/pdf/1611.02247.pdf](https://arxiv.org/pdf/1611.02247.pdf)

    89. Particle Value Functions

        201. [https://openreview.net/pdf?id=BJyBKyHKg](https://openreview.net/pdf?id=BJyBKyHKg)

    90. Path Integral Guided Policy Search [Also, Robotics]

        202. [https://arxiv.org/pdf/1610.00529.pdf](https://arxiv.org/pdf/1610.00529.pdf)

    91. Interpolated Policy Gradient: Merging On-Policy and Off-Policy Gradient Estimation for Deep Reinforcement Learning

        203. [https://arxiv.org/pdf/1706.00387.pdf](https://arxiv.org/pdf/1706.00387.pdf)

    92. Improving Policy Gradient by Exploring Under-Appreciated Rewards

        204. [https://openreview.net/pdf?id=ryT4pvqll](https://openreview.net/pdf?id=ryT4pvqll)

    93. Deep Reinforcement Learning for Robotic Manipulation with Asynchronous Off-Policy Updates

        205. [https://arxiv.org/pdf/1610.00633.pdf](https://arxiv.org/pdf/1610.00633.pdf)

    94. Collective Robot Reinforcement Learning with Distributed Asynchronous Guided Policy Search

        206. [https://arxiv.org/pdf/1610.00673.pdf](https://arxiv.org/pdf/1610.00673.pdf)

    95. Changing Model Behavior at Test Time Using Reinforcement Learning

        207. [https://arxiv.org/pdf/1702.07780.pdf](https://arxiv.org/pdf/1702.07780.pdf)

    96. Bridging the Gap Between Value and Policy Based Reinforcement Learning

        208. [https://arxiv.org/pdf/1702.08892.pdf](https://arxiv.org/pdf/1702.08892.pdf)

    97. A comparative study of counterfactual estimators

        209. [https://arxiv.org/pdf/1704.00773.pdf](https://arxiv.org/pdf/1704.00773.pdf)

    98. PRM-RL: Long Range Robotic Navigatio nTasks by Combining Reinforcement Learning and Sampling-based Planning

        210. [https://arxiv.org/pdf/1710.03937.pdf](https://arxiv.org/pdf/1710.03937.pdf)

    99. Path consistency Learning in Tsallis Entropy Regularized MDPs

        211. [https://arxiv.org/abs/1802.03501](https://arxiv.org/abs/1802.03501)

    100. Leave No Trace: Learning to Reset for Safe and Autonomous Reinforcement Learning

        212. [https://openreview.net/pdf?id=S1vuO-bCW](https://openreview.net/pdf?id=S1vuO-bCW)

    101. Deep Bayesian Bandits Showdown

        213. https://openreview.net/pdf?id=SyYe6k-CW

9. Metalearning

    102. Neural Programming

        214. Reinforcement Learning Neural Turing Machines

            145. [https://research.google.com/pubs/pub45478.html](https://research.google.com/pubs/pub45478.html)

        215. Neural Random-Access Machines

            146. [https://research.google.com/pubs/pub45472.html](https://research.google.com/pubs/pub45472.html)

        216. Neural Programmer: Inducing Latent Programs with Gradient Descent

            147. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44927.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/44927.pdf)

        217. Neural GPUs Learn Algorithms

            148. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45139.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/45139.pdf)

        218. Learning a Natural Language Interface with Neural Programmer

            149. https://arxiv.org/pdf/1611.08945.pdf

    103. Hyperparameter Optimization

        219. Toward Optimal Run Racing: Application to Deep Learning Calibration

            150. [https://arxiv.org/pdf/1706.03199.pdf](https://arxiv.org/pdf/1706.03199.pdf)

        220. Searching for Activation Functions

            151. [https://arxiv.org/pdf/1710.05941.pdf](https://arxiv.org/pdf/1710.05941.pdf)

        221. Neural Optimizer Search with Reinforcement Learning

            152. [https://arxiv.org/pdf/1709.07417.pdf](https://arxiv.org/pdf/1709.07417.pdf)

        222. Neural Combinatorial Optimization with Reinforcement Learning

            153. [https://openreview.net/pdf?id=Bk9mxlSFx](https://openreview.net/pdf?id=Bk9mxlSFx)

        223. Neural Architecture Search with Reinforcement Learning

            154. [https://arxiv.org/pdf/1611.01578.pdf](https://arxiv.org/pdf/1611.01578.pdf)

        224. Large-Scale Evolution of Image Classifiers

            155. [https://arxiv.org/pdf/1703.01041.pdf](https://arxiv.org/pdf/1703.01041.pdf)

        225. Searching for Activation Functions

            156. https://arxiv.org/pdf/1710.05941.pdf

    104. Learned Optimizers that Scale and Generalize

        226. [https://arxiv.org/pdf/1703.04813.pdf](https://arxiv.org/pdf/1703.04813.pdf)

    105. HyperNetworks

        227. [https://openreview.net/pdf?id=rkpACe1lx](https://openreview.net/pdf?id=rkpACe1lx)

    106. Supervised Learning of Unsupervised Learning Rules

        228. [http://metalearning.ml/papers/metalearn17_metz.pdf](http://metalearning.ml/papers/metalearn17_metz.pdf)

    107. MorphNet: Fast & Simple Resource-Constrained Structure Learning of Deep Networks

        229. [https://arxiv.org/pdf/1711.06798.pdf](https://arxiv.org/pdf/1711.06798.pdf)

    108. A Meta-Learning Perspective on Cold-Start Recommendations for Items

        230. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46346.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/46346.pdf)

    109. Meta-Learning for Semi-Supervised Few-Shot Classification

        231. [https://openreview.net/pdf?id=HJcSzz-CZ](https://openreview.net/pdf?id=HJcSzz-CZ)

    110. Generalizing Hamiltonian Monte Carlo with Neural Networks

        232. https://openreview.net/pdf?id=B1n8LexRZ

10. Generative

    111. GANs

        233. Improved Generator Objectives for GANs

            157. [https://arxiv.org/pdf/1612.02780.pdf](https://arxiv.org/pdf/1612.02780.pdf)

        234. Unrolled Generative Adversarial Networks

            158. [https://openreview.net/pdf?id=BydrOIcle](https://openreview.net/pdf?id=BydrOIcle)

        235. Improving Image Generative Models with Human Interactions

            159. [https://arxiv.org/pdf/1709.10459.pdf](https://arxiv.org/pdf/1709.10459.pdf)

        236. Conditional Image Synthesis with Auxiliary Classifier GANs

            160. [https://arxiv.org/pdf/1610.09585.pdf](https://arxiv.org/pdf/1610.09585.pdf)

        237. Are GANs Created Equal? A Large-Scale Study

            161. [https://arxiv.org/pdf/1711.10337.pdf](https://arxiv.org/pdf/1711.10337.pdf)

        238. AdaGAN: Boosting Generative Models

            162. [https://arxiv.org/pdf/1701.02386.pdf](https://arxiv.org/pdf/1701.02386.pdf)

        239. MaskGAN: Better Text Generation Via Filling in the _____

            163. [https://openreview.net/pdf?id=ByOExmWAb](https://openreview.net/pdf?id=ByOExmWAb)

        240. Many Paths to Equilibrium: GANs Do Not Need to Decrease a Divergence at Every Step

            164. https://openreview.net/pdf?id=ByQpn1ZA-

    112. Experiments in Handwriting with a Neural Network

        241. [https://distill.pub/2016/handwriting/](https://distill.pub/2016/handwriting/)

    113. From optimal transport to generative modeling: the VEGAN cookbook

        242. [https://arxiv.org/pdf/1705.07642.pdf](https://arxiv.org/pdf/1705.07642.pdf)

    114. Density Estimation Using Real NVP

        243. [https://arxiv.org/pdf/1605.08803.pdf](https://arxiv.org/pdf/1605.08803.pdf)

    115. A Neural Representation of Sketch Drawings

        244. [https://arxiv.org/pdf/1704.03477.pdf](https://arxiv.org/pdf/1704.03477.pdf)

    116. Wasserstein Auto-Encoders

        245. [https://arxiv.org/pdf/1711.01558.pdf](https://arxiv.org/pdf/1711.01558.pdf)

    117. Stochastic Variational Video Prediction

        246. [https://openreview.net/pdf?id=rk49Mg-CW](https://openreview.net/pdf?id=rk49Mg-CW)

    118. Latent Constraints: Learning to Generate Conditionally From Unconditional Generative Models

        247. https://openreview.net/pdf?id=Sy8XvGb0-

11. Interpretability

    119. Deconvolution and Checkerboard Artifacts

        248. [https://distill.pub/2016/deconv-checkerboard/](https://distill.pub/2016/deconv-checkerboard/)

    120. Visualizing Dataflow Graphs of Deep Learning Models in Tensorflow

        249. [http://idl.cs.washington.edu/files/2018-TensorFlowGraph-VAST.pdf](http://idl.cs.washington.edu/files/2018-TensorFlowGraph-VAST.pdf)

    121. Towards A Rigorous Science of Interpretable Machine Learning

        250. [https://arxiv.org/pdf/1702.08608.pdf](https://arxiv.org/pdf/1702.08608.pdf)

    122. The (Un)reliability of Saliency Methods

        251. [https://arxiv.org/pdf/1711.00867.pdf](https://arxiv.org/pdf/1711.00867.pdf)

    123. Input Switched Affine Networks: An RNN Architecture Designed for Interpretability [Also, Recurrent Neural Networks]

        252. [https://arxiv.org/pdf/1611.09434.pdf](https://arxiv.org/pdf/1611.09434.pdf)

    124. VisualBackProp: Efficient Visualization of CNNs

        253. [https://arxiv.org/abs/1611.05418](https://arxiv.org/abs/1611.05418)

    125. Learning How to Explain Neural Networks: PatternNet and PatternAttribution

        254. [https://openreview.net/pdf?id=Hkn7CBaTW](https://openreview.net/pdf?id=Hkn7CBaTW)

    126. Beyond Word Importance: Contextual Decomposition to Extract Interactions from LSTMs [Also, Recurrent Neural Networks]

        255. https://openreview.net/pdf?id=rkRwGg-0Z

12. Tools, Environments & Datasets

    127. One Billion Word Benchmark for Measuring Progress in Statistical Language Modeling

        256. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41880.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/41880.pdf)

13. Adversarial Examples

    128. Intriguing Properties of Neural Networks

        257. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42503.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42503.pdf)

    129. Explaining and Harnessing Adversarial Examples

        258. [https://arxiv.org/pdf/1412.6572.pdf](https://arxiv.org/pdf/1412.6572.pdf)

    130. Virtual Adversarial Training for Semi-Supervised Text Classification

        259. [https://research.google.com/pubs/pub45403.html](https://research.google.com/pubs/pub45403.html)

    131. The Space of Transferable Adversarial Examples

        260. [https://arxiv.org/pdf/1704.03453.pdf](https://arxiv.org/pdf/1704.03453.pdf)

    132. Adversarial Examples in the Physical World

        261. [https://arxiv.org/pdf/1607.02533.pdf](https://arxiv.org/pdf/1607.02533.pdf)

    133. Adversarial Training Methods for Semi-Supervised Text Classification

        262. [https://arxiv.org/pdf/1605.07725.pdf](https://arxiv.org/pdf/1605.07725.pdf)

    134. Adversarial Machine Learning at Scale

        263. [https://arxiv.org/pdf/1611.01236.pdf](https://arxiv.org/pdf/1611.01236.pdf)

    135. Thermometer Encoding: One Hot Way to Resist Adversarial Examples

        264. [https://openreview.net/pdf?id=S18Su--CW](https://openreview.net/pdf?id=S18Su--CW)

    136. Intriguing Properties of Adversarial Examples

        265. [https://arxiv.org/pdf/1711.02846.pdf](https://arxiv.org/pdf/1711.02846.pdf)

    137. Ensemble Adversarial Training: Attacks and Defences

        266. [https://openreview.net/pdf?id=rkZvSe-RZ](https://openreview.net/pdf?id=rkZvSe-RZ)

    138. Adversarial Spheres

        267. https://arxiv.org/pdf/1801.02774.pdf

14. Multi-Agent Systems

    139. Learning to Protect Communications with Adversarial Neural Cryptography

        268. [https://arxiv.org/pdf/1610.06918.pdf](https://arxiv.org/pdf/1610.06918.pdf)

    140. Adversarial Autoencoders

        269. [https://arxiv.org/pdf/1511.05644.pdf](https://arxiv.org/pdf/1511.05644.pdf)

    141. XGAN: Unsupervised Image-To-Image Translation for Many-To-Many Mappings

        270. [https://arxiv.org/pdf/1711.05139.pdf](https://arxiv.org/pdf/1711.05139.pdf)

    142. Supervision via Competition: Robot Adversaries for Learning Tasks

        271. https://arxiv.org/pdf/1610.01685.pdf

15. Variational Inference

    143. Variational Boosting: Iteratively Refining Posterior Approximations

        272. [https://arxiv.org/pdf/1611.06585.pdf](https://arxiv.org/pdf/1611.06585.pdf)

    144. Reducing Reparameterization Gradient Variance

        273. [https://arxiv.org/pdf/1705.07880.pdf](https://arxiv.org/pdf/1705.07880.pdf)

    145. Filtering Variational Objectives

16. Kernel Machines

    146. Fastfood - Approximating Kernel Expansions in Loglinear Time

        274. [http://www-cs.stanford.edu/~quocle/LeSarlosSmola_ICML13.pdf](http://www-cs.stanford.edu/~quocle/LeSarlosSmola_ICML13.pdf)

    147. Random Features for Compositional Kernels

        275. [https://arxiv.org/pdf/1703.07872.pdf](https://arxiv.org/pdf/1703.07872.pdf)

    148. The Geometry of Random Features

        276. http://storage.googleapis.com/pub-tools-public-publication-data/pdf/70a89b15f9b160dd10248de8862d1584f03ddc22.pdf

17. Collaborative Filtering

    149. Local Collaborative Ranking

        277. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42242.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42242.pdf)

18. Graphical / Relational Learning

    150. Large-Scale Object Classification Using Label Relation Graphs

        278. [https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42854.pdf](https://static.googleusercontent.com/media/research.google.com/en//pubs/archive/42854.pdf)

    151. Graph Searching Games and Width Measures for Directed Graphs

        279. [http://drops.dagstuhl.de/opus/volltexte/2015/4902/pdf/2.pdf](http://drops.dagstuhl.de/opus/volltexte/2015/4902/pdf/2.pdf)

    152. Graph Partition Neural Networks for Semi-Supervised Classification

        280. https://arxiv.org/pdf/1803.06272.pdf

19. Miscellaneous

    153. Tensorflow: Learning Functions at Scale

        281. [https://dl.acm.org/citation.cfm?id=2976746](https://dl.acm.org/citation.cfm?id=2976746)

    154. Deep Learning Games

        282. [https://papers.nips.cc/paper/6315-deep-learning-games.pdf](https://papers.nips.cc/paper/6315-deep-learning-games.pdf)

    155. Tangent: Automatic Differentiation Using Source Code Transformation in Python

        283. [https://arxiv.org/pdf/1711.02712.pdf](https://arxiv.org/pdf/1711.02712.pdf)

    156. ExtDict: Extensible Dictionaries for Data and Platform-Aware Large Scale Learning

        284. [http://www.aceslab.org/sites/default/files/main_0.pdf](http://www.aceslab.org/sites/default/files/main_0.pdf)

    157. Dynamic Routing between Capsules

        285. [https://research.google.com/pubs/pub46351.html](https://research.google.com/pubs/pub46351.html)

    158. Climbing a Shaky Ladder: Better ADaptive Risk Estimation

        286. [https://arxiv.org/pdf/1706.02733.pdf](https://arxiv.org/pdf/1706.02733.pdf)

    159. Avoiding Discrimination through Causal Reasoning

        287. [https://arxiv.org/pdf/1706.02744.pdf](https://arxiv.org/pdf/1706.02744.pdf)

    160. Who Said What: Modeling Individual Labelers Improves Classification

        288. [https://arxiv.org/pdf/1703.08774.pdf](https://arxiv.org/pdf/1703.08774.pdf)

    161. Matrix Capsules with EM Routing

        289. [https://openreview.net/pdf?id=HJWLfGWRb](https://openreview.net/pdf?id=HJWLfGWRb)

    162. Graph sketching-based Space-efficient Data Clustering

        290. http://storage.googleapis.com/pub-tools-public-publication-data/pdf/7174df3a5627e483b5d120d8edb5843fa593577e.pdf

Major Researchers [10+ Papers / Founding]

* Jeff Dean

* Samy Bengio

* Geoffrey Hinton

* Andrew Ng

* Quoc Le

* Greg Corrado

* Vincent Vanhoucke

* Yoran Singer

* Ian Goodfellow

* Tomas Mikolov

* Ilya Sutskever

* Oriol Vinyals

* Marc’ Aurelio Ranzato

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

Founding Team

* Jeff Dean

* Samy Bengio

* Geoffrey Hinton

* Andrew Ng

* Quoc Le

* Greg Corrado

* Vincent Vanhoucke

* Yoran Singer

* Ian Goodfellow

* Tomas Mikolov

* Rajat Monga

* Kai Chen (Brain NY)

* Matthieu Devin

* Mark Mao

* Marc’ Aurelio Ranzato (Brain NY)

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

