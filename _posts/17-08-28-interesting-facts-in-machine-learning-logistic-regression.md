---
layout: post
title:  "12 Interesting Facts in Machine Learning (Logistic Regression)"
date: 2017-08-28
categories:
---
1. Two major ways to do multinomial eval:
    * Softmax Loss
    * One vs. All with binary (logistic) function
2. Naming - 
   * “Logistic” regression due to Sigmoid (logistic) function
   * “Softmax” regression due to softmax function
3. No closed form solution, despite convexity
   * Newton / Newton-CG
   * BFGS
       * L-BFGS
   * IRLS
   * Trust Region Conjugate Gradient
   * Gradient Descent
       * GD + Line Search
   * Stochastic Average Gradient
4. Many, many optimizers:
5. Difficult Bayesian Solutions (No convenient conjugate prior)
6. Discriminative (Learns P(Y|X), rather than first the joint P(Y, X) and then conditioning on X (the generative approach))
7. Without regularization, the weights will become arbitrary large, damaging generalization. Penalties are more important than in the regression setting.
8. You can get better generalization with a stochastic solver. Reference: [Data-driven advice for applying machine learning to bioinformatics problems](https://arxiv.org/pdf/1708.05070.pdf)
9. The reason scaling can still be important is for the optimizer - even though you technically have a convex model and will get the same solution
10. Linear generalization is stronger than almost every other form of generalization for unstructured data (trees + networks overfit)
11. Every relationship between your feature and the label should be as close to linear as possible
12. You can use boxcox transform to automatically get close to linear