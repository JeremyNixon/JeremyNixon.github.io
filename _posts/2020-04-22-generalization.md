---
layout: post
title:  "Generalization"
date:   2020-04-22
categories: thinking
---


What is generalization?

The critical property of an abstraction is its ability to generalize. What is the scope of its context? How cleanly does it adhere to reality, both in scope and out of scope? What flagrant misuses of the abstraction are likely? What natural safties, gramatical or otherwise, are built in?

Within a domain, learning often looks like generalization - in sports, you pattern match one situation to similar past situations, and react instinctively in a way that your intuition hopes will lead to success. In mathematics, solving a problem with an algebraic manipulation once lets you recognize that type of manipulation in other situations. And often so you abstract the manipulation into a rule or into an operation that you can run more flexibly.

But you’d also like to do out of domain generalization - learn something in one context and apply it to an entirely different context. Learning language in one domain (say, in a home) and then applying it at school, or with friends rather than parents, or in speeches. Take the concept of specialization and lift it from economics to understanding sexual dimorphism in evolution. Taking the concepts of a replicator and differential selection from evolution and apply it to ideas and tunes and fashions that replicate by imitation. (add something about decomposition, modularity, causality)

Generalization as a Standard

Generalization accuracy is a great standard to hold abstractions to. What we want is for our representations to aid us in problem solving, which often takes the form of prediction what the impact of our actions will be or predicting what the state of our system will be in future.

When adjudicating between representations and when constructing them, we’ll optimize for the representation that is easy to evaluate (simplicity heuristic) and that makes the most accurate predictions. And simplicity is also a part of accuracy - models that are simpler have the advantages of capturing more data (because in general they’re more abstract), being more robust to small differences between observations and so better able to capture the higher level regularity, and being straightforward to update when they’re mistaken.

Tradeoffs need to be adjudicated, and so having a downstream task to determine the appropriate lines for those tradeoffs is invaluable. Yet in practice people use other standards either as proxies for generalization or to preserve longer term value - truth is a classic example. Instead of asking if a representation is predictive, you can ask how closely it corresponds to reality via some similarity metric between your map of the territory and the territory. Often there are tradeoffs between the true model and the model that leads to the best generalization accuracy. 

Even generalization accuracy should be seen as an intermediate standard or proxy, with utility as the true goal. And perhaps we should resolve the tension between predictive accuracy and utility in favor of utility. Many models or pieces of information that improve predictive accuracy do dramatic damage to agent utility (ex., noble lies - rights, objective grounding to values, sacred & religious beliefs, etc.). It’s not clear that the metric we want to evaluate these pieces of information over with is predictive accuracy, and so that evaluation needs to happen in a decision function that adjudicates between standards based on their contribution to utility.

What is Transfer?

A central part of the efficient use of models is their generality. Generality means that a model works across many tasks and domains, and a so a central component of an intelligent worldview is the ability to recognize and model shared structure. This flexibility allows us to deal with unforeseen problems efficiently, by co-opting ideas and models that are already well fit by world experience and leveraging them for the task at hand. It also lets us compress the information in our world model. But there’s also this wonderful exponential structure to composing models of systems that lets us counter the exponential complexity of the problems we face. 

Transfer is identifying shared structure between objects of ideas or domains, and assuming that additional information that you have about one domain will generalize to being true of the other domain.

All machine learning is transfer. Transfer is the ‘identical’ in identical and independently distributed. At a low level, we have transfer between datapoints which leads to a standard machine learning model. It’s transfer between datasets that we usually refer to as transfer, but that’s simply a level of abstraction above the datapoint level.

Distributions can be closer to or farther from one another. Overfitting classically refers to an inability to ‘generalize’ to data drawn from the exact same distribution. We also need some conception of generality of models to distributions that are of different data but that have a similar structure

There are two major components to Transfer. The first is the recognition that transfer is possible - the recognition of shared structure between domains. The second is the application of a model whose properties were learned in one domain to another domain. 

Abstraction and transfer are connected because the transfer between domains generally demands that the model be learned at the proper level of abstraction. The model can always be a memorization of the data that exists in that domain, and at that level it will be very difficult to transfer it to a new domain. 

For example, say that you’re trying to determine the proper sorted order of 1-n. You’re given a few lists of numbers, and shown that after the sort they all go to 1-n. You may think of sorting, but you could also only learn that the data you’ve seen goes to the particular n-length vector you see. Trained at a low level, your model for this system will perform perfectly on the information you’ve seen thusfar. But it’s the wrong level of abstraction if you want it to generalize. When we move up, to a sorting function, we gain the ability to generalize ‘internally’, where data is generated from the same distribution as the old and we still get the sorted output correct - this won’t happen if we just memorize instances seen before, unless we look at every possible combination. But the concept of sorting itself can generalize to other problems - say, choosing the closest neighbors from a set of distances in kNN. 

What gets transferred? The information gained from training on some domain / ask, which is stored in a model, gets transferred to a new domain.

Using language forces analogy / transfer over all domains - to describe a situation, we have to build a model in order to use words to describe things. And that brings in information from every other instance of the modular words used to describe the situation. Which makes it much harder to memorize the particular task at hand. Instead, we have to map it to a known structure, and in so doing transfer structure and models to it. Say you tell someone “I’m having trouble deciding what my course load should be.” The word ‘load’ brings in information about resource use and the heaviness implies there is a cost to be optimized or minimized. The word ‘decision’ implies that a set of models needs to be applied to it. You can barely describe the problem without transferring information to it.

The Recognition of Shared Structure

The recognition of shared structure is what allows transfer to happen. Shared structure can come in many forms. Often, fields are formed around the shared structure in some set of problems, and then a body of techniques are built to flexibly solve those problems. 

A great example is in economics - there is shared structure in resource allocation problems. Take opportunity cost. It can be applied to any situation where there are scarce resources being allocated that are associated with actions that lead to some utility. 

There’s this story where I want to finish my monthly goals, but it’s late and swing dancing starts soon. If I go to swing I can’t finish my goals - the opportunity cost to my going to swing becomes finishing these goals. At a very low level, I could take a lesson away from this which is extremely specific. Swing dancing leads to forgone goal setting. One form of learning looks like memorizing that relationship.

There’s a more abstract form of learning that comes out of abstracting, introducing time to the picture. There’s time that I won’t have to work on goals if I’m dancing. If I abstract at that level, I can take the lesson that time will make actions mutually exclusive - I can’t do one if I do the other. At that level, I can learn about other situations from this one. Any case where I spend time on one thing, it gets lost to being spent at another thing. And I can learn about the tradeoff from time in the context of swing dancing vs. goal setting and apply it to a number of other situations, thus achieving transfer.

I can amplify that transfer even more by pushing to a higher level of abstraction. Abstracting up from time to resource, I can realize that this mutual exclusivity / scarcity framework works on money and on energy (oil, gas, nuclear), works on computer memory and human memory, attention, and so on. The breadth of impact that a discovery in any of these spaces can have on the others is a function of our ability to abstract to the appropriate level to recognize the shared structure that exists around them.
