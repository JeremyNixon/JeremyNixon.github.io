---
layout: post
title:  "Abstraction"
date:   2010-01-21
___

#Abstraction
##On Information and its Representation
Abstraction	1
Table of Contents	3
True Draft	3
Similarity	3
Compression	7
Unstructured Content	7
Opening	7
Book Summary	8
Definitions	8
Transfer	11
Compression	13
Temporal Abstraction & Causality	13
Explicating an Example	14
Application: Learning	15
Creating New Abstractions	15
Similarity / Distance	16
Value of Representations	21
Compositionality	22
Generalization	23
Alignment of Representation over Shared Structure	25
Abstraction of Reality as Business	25
Examples	26
Structure as Abstraction over Relationships	29
Clean vs. Dirty	34
Valuable Properties of Representations	36
Abstraction as Religion	37
Abstraction to Transcendence	39
Tradeoff Between Concept-relevant data and Precision	40
Ways in Which Abstraction is Done	42
Difficulties in Thinking About Abstraction	43
Terms, How People Talk about Abstraction	44
Bias Variance	47
Abstraction and Systems Thinking	50
Beautiful Example of Shared Structure in Systems	50
Search as Abstraction	51
Fundamental Questions in Representation Learning	52
Notes & Thoughts	55
Book Organization	59
Potential chapters	60
Potential Interactions:	63
Properties of Thought & Information Processing	63
Citations	65
Reading List	66
Old Draft	66
Old Draft Table of Contents	66
What is Abstraction?	68
Introduction	68
How to Think About Abstraction - Abstraction as an Abstraction	69
Hierarchical Compression	70
Shared Structure	71
Pure Abstractions	71
Transfer, Across Definitions	71
Types of Abstraction	73
Examples	73
Base Unit	73
Consistency	73
Discreteness vs. Continuity	74
Terms, How People Talk about Abstraction	74
Power	75
Transfer and Generalization	75
What is transfer?	76
What is generalization?	76
Generalization as a Standard	77
Implicit Transfer	77
Glorious Heights of Representation	78
Pitfalls	78
Transfer and Generalization	78
Information Loss	79
Conflation, Unlike Objects & False Transfer	79
Excessive Height	80
Abstraction as an Unseen Assumption	81
Lack of Grounding	81

Table of Contents

True Draft
Similarity

Similarity, Distance, and Memorization

This is so so long in the making.

Think about: Distance and intuitive physics

Continuum of similarity:
Discrete
Equality / Identicality
Property overlap
Edit Distance
Continuous
Euclidean Distance
Angles
Cosine Distance
KL Divergence

Think about a distance metric between shapes. Humans have an intuitive sense of the similarity between shapes, as a part of a general ability to judge the similarity of any two objects in an undefined intuitive space. But writing down that metric is incredibly difficult. And so much of the mission of representation learning research is learning how to compare arbitrary objects to one another through a distance metric that’s learned from experiencing arbitrary data. 

Similarity is at the core of all learning and cognition. Neuroscience side, an example is the heuristic that ‘neurons that fire together, wire together’, connecting sets of data that are similar in that they occur close by in the time series that a mind experiences. It also leverages another notion of similarity - if a and b there are previous patterns that are established, those previous patterns a’ associated with the firing of a will also be associated with b. This transitivity quickly becomes a wonderfully nuanced and complex form of similarity.

In developing knowledge, there’s a value to the knowledge that will generalize. Memorization is fine if you know that the data you see in future will be identical to the data that you’re seeing now. But there’s a continuum over the richness of similarity metrics, where memorization can be defined as the way similarity breaks down a short distance from the datapoints that have been memorized (or an inability to return an answer when you’re a short distance away). We get beyond memorization by finding ways to map similar datapoints to one another, and through that connection drawing conclusions about the properties that those similar datapoints will share (this depends on the ways in which the objects are similar) and is stronger than memorization in that when you encounter new information that hasn’t been seen before, you can compare it to that which you’ve already seen and use that history to inform your understanding of this new experience.

Often memorization looks like a lookup, which is fragile. If you don’t find something that’s exactly equal to what you’ve seen in the past, you can’t return anything. The more effectively you can connect a new experience to a vast array of old experiences, the more data you’ll have to draw on when you make inferences about it.

One implication is that broadening the types of connection that you make between objects allows you to transfer more information and connect more types of object. Seeing more of an objects properties creates a larger surface for comparison, enriching the kinds of connection you can make between your object and others.

As you move to a more expressive and nuanced similarity metric (ex. from binaries to a continuum, say from whether a person is good or not to how good a person is) the distortions that come from conflating datapoints that are relatively close but not identical with each other can disappear. But the tradeoff to eliminating that conflation is needing to store a much more complex representation of goodness for every person (and likely move from an intentional, deliberate process for thinking about it to an intuitive one).

Properties of data that make certain kinds of similarity metric more relevant:

Imagine trying to use edit distance for semantics, where you tried to map words’ conceptual similarity to the number of changes you’d need to make to the letters in one word to get to another word. The lack of overlap between a word’s spelling and its meaning makes this notion of similarity irrelevant. 
But instead, imaging looking at the similarity of the contexts in which words appear. Specifically, say, the number of occurrences of a small 2-5 word window of surrounding words. Suddenly, words with similar contexts and meanings can be mapped to each other - ex. Cat and dog are often used with similar surrounding words, and so will be close to one another. King and queen are also used with similar surrounding words. And when they differ, they tend to differ in a way that has to do with the meaning of the words. So distance on this similarity metric is meaningful in ways that aren’t captured by edit distance. The design of distance metrics that capture the structure that matters for a task is extremely important. 

Implication:
Languages need to merge semantics with 
A language that merged its word / letter representation with the actual meaning of the words (where, say, base sounds / letters represented the principal components of learned word vectors) wouldn’t require memorization to learn because the mapping from concepts to reality would be on a continuum and its meaning grounded in the language itself rather than being an arbitrary mapping from a word to a concept.

Generator:
Why does language learning require so much memorization? In general, needing to memorize indicates that you’re using a degenerate distance metric and that your learning will fail to generalize. 


Similarity 1.0

What is this ‘shared structure’?

Underlying the concept of ‘shared’ is a notion of similarity.

Closeness to equality.

Question:
Are all forms of similarity captured by 'how much you have to change the object to get equivalence?, and where equivalence is "these objects are the same"?"


Topics:
Relationship of abstraction to similarity	
One type of abstraction identifies shared structure across objects and compresses it into a single concept or abstract object.


Similarity as existing over different features
Type of similarity as a function of the nature of the thing being compared
Types of similarity measures
Discrete:
Equivalence
Edit Distance
Number of properties in common
(Having a property in common is similarity over that property)
Continuous:
Cosine Distance
Euclidean Distance
KL Divergence / Cross Entropy
Wasserstein Distance
Hinge Loss
Generating Similarity Metrics
Concept Representations
Word Embeddings, same up to angle
Networks
PCA over learned representation
Types of Similarity
Have the same function / accomplish the same task, consequently
Laptop is actually a functional abstraction, more than a compressive technique over sub-parts.
But it also cares about the sub-parts… the surface and ipad are functionally similar but are called ‘tablets’ instead of ‘laptops’.
Use the same mechanism
Have the same property
Ex. shape, color, density
Have a set of shared properties
Question: Are all forms of similarity captured by 'how much you have to change the object to get equivalence?, and where equivalence is "these objects are the same"?"
Cognitive Fit, human notions of concept similarity

Relationship of Abstraction to Similarity
Similarity is a foundational concept that forms the basis of the ability to compress information across objects. When objects are similar, whether it be in their properties, or their constituent parts, or in their function, it becomes possible to transfer information from one object to another via awareness of this shared structure. 
In the extreme case where objects are identical or equal, we can compressive massively - we can throw out one of the objects, and merely remember that it’s equal to the other object. On the continuum away from equal, we lose compressive power in that we have to trade the compactness of our representation of the object against the amount of new information that the object holds.
As an example, it’s often much easier to store a deviation from an existing object that to construct an entirely new object. Say, this is like headphones without the wires (for bluetooth headphones), rather than inventing a new name entirely. This is a phone, but smart. That modification of an existing representation is transferable across people who have the existing representation, and is compact in the amount of new information that exists (only the deviation). In the same way that human attention is drawn merely to what changes in the environment (and in general things that are unchanging fade out of awareness), representing new information as a deviation from an old representation is a classic example of efficiently taking advantage of similarity.

Similarity Over Different Features
Similarity can operate over all the features of an object. It’s often the case that features are intercorrelated, and so when enough features intercorrelate we tend to create a term or concept for that body of relationships. When objects are similar over one feature but not in others, there’s often conflation or confusion when an attempt to generalize from the workings of one object to another fails.

We can think of similarity over different features as often having very different properties - being measured in different ways, allowing or disallowing transfer in different ways, etc.


Measuring Similarity
There are a body of metrics for measuring similarity - the classic example is equality. When two systems are equal, they reflect one another perfectly. There’s no information in one system that isn’t reflected in the other system. And so we can do heavy compression. But equality is binary - the objects are either equal or not. And so it’s not granular enough to capture shared structure that is incomplete. Equality strongly limits the complexity of the objects that can be compared to one another, and so looser metrics are critical to modeling real systems.

notes


Difficulty in describing continuous similarity, distributional similarity. Similar difficulty in describing distinctions, or breakages of similarity in distributions. General difficulty of reasoning outside of discrete space. Need for cognitive fit.




Types of Similarity
Difference from Equivalence (Shared structure over metrics)
Cognitive Fit (Similarity in human intuition)


Compression
Unstructured Content

Opening

Abstraction’s power is to allow the wielder to represent huge amounts of information in a single object. Layers of abstraction allow the entire universe to be summarized by a single node, on top of a hierarchy of lower level representations. The tool is dangerous, making ideas inaccessible and hiding distorted information. It’s foundational to the way that we think. This book is about how Abstraction operates. How it allows us to create, to analogize, and to build knowledge out of information.

Representing Information

Abstraction itself is a wonderful example of abstraction. From the child learning language to a college student studying category theory to a computer scientist designing a representation of the world, the term covers a staggeringly large span of tools and techniques across all modalities of thinking about reality.

When fields develop their own language to build ideas on top of one another, we see abstraction at work. The delineation of fields themselves are but an abstraction, one that attempts to create clarity and allow us to summarize and specialize and focus. But also one that separates ideas from one another. 

Elaborate on scientific fields as abstractions that let us represent huge amounts of information under them. And transfer between them.
Book Summary
It’s called Abstraction. It’s about the way that compression allows us to climb to the heights of abstraction, encapsulation hilarious amounts of information into a single concept. About the way that we load our language with these concepts, implicitly transferring information across umpteen experiences across our own lives and the lives of all others who have held and used the concept.
Definitions


On definitions:
What are definitions? The version that I like is that in practice, each concept is a bundle of properties. And so abstraction has a bunch of properties:
Conceptual rather than concrete
General rather than specific
Compressed representation
Abstraction as hierarchical compression (of lower level objects)
Representation that allows for predictive generalization out of range (both interpolation and extrapolation)
Details have been removed (salient features have been kept)
Shared structure between particular facts has been identified
Shared structure between particular facts has been labeled
(Is it an abstraction / is it abstraction if we don’t label it?)
Metaphor as implicit abstraction makes this distinction
And when a process has some of these properties we’ll call it abstracting. The hard question is which of these are necessary? Which of these are optional? Is the binary classifier for whether or not something is an abstraction whether it has a single one of these? May it need all of these? Certainly, this body of properties is a surface from which you can explore a space of definitions that are all likely useful in their own way and are close to what we mean when we say abstraction. Settling on one combination of properties with a set of rules like ‘these two are necessary, but if this third property is paired with this fifth property we can disregard the second property’ feels like a painful and terrible way to go about defining things.

What is the right way to think about things? I’d love to just introduce all of the properties and then leave the usage up to context. OR I could make a number of distinctions across the properties that tend to vary most often. And so we’d have a PCA-style set of principal component (variance maximizing) differences in usage. And each difference in usage would get a name that made the appropriate distinction (say, compressive abstraction, or labelless abstraction). And also make the distinctions between transfer and abstraction, between metaphor and abstraction.

Many properties of the defined object are actually consequences rather than causes of consequences. And then you can optimizer the object for those consequences (say, optimize the way in which you abstract for generalization ability). But it feels unusual to define the object in terms of its consequences.

Need a word for the way that there’s a bundling of related traits into a single concept.
Take ‘running’ as the general version of 1. Many animals running, say. It could be seen as using legs to move quickly. It becomes a metaphor quickly - “I’m running my mind over this paper”, or “my mind is running back and forth”.

Examples of abstraction that violate each property:

Conceptual rather than concrete
In object oriented programming, the creation of an abstract class is a solid example of an abstraction that’s just as concrete as its subcomponents.
General rather than specific (This one is hard, may want to stick with it)
Can argue that mechanics is more abstract than quantum (because it abstracts away the details), but it is actually less general than quantum.
Compressed representation
Non-compressive abstraction… This is really strong. Can’t find one after ~2m.
Representation that allows for predictive generalization out of range (both interpolation and extrapolation)
Going too high usually kills predictive power. Say you think in terms of blocs of countries (which leads to assuming that the countries with the blocs and their hierarchy of suborganizations all want the same thing) 
Details have been removed (salient features have been kept)
This is quite strong.
Multiplication is an example of the level of detail remaining the same. (acutally wait, multiplication eliminates the particular numbers involved… nvm.)
Shared structure between particular facts has been identified
You an abstract over a single datapoint, so no. But it’s likely that you won’t do it well.
Shared structure between particular facts has been labeled
Stores as abstraction over the production / supply chain violate this. But they do create an easier to use, higher level simpler interface to the backend.
(Is it an abstraction / is it abstraction if we don’t label it?)
Metaphor as implicit abstraction makes this distinction
Creation of a hierarchy
Counterexample - properties are abstractions across animals…
Only if animals are your datapoints. If the concept of ‘claws’ is your property (the animal has claws) then you see each instance of claw as your lower level.
This also feels strong. You can almost always create a hierarchy. 

Implicit to this question is that the definition should be that which is invariant across all examples of abstraction. But this is overly focused on consistency, and not enough focused on a principle component analysis of the properties that are most key to abstraction.  (On the battle between intuition and rigor in definitions).

If you care for rigor:
Details have been removed, keeping only the salient features
Do not pick conceptual rather than concrete (abstractions can be concrete too, say in programming)
If you care for intuition, ordered list:
General rather than specific
Shared structure (labeled)
Conceptual rather than concrete
Compressed Representation
Details have been removed
Representation that allows for predictive generalization

Justification for Ordered List

First, the things that were removed / didn’t make the list: metaphors as implicit abstraction is interesting (as a broader category of transfer exists, which perhaps should be the true title of this book, since we really care that we do transfer/induction successfully and not necessarily that we use abstraction to do it [whoa. I should think about that]).

General rather than specific is the most important defining quality, 


On General rather than specific

This depends on a reference point of generality. Which means that the process of abstraction moves from the more specific to the more general, rather than being objective. Or this is a distinction - you may say that a category like ‘dog’ is abstract, but compared to what? Compared to base reality. But it’s extremely grounded in comparison to animal, or being, or object (of which it’s a sub-class). And so there are two versions of abstraction at work here - the conceptual (relative to the concrete), and the relatively more general (or broader) class of objects. 

Types of shared structure (and so, types of abstraction)
Function
Leading to functional abstraction
Presence of a property / sub-object

Transfer
Abstraction is one way to map shared structure from one problem / solution / dataset to another. Transfer is what allows for efficient modeling and learning, where upon encountering a situation an intelligent being or system can bring patterns seen in data and problems from the past to bear on the new situation, and so be able to act as if it’s already seen the ‘new’ situation before, informed by situations like it. Abstraction involves identifying a property or pattern that exists (usually across many datasets / problems / examples) and then naming that pattern in a way that is general across the examples (and so which you would expect to generalize to similar examples)

There are forms of transfer that don’t move from the specific to the general, but instead relate the specific directly to the specific - one quality example of this is metaphor. Metaphor works by pointing out that one object is like another object, without necessarily spelling out exactly in which way it is similar (often, the metaphor will draw upon many intuitive and emotional properties, simultaneously). For example, take the metaphor ‘she has a heart of gold’. At one level it’s asking you to feel about her heart the way that you feel about gold. In abstract terms, you could say that the sense of awe you feel at the lustre and rarity and globally recognized value should also be felt about her heart. The way that metals can’t be changed, the strength implicit in it, the sense of being able to depend or it and (more importantly) the body of felt associations that any person moving through the world has associated with gold get transferred to this different object, the heart.

Abstraction does transfer through surprisingly similar mechanisms. Over time we build up associations between concepts and the properties and emotions that are experienced in tandem with those concepts. When we bring that concept (take an example from above: strength, or rarity, or metal) to bear in a situation, the properties associated with that concept are naturally brought to awareness when the concept is used.
The difference is that in abstraction, an explicit label is given to the set of shared properties. Take ‘strength’. What do strong things have in common? There’s an element of power, robustness, capability - there’s transfer between everything that has been described in the past and every other object with that description. And now we have an abstract object, strength, which holds that bundle of properties.
This natural build up of descriptive transfer allows us to use language to connect multitudes of experiences with one another without ever explicitly comparing them to each other. We merely have to experience the same abstract object in each context, and the transfer will follow naturally from using that abstract object to describe a new situation.

Transfer of solutions can be particularly powerful, if you realize that some abstract descriptions of problems share solutions than finding a way to represent your problem in the way that others are represented often gives you a surface for problem solving and decision making that didn’t exist before.

Transfer is at the core of induction itself. And even in deduction, the rules that it makes sense to trust are trusted for their ability to yield correct predictions in an inductive sense beforehand. Much of thinking is pattern matching between situations that you’ve seen in the past and the current situation, or is intuiting about a situation which calls upon implicit knowledge that you have also gained across time or that has been built into you through evolutionary transfer, where your instincts have been finely tuned for (say) social environments and so you can pick up on leagues of implicit knowledge emotionally based on a set of ancient and natural instinctual responses. Fight, flight or freeze responses are a pattern match to situations where that response saved the lives of the being making that response in the past, and so is present as a form of transfer from situations where stimuli were similar enough to current stimuli to trigger the same response.

Machine learning algorithms are all driven by transfer. The goal is to observe some set of datapoints, and on that basis find a set of patterns that will allow knowledge about new datapoints to be inferred. The process of transferring knowledge can be driven by different notions of similarity (which is the basis on which you expect the transfer to be successful or to fail). Often algorithms will weight the ability to do transfer on the basis of the degree of similarity to other datapoints, ex. kNN. That set of principles is general across all learning algorithms, and while transfer is often referred to as being between-dataset transfer in machine learning, each algorithms focus is this within-dataset transfer for generalization.

Compression
Compression lowers working memory requirements
Compression lets you store more

Lower working memory requirements for compressed objects means that more information can be fit into working memory. The reality is that most thinking requires that you put multiple objects into slots in working memory and then watch them interact with one another, using the recombination of those objects, their properties and relationships to generate insights or plans.
With a compressed object representation, something that may have taken up three, four, or more slots in working memory can pick up just one. (Functional abstraction is particularly useful in this context). That means that at high level of abstraction you can think through the interactions of tens or thousands of sub-objects and sub-sub objects while looking at only a few high level objects which you hold in working memory.

Compression also likely has deep impacts on long term memory. There’s a sense that total storage space is dramatically improved by not having to remember the details of situations, by representing the memory conceptually. There’s this sense that recall is generative and so in effect stored as a time series of neural activations. This further compresses the pure capacity necessary for memory.

When we use language we attach information about datapoints to those descriptive concepts and let the transfer occur through the connotations and lessons attached to those concepts.

Temporal Abstraction & Causality

One of the most fundamental types of abstraction is across time. We organize time into a natural hierarchy, from sets of seconds that make up each minute, to sets of minutes that make up each hour, to sets of hours that make up each day, and on up. Thinking in these terms is liberating. Imagine needing to make a plan, and having to do it at the insanely granular level of detail of seconds or minutes rather than weeks or months at a time. The ability to operate at a higher level is what makes makes planning feasible.
Thinking causally is one of the most powerful sources of our prediction capacity, and it’s enabled by this ability to abstract across time. One easy way to think about causal reasoning is to think about ‘what would have happened otherwise’, or counterfactuals. In order to simulate what would have happened with or without an event occuring, or whether a particular action was the difference between an important outcome happening or not happening, it’s necessary to both group time periods where the action could have happened together and to group time periods where the outcome is expected together. Otherwise, assigning causal impact to an event fails.

Temporal abstraction lets us compare the same action or event happening at slightly different points in time to other experiences where that action or event happened at slightly different points in time. It makes our thinking robust to small shifts in the patterns we see between actions and outcomes. 

Our mind is constantly making predictions (whether or not we recognize them as predictions) at multiple time scales. A prediction like whether or not a project will go as planned that plays itself out over the course of weeks is at an entirely different time scale than whether we’re going to get crushed or not by a heavy closing door (and in the case of a positive prediction, need to dart out of the way).
Abstraction is what makes feedback at a meaningful scale possible. It also allows us to make predictions arbitrarily far into the future, filtering out huge messes of detail that could feasibly crop up in the interim. 
Decomposition
Decomposition is inverse abstraction. You can do extremely direct transfer between them.

Linearity (sum of parts) as allowing for decomposition and recombination to allow for solutions in linear problem solving that are difficult in non-linear systems.

The types of decomposition correspond to types of abstraction - 
Functional Abstraction (We got here by other means)
Modular Abstraction
Property-based abstraction
Physical Abstraction (composition of parts)
Recursive Abstraction
Temporal Abstraction (We got here by other means)


What kind of x’s exist?
Ex, what kinds of deconstruction are there?
What properties does x have?
Elimination over the set of properties as fodder for new similar but different objects
Take love. Say there are 7 types of love, all of which share some properties and not others. The deconstruction creates nuances, but also creates a space of possibilities where each parameter in the space is turned off or on (if it’s a binary property), or can be in one of many states (if it’s discrete non-binary) or can vary along its continuum.
Modular Decomposition
How does x accomplish its purpose?
For each step in that causal graph, create a node
Functional Deconstruction
How does x accomplish its purpose?
For each step in that causal graph, create a node
Ask what the function of each node is (why it is there)
Generate new options that accomplish the same function
Physical Decomposition
Recursive Decomposition
Temporal Deconstruction
Often a process has a dependency set that implies a temporal ordering.
Recombining the orderings of a process can dramatically change it.
Parallelizable processes can be even more valuable to deconstruct, because they can be scaled arbitrarily.
Explicating an Example

Scientific disciplines are distinguished by the grade at which they interact with reality, from lower level to higher level, and by the relative ease of formalizing lower levels of abstraction.

Take biology (say, using the cell as an example of an object in biology) to be a particular composition of a body of chemical interactions. And notice that across almost every object in biology, sets of chemical interactions characterize the interactions and effects we seen in living creatures. In this sense, biology is more specific, and chemistry is a wider set of tools which can be combined to create objects in biology. 
In this context there’s functional hierarchical abstraction, in that sets of chemical reactions paired together can be represented of as a process that has some higher level function or purpose. The grouping of these interactions (by location in the living creature, or by time, or by similarity in the same kinds of bond between kinds of atom or molecule) drives a compressive process that lets us think about the abstract representation as a single entity.
The upside to this representation is that often processes will involve the entity as a whole (say, the cell dying) and without the abstract representation it would be a challenge to label all of the sub processes involved in cell-level phenomena like that without having an explicit way to refer to is.
There’s this question of how many layers of representation is optimal for thinking about problems in the space. For example, a canonical representation of the biological levels of organization is (from this simplest to the most complex) is organelle, cells, tissues, organs, organ systems, organisms, populations, communities, ecosystem, up through the biosphere. But between ex. tissues and organs there is a huge gap, for which having a representation may reveal sets of phenomena that would not have been properly conceived of otherwise.
Chemistry is in a similar position with respect to physics, where most chemical interactions are driven by forces (ex., the electromagnetic force between electrons and protons) identified in physics. 
Application: Learning
The implications of abstraction for learning are multitudinous. The obvious place to start is that every concept we use and tie together and show this that we create our intellectual surface or profile.

Creating New Abstractions
Examples:
Moving ideas out of and across domains
The making of consilience, the reification of the unity of knowledge
Invert creativity (non-novel value)
Making the discrete continuous
The mechanism that selects identities
Both identity in this moment and the identity(ies) worth moving towards
Meta-identity?
Re-name the curse of dimensionality
Invert Chaos
Statistical Mechanics? This is how I’ve been describing it, as stat-mech vs. chaos.
Need a temporal version of distributions
Gaussian / Poisson Process?
Need a verb for mutual information, for ‘has information about’
Can say x is correlated is y, but can’t say x is informationed with y’
This is a problem because you can say ‘anti-correlated’, but can’t say anti-has information about
Actually nvm, this is a tragedy where correlation can say that the relationship is positive or negative because linearity implies that the relationship always is positive or negative. You can’t do that with mutual information, it captures non-linear relationships.
For the way that the future is always in the present
Ex., how differently you treat someone you’ll be with forever
I consistently frame this in terms of the iterated vs. uniterated prisoner’s dilemma, but it needs a word
Words for the different forms of meaning
Meaning that comes from devotion / sacrifice to something higher than yourself
Meaning that comes from connection, community, relationship
The use of dramatic social upheaval for a fundamental values shift
He needs an <insert word>
He needs a social rite of passage
He needs a social cleansing
None of these are close..
Making the binary probabilistic
Map-territory conflation
Concept-instantiation conflation
There needs to be a word for the ‘bayesian problem’ where you just don’t take the prior into account when they’re doing causal inference.
Ex., canonical success traits that work but that are underrepresented in the base population

These are some fascinating objects, many of them conceptual, that are a set of example of creativity in finding patterns or shared structure between our own stories or experiences that can be named and in being name be efficiently referred to and more easily built on top of (due to the freeing up of working memory).

When a new concept is created and codified as a word (say, you give a name to the moving of an idea out and across domains), suddenly the ability to think with and communicate with that concept is dramatically enhanced. In our example of moving an idea out and across domains, we may recall several examples to mind. Take Antifragile, by Nasim Nicholas Taleb. It’s built out of the inversion of another concept (fragility) but does helpful work by allowing us to gather all of the examples of a particular property of systems under the same concept, and insodoing understand it more deeply and wield it more fluently.

Many problems can be discovered completely conceptually, and (often) would only have been discovered conceptually. People ignore selection effects all over the place. Importantly, they ignore base rates. In what I call a bayesian problem (where you fail to take the prior into account) there’s a body of counterintuitive truths about the functioning of our minds that can be discovered and used. Without the conceptual representation, selection effects would have driven data to be interestingly in violation of naive expectation. 

A concrete example is the effect of college on students. Demographics consistently show wonderful outcomes from students who went to ivy league schools. One reasonable counterhypothes to the value of the schols’ education system is that students are selected for quality in advance.


Conceptual Schemes

Abstraction is actually (partially) about founding the field of conceptual analysis

It's about making the conceptual scheme explicit, along with the questions, answers, representations and assumptions that come out of that scheme.

It's about how we fit all of our data into our existing conceptual scheme, and about how to minimize the bias induced by our scheme (and optimize the bias that does exist for predictive value or other kinds of value)

Example:
'Products' are an abstraction over unlike objects. The natural attempt at decomposition yields 'product categories', grating similar products and lumping them together. This aids transfer by letting you consider transfer within categories, which is between much more similar objects. Without a concept of product categories, many connections would not be made between products, because the general class of 'products' doesn't support those connections across all products. In many cases, we lack concepts like 'product category', and fail to make umpteen extraordinarily valuable connections because our conceptual scheme is insufficient.


Similarity / Distance

Similarity, Distance, and Memorization

This is so so long in the making.

Think about: Distance and intuitive physics

Continuum of similarity:
Discrete
Equality / Identicality
Property overlap
Edit Distance
Continuous
Euclidean Distance
Angles
Cosine Distance
KL Divergence

Think about a distance metric between shapes. Humans have an intuitive sense of the similarity between shapes, as a part of a general ability to judge the similarity of any two objects in an undefined intuitive space. But writing down that metric is incredibly difficult. And so much of the mission of representation learning research is learning how to compare arbitrary objects to one another through a distance metric that’s learned from experiencing arbitrary data. 

Similarity is at the core of all learning and cognition. Neuroscience side, an example is the heuristic that ‘neurons that fire together, wire together’, connecting sets of data that are similar in that they occur close by in the time series that a mind experiences. It also leverages another notion of similarity - if a and b there are previous patterns that are established, those previous patterns a’ associated with the firing of a will also be associated with b. This transitivity quickly becomes a wonderfully nuanced and complex form of similarity.

In developing knowledge, there’s a value to the knowledge that will generalize. Memorization is fine if you know that the data you see in future will be identical to the data that you’re seeing now. But there’s a continuum over the richness of similarity metrics, where memorization can be defined as the way similarity breaks down a short distance from the datapoints that have been memorized (or an inability to return an answer when you’re a short distance away). We get beyond memorization by finding ways to map similar datapoints to one another, and through that connection drawing conclusions about the properties that those similar datapoints will share (this depends on the ways in which the objects are similar) and is stronger than memorization in that when you encounter new information that hasn’t been seen before, you can compare it to that which you’ve already seen and use that history to inform your understanding of this new experience.

Often memorization looks like a lookup, which is fragile. If you don’t find something that’s exactly equal to what you’ve seen in the past, you can’t return anything. The more effectively you can connect a new experience to a vast array of old experiences, the more data you’ll have to draw on when you make inferences about it.

One implication is that broadening the types of connection that you make between objects allows you to transfer more information and connect more types of object. Seeing more of an objects properties creates a larger surface for comparison, enriching the kinds of connection you can make between your object and others.

As you move to a more expressive and nuanced similarity metric (ex. from binaries to a continuum, say from whether a person is good or not to how good a person is) the distortions that come from conflating datapoints that are relatively close but not identical with each other can disappear. But the tradeoff to eliminating that conflation is needing to store a much more complex representation of goodness for every person (and likely move from an intentional, deliberate process for thinking about it to an intuitive one).

Properties of data that make certain kinds of similarity metric more relevant:

Imagine trying to use edit distance for semantics, where you tried to map words’ conceptual similarity to the number of changes you’d need to make to the letters in one word to get to another word. The lack of overlap between a word’s spelling and its meaning makes this notion of similarity irrelevant. 
But instead, imaging looking at the similarity of the contexts in which words appear. Specifically, say, the number of occurrences of a small 2-5 word window of surrounding words. Suddenly, words with similar contexts and meanings can be mapped to each other - ex. Cat and dog are often used with similar surrounding words, and so will be close to one another. King and queen are also used with similar surrounding words. And when they differ, they tend to differ in a way that has to do with the meaning of the words. So distance on this similarity metric is meaningful in ways that aren’t captured by edit distance. The design of distance metrics that capture the structure that matters for a task is extremely important. 

Implication:
Languages need to merge semantics with 
A language that merged its word / letter representation with the actual meaning of the words (where, say, base sounds / letters represented the principal components of learned word vectors) wouldn’t require memorization to learn because the mapping from concepts to reality would be on a continuum and its meaning grounded in the language itself rather than being an arbitrary mapping from a word to a concept.

Generator:
Why does language learning require so much memorization? In general, needing to memorize indicates that you’re using a degenerate distance metric and that your learning will fail to generalize. 


Similarity 1.0

What is this ‘shared structure’?

Underlying the concept of ‘shared’ is a notion of similarity.

Closeness to equality.

Question:
Are all forms of similarity captured by 'how much you have to change the object to get equivalence?, and where equivalence is "these objects are the same"?"


Topics:
Relationship of abstraction to similarity	
One type of abstraction identifies shared structure across objects and compresses it into a single concept or abstract object.


Similarity as existing over different features
Type of similarity as a function of the nature of the thing being compared
Types of similarity measures
Discrete:
Equivalence
Edit Distance
Number of properties in common
(Having a property in common is similarity over that property)
Continuous:
Cosine Distance
Euclidean Distance
KL Divergence / Cross Entropy
Wasserstein Distance
Hinge Loss
Generating Similarity Metrics
Concept Representations
Word Embeddings, same up to angle
Networks
PCA over learned representation
Types of Similarity
Have the same function / accomplish the same task, consequently
Laptop is actually a functional abstraction, more than a compressive technique over sub-parts.
But it also cares about the sub-parts… the surface and ipad are functionally similar but are called ‘tablets’ instead of ‘laptops’.
Use the same mechanism
Have the same property
Ex. shape, color, density
Have a set of shared properties
Question: Are all forms of similarity captured by 'how much you have to change the object to get equivalence?, and where equivalence is "these objects are the same"?"
Cognitive Fit, human notions of concept similarity

Relationship of Abstraction to Similarity
Similarity is a foundational concept that forms the basis of the ability to compress information across objects. When objects are similar, whether it be in their properties, or their constituent parts, or in their function, it becomes possible to transfer information from one object to another via awareness of this shared structure. 
In the extreme case where objects are identical or equal, we can compressive massively - we can throw out one of the objects, and merely remember that it’s equal to the other object. On the continuum away from equal, we lose compressive power in that we have to trade the compactness of our representation of the object against the amount of new information that the object holds.
As an example, it’s often much easier to store a deviation from an existing object that to construct an entirely new object. Say, this is like headphones without the wires (for bluetooth headphones), rather than inventing a new name entirely. This is a phone, but smart. That modification of an existing representation is transferable across people who have the existing representation, and is compact in the amount of new information that exists (only the deviation). In the same way that human attention is drawn merely to what changes in the environment (and in general things that are unchanging fade out of awareness), representing new information as a deviation from an old representation is a classic example of efficiently taking advantage of similarity.

Similarity Over Different Features
Similarity can operate over all the features of an object. It’s often the case that features are intercorrelated, and so when enough features intercorrelate we tend to create a term or concept for that body of relationships. When objects are similar over one feature but not in others, there’s often conflation or confusion when an attempt to generalize from the workings of one object to another fails.

We can think of similarity over different features as often having very different properties - being measured in different ways, allowing or disallowing transfer in different ways, etc.


Measuring Similarity
There are a body of metrics for measuring similarity - the classic example is equality. When two systems are equal, they reflect one another perfectly. There’s no information in one system that isn’t reflected in the other system. And so we can do heavy compression. But equality is binary - the objects are either equal or not. And so it’s not granular enough to capture shared structure that is incomplete. Equality strongly limits the complexity of the objects that can be compared to one another, and so looser metrics are critical to modeling real systems.



Difficulty in describing continuous similarity, distributional similarity. Similar difficulty in describing distinctions, or breakages of similarity in distributions. General difficulty of reasoning outside of discrete space. Need for cognitive fit.




Types of Similarity
Difference from Equivalence (Shared structure over metrics)
Cognitive Fit (Similarity in human intuition)


Temporal invariance is so critical to abstraction
"I" am that which is invariant across time
Because HOW ELSE WOULD YOU ACCOMPLISH THE TRANSFER???

Who are you?

I am he who selects value systems.
But as soon as you can see that, you become he who selects he who selects value systems.
And so who you are is the level at which your self awareness of the emotions that are driving your decisions bottoms out due to the constraints of your working memory, attention and knowledge.

Generalize
Generalize to all labels
Labels have power insofar as they can be applied consistently across time
Generalization requires similarity in the training and test distributions


"I" being that which is invariant across time is strong, because you expect transfer into the future. That which has varied in the past can vary in future. And so true destruction of self looks like varying every aspect of your identity, substantially, repeatedly. Until not even the fact or degree to which you vary your identity is consistent across time.
This is a nod to that which stands the test of time, and to the lindy effect.

'Invariance' is just a particular nod to similarity. 'Non-changing' implies similarity across that which is invariant. And so it's just one of umpteen kinds of similarity. And similarity is the grounding for transfer.

In many ways, though, invariance is stronger than similarity when you’re looking for a sense of certainty that the transfer you intent to pull off will actually hold. There’s this ease of transfer when the match is exact - when the match is inexact, suddenly the properties or effects that do or don’t successfully transfer are called into question. In the abstract (I can find a few examples later), there’s a body of motions involved in transfer (which should be enumerated) which include properties being shared, solutions being shared, levels of representation being shared, and relationships between objects being shared. All of these depend on the similarity between the two high level objects that contain these properties, problem and solution representations, objects and relationships in them. And so when you get invariance (which is closer to being identical than mere similarity), many of these properties transfer more cleanly than if there’s a loose analogy or a continuous (rather than a discrete) notion of similarity binding the objects together.

First, this calls for a break down of similarity. Discrete and continuous modes, and an analysis of the loseness or tightness of metaphors or connections between systems. There’s a body of conditionals, where the interactions between the type and the degree of similairty and the kinds of transfer that are acceptable or not acceptable have pattens that let you know whether or not the inference you’re attempting is legitimate. 

Second, this asks for a kind of breakdown of transfer - what kinds of transfer are possible, between what kind of objects, what kinds are common, what are the properties and failure modes of those popular kinds of transfer. Examples that have been explicated that spring to mind include  reference class forecasting and k-nearest-neighbors, both of which can be analyzed statistically and intuitively. In both cases there’s some notion of a set of features or properties of each datapoint that has a notion of similarity attached to each feature / property, which in aggregate (usually through a weighted aggregation) can be compared to other datapoints and used for inference insofar as their similarity score to another datapoint is high.

It’s likely that particular kinds of similarity (say, over one property but not others) leads to the ability to do particular kinds of transfer. We learn these relationships by spending time in the domains in question, and likely also learn it in the abstract (though I haven’t looked at examples closely enough to say just yet).

Spatial and temporal invariance are grounded in physics. There’s a question of whether temporal invariance is special, whether spatial invariance is special. Temporal structure has a lot to say about this kind of invariance.

In what way shoudl your transfer decay as your similarity score drops? Should you do transfer in the same way, but merely drop your confidence in the results? Obviously you have to see the featurs across which the distributional shift occured, and ask how those features causally interact with the outcomes that you’re attempting to predict. 

Temporal invariance has to be measured across multiple timescales. What is invariant at a large timescale (say, years) may not be invariant over the weeks timescale or the days timescale. And it’s the choice of the scale at which to analyze relationships that lets us do long term planning or abstract over the experience of entire civilizations. 

Dynamical systems where interactions across time blow up the complexity of the model needed to capture the sense that interactions can be measured at any of many possible timesteps call for temporal abstraction to fit reasonable hypotheses to the dynamics of the system. And so learning how to judge which time scale at which to do the analysis is extremely important, and something we do intuitively.

Calming down, there’s a want to cover all invariances. Temporal and spatial invariances ground our thinking in intuitive physics. Which is strong and helpful, but not nearly as strong and helpful as being able to capture invariances in informational space generally, and not just physical space. There’s this sense that there are invariances across concepts, or across systems, or that are necessary for consistency that can be leveraged to make intellectual progress. And the focus on neuroinspiration comes with a focus on physics inspired invariances. But the principle is scarily general.

Value of Representations
Everything has a representation. Raw sensory content is represented to sensors as a stream of sets of pixels [should include whatever the brain uses], or frequencies of vibration. (Taste? Touch? Smell?) [Describe the way the brain re-represents reality so that creatures like us can interact with it]
Re-representing information is powerful. Ex., re-representing information so that it can be transferred from one situation to another. Representing the internet as a graph (with links as edges between web pages that are graphs) rather than as an amorphous concept or as TCP-IP allowed the use of Page-Rank (a graph algorithm) to turn into Google. Other representations of the internet don’t lead to the same solutions for searching the internet.
The concepts you use to describe a situation carry implicit assumptions (a frame) that can be considered your default representation. For example, when you represent numbers as arabic numerals (2, 3, 5) multiplication becomes easy (for a few reasons, ex. The number of digits of the two numbers being multiplied correspond to the number of digits in the resulting number, or ex. You can use the distributive property to break a multiplication down into a value that’s 10*x + y, say distributing multiplying by 32 into multiply by 3 and adding a 0 and multiplying by 2.)
When you use roman numerals, things become much much more difficult. This re-representation of our numbers turned a problem that used to require expert level mathematicians into something that most 10 year olds know how to do reliably.

One easy way to see the way that a change in representation can be valuable is to see where a discrete representation of some information would be better off continuous and when a continuous representation would be better off discrete. Imagine if, instead of measuring, say, speed of a car on a continuum it was measured as a binary (fast or not fast) which would be triggered at some MPH rating. Immediately many more people would die due to accidents in speeding which come from an inability to make distinctions between levels of speed limit. And when it comes time to debate the speed limit, instead of seeing the hidden assumption (a binary speed representation) often the debate will center around what the number that determines the speed transitions from not fast to fast.

Think about the re-frame from binary belief (where statements are true or not true) to probabilistic belief (where statements have higher or lower probability as a function your knowledge that’s relevant to the belief). This reframe dramatically improves thinking on many philosophical issues (is it just or not just to ‘to what degree does it serve justice) and practical issues (ex. the probability of a cyber attack is low, rather than thinking that an attack will or will not exist).

Compositionality

Abstraction is how you construct a compositional conceptual hierarchy, and so benefits from compositionality are akin to benefits from quality abstraction.

The answer generally given is informational efficiency. Recombination of abstract concepts allows you to hit so many more possible meanings than having a particular concept for each importantly different object.

The conceptual building blocks automatically allow for changes at lower levels to impact many higher level recombinations of concepts.

Compositionality makes rapid learning possible through flexible generalization, without a need to see data for every recombination of parameters in an environment.

There’s a generality to decomposition + recombination for problem solving.

Creativity through recombination of existing concepts.

Compositionality is at the core of productivity in building objects, building software, building ideas, almost all creation.

Easier generalization, as there’s much more data informing a sub-concept in a conceptual hierarchy since you can draw from every instance where the sub part exists (abstraction extends dataset size)

Existing models of new data that can be decomposed into existing parts.

Decomposed problem / goal representations


Combinatorial Representational Capacity
Broadens space of possible meanings through finite concepts
Elegant Updates
Updates to a sub-concept flexibly updates all recombinations with that concept, capturing shared structure between more specific concepts that include the sub-concept
Speeds learning through efficient generalization
Creativity - creative solutions often take the form of recombinations of existing concepts
Decomposition + recombination for problem solving
Abstraction allows for learning about sub-concepts, broadening dataset to all instances of the sub-concept
Stronger Generalization - existing models of new data that can be decomposed into existing parts.


Examples:
Building Objects
Car / Bike / Train = composing wheels + frame + engine / power
Building Software
Statements, variables, conditionals compose to create functions / classes compose to flexibly and consistently solve software preoblems
Building ideas
All of language as concept recombination, each sentence merging composable meanings.

The project of efficiently representing unbelievable amounts of knowledge generally relies on finding a body of recombinable patterns which can flexibly represent an extremely wide array of objects. Atoms up through objects work this way. Human and programming languages work this way. This is the most likely generative model for our universe.
Generalization
What is generalization?

The critical property of an abstraction is its ability to generalize. 

Within a domain, learning often looks like generalization - in sports, you pattern match one situation to similar past situations, and react instinctively in a way that your intuition hopes will lead to success. In mathematics, solving a problem with an algebraic manipulation once lets you recognize that type of manipulation in other situations. And often so you abstract the manipulation into a rule or into an operation that you can run more flexibly.

But you’d also like to do out of domain generalization - learn something in one context and apply it to an entirely different context. Learning language in one domain (say, in a home) and then applying it at school, or with friends rather than parents, or in speeches. Take the concept of specialization and lift it from economics to understanding sexual dimorphism in evolution. Taking the concepts of a replicator and differential selection from evolution and apply it to ideas and tunes and fashions that replicate by imitation. (add something about decomposition, modularity, causality)

Generalization as a Standard

Generalization accuracy is a great standard to hold abstractions to. What we want is for our representations to aid us in problem solving, which often takes the form of prediction what the impact of our actions will be or predicting what the state of our system will be in future.

When adjudicating between representations and when constructing them, we’ll optimize for the representation that is easy to evaluate (simplicity heuristic) and that makes the most accurate predictions. And simplicity is also a part of accuracy - models that are simpler have the advantages of capturing more data (because in general they’re more abstract), being more robust to small differences between observations and so better able to capture the higher level regularity, and being straightforward to update when they’re mistaken.

Tradeoffs need to be adjudicated, and so having a downstream task to determine the appropriate lines for those tradeoffs is invaluable. Yet in practice people use other standards either as proxies for generalization or to preserve longer term value - truth is a classic example. Instead of asking if a representation is predictive, you can ask how closely it corresponds to reality via some similarity metric between your map of the territory and the territory. Often there are tradeoffs between the true model and the model that leads to the best generalization accuray. 

Even generalization accuracy should be seen as an intermediate standard or proxy, with utility as the true goal. And perhaps we should resolve the tension between predictive accuracy and utility in favor of utility. Many models or pieces of information that improve predictive accuracy do dramatic damage to agent utility (ex., noble lies - rights, objective grounding to values, sacred & religious beliefs, etc.). It’s not clear that the metric we want to evaluate these pieces of information over with is predictive accuracy, and so that evaluation needs to happen in a decision function that adjudicates between standards based on their contribution to utility.

Alignment of Representation over Shared Structure

What this means is that you’d like to guarantee that making a single update will apply over the entire affected part of the representation.

For example, if you’re using the connotations of words to do the transfer concepts need to be valuable as language, it’s possible to run into russell conjugates (where two different words mean the same thing). In that case, updating one may not update the other - an ideal representation would realize that those words have similar contexts and make an update to one consistently lead to an update in all of its russell conjugates.

Often it’s efficient to update representations compositionally, where an update to a part of the representation that’s used in many downstream components can effortlessly feed into those components.

This has implications for concept creation and usage. When you introduce or create a new concept, you split the data between it and the substitute set of concepts you’ve likely been using to communicate the same idea.
Abstraction in Reality

Example fodder:
Grocery stores as an abstraction over supply chain / production of foods
Machines as abstractions over the few parameters that need to be manually controlled in a process
Computer APIs are literally referred to as abstraction layers

Almost every interface is a wonderful example of abstracting away the details of the inter

Many profitable opportunities (as well as ways to make people’s lives easier) involves abstracting away the painful details of a process that people need to go through. 
Food is one easy example. Instead of having people interact with the details of a complex supply chain and act as farming experts, grocery stores let people interact with a high level interface (a shelf in a store) which hides all of the details of the work required to produce and transport the product and reduces decision making to a comparison of prices. 
This bears similarities to abstraction layers in computer science. These eliminate needing to deal with the details of (say) the implementation of a particular sorting algorithm by having a generic sort function that’s backed by code that can change without changing the way that the user calls that code. This allows for improvement and change over time without a need for the high level behavior to change (and so improvements can be seamlessly integrated), but also exposes just the few parts of the system that really matter for it to operate properly (like which foods to pick in the grocery store example) and allows the other details to be abstracted away.
Leaky abstractions in computer APIs (where you actually need to understand the underlying code implementation in order to use the interface or abstract representation properly) also show up in reality, where a store that’s serving as an interface to an implementation may not expose whether some food was factory farmed or not, or was exposed to pesticides or carcinogens or not, or was genetically modified or not. In the absence of this information, customers (or the FDA) would propose or demand that that information about the details of the production process be made available to the users of the interface. In some cases (whether a food was prepared next to peanuts that could trigger an allergy, for example) there’s a clear need for somebody to have knowledge of the details of the production process in order to make reasonable decisions.

Examples
It’s extremely important to have a set of examples to reason from. 
I’m going to list a number (perhaps 3+) of examples for each component of abstraction that exists. I currently have two decompositions of the concept of abstraction: One over the domains that abstraction works in and one over the contrast between idealized abstraction and abstraction in reality. I want clean examples for all.

Computer Science
Object Oriented - Classes as a collection of properties.
The class dog contains properties that all dogs have (snout size, color, breed), and the classes for cat and for cow contain cat and cow specific information. Objects (particular instances of animal) instantiate the class.
The class Orange, or Apple, or Banana. They’ll have the type of apple, the number of spots, the density of the orange peel, etc.
Some graphic objects will have curves with eccentricity (oval), or an aspect ratio (rectangle), and those properties can be contained in their classes.
APIs - an abstraction over implementations.
Abstract Classes - A collection of properties of classes.
Animals Abstract class, where each animal eats food, sleeps, makes noise, etc. Then Dog extends animal, cow extends animal, etc.
Fruits abstract class, where each fruit has some weight, some time to ripeness, some water content, some color. Then apple extends fruit, orange extends fruit, banana extends fruit
Graphic Object, where each graphical object has properties in common like position, orientation, line color, fill color. Rectangle extends graphic object, line extends graphic object, circle extends graphic object.
Functions within Functions
Recursion
Mathematics
Algebra, as opposed to manipulating scalars (particular scalars) directly
Abstract algebra and its complexities 
Functions as the abstraction of an operation
Rules / Operations (operations as a codification of more specific manipulations)
Addition
Multiplication
Exponentiation
Category Theory
Cartesian plane / geometry, as an abstraction over numbers and geometric objects.
Bayes rule as built on top of conditional probability. Conditional probability built on top of set theory (the condition is a subset of the space) and general probability.
Logic
Abstraction over thoughts / beliefs / hypotheses
Ex., If A is true then B is true => B is false, therefor A is false
Ex., If A is true, then B is true => B is true, therefor, A becomes more plausible
Probability Theory
As an abstraction over relationships between arbitrary variables
Physics
Mechanics vs. Quantum
The level of specificity/precision at which measurements of systems are/can be made
Height as the appropriate level for measuring the meaningful content that humans care to model [Hikari on height], as opposed to the thing that we care about when we’re measuring height (say it’s predictive of age, and better would be the lower level chemistry of the organism that led it to grow to the height it is at)
Choice of certain features as being more “fundamental” than other features, and some features as being manifestations of many interactions between other, lower-level features
Language
The concept of abstraction
Society
Harvard students vs. student organization / student concentrations vs. individual students
Countries vs. organizations within countries / states within the country vs. people running organizations / collective population
Pattern Recognition / Signal Processing
Humans perceive color as discrete, whereas computers measure pixel values that are often still discrete but at a much finer grain, and in reality there are photons bouncing off of objects that absorb particular frequencies of light.
Images with hierarchical structure, where edges and curves become shapes and shapes become objects
Sounds to phonemes, phonemes to words
Intuition
Generalizing across dangerous animals by picking out elements like strength, sharp teeth, claws
Generalizing across human emotion - anger looks different across different people, but shares enough characteristics that we label it in the abstract.
Biology / Chemistry (This may simply be hierarchical structure… need to think about whether an abstraction is necessarily ‘virtual’)
Atom, molecule, cell, tissue, organ, organism, population, ecosystem
Atoms to molecules, ‘stability’ as important at the more abstract level, to maintain atoms in a particular structure.
The same foundational building blocks (atoms, molecules, cells containing genes) generalize up to diversity in animals, plants, bacteria, viruses.
Species - Genus - Family - Order - Class - Phylum - Kingdom - Domain
Species - genus (unified by common ancestry)
Individuals to species (unified by ability to interbreed)
Turning continuum into a class
Color
Red, Orange, etc.
People speaking other languages that cut up color space differently remember colors differently than english speakers
Length
Weight
Money
As an abstraction over value of labor / combined resource costs (I guess this is hierarchical compression)
Machine learning is a *wonderful* example of abstraction, where all problems of prediction an output from an input can cleanly fall into an X, Y pair that is fed into an arbitrary algorithm.
It’s pretty close to ‘function’ as a great abstraction, it’s a subset of that. It’s the subset where the utility of the function is making a prediction, or something nearby that.
This example of abstraction is about shared structure between the problems as well as functional unity.
Are there other implicit meanings in the word abstraction than shared structure and functional unity? Result of a compositional process?
Graph
Relational Structure
Object Oriented Structure
Object (Entity)
X is a Y relationships (Classification, Inheritance)
X has a Y relationships (Composition / Aggregation)
Properties of an Object
Causal Graph - X leads to Y
Dependency - X depends on Y
Subject - Object relationships (in sentences)
Linking verbs - ‘is’, ‘has’, ‘are’, ‘being’, ‘sense’ etc. between Object and Subject
Co-occurrence
Ex. Words mentioned in concert with one another
Link - are connected
Linkage Distribution
Locality
Edge Density
Examples of Relational Structure
Categories
Connections
Similarities between relational and hierarchical structure
Number of connected components
Topology & Graphs (manifold structure)
Abstraction gone wrong
Weapons of mass destruction is a beautiful example of abstraction gone wrong.
Conflation 
(See page 1 of Deadly Arsenals)
Illegal Drugs



Structure as Abstraction over Relationships

Structural Thinking

The key to low bias models is alignment between the the model’s structure and relationships in the data - not merely the representational capacity of the model. And so rather than thinking of measures of capacity or representational breadth as sources of low bias, we should recognize that these only create bias when they misalign with the structure present in the data. And so bias is not a property of a particular model or algorithm, but comes out of an interaction between a particular model and the dataset it’s trained on. That said, increasing the representational capacity of a model will expand the space of functions that it’s capable of finding through optimization, and so will be one proxy for how close the function that that model can learn is to the real relationships that exist in the data.

In the contexts where bottom-up hierarchical (compositional) models are applied to data that has bottom-up hierarchical structure (audio, vision) we see strong generalization. This alignment makes generalization easier for the same reason it’s straightforward to get strong generalization with linear regression over linear relationships. Whether interpolating or extrapolating, if the genuine relationship was captured it will continue to hold outside the training data range. If the structure in the training data isn’t capture by the model, we require strong amounts of regularization (in the case of networks, lots of dropout and weight decay) to learn a relationships that will generalize to the validation set. (cite the comparison)


Implications for Research

Intuition for Model Creation
Transfer Learning
Multi-Task / Multi-Dataset learning
AutoML




Intuition for Model Creation
In choosing which models to build, a common approach is to take structure that is present in important datasets but cannot be learned, and generate models that incorporate that kind of structure. A classic example is in learning long term dependencies in RNNs, motivating gating mechanisms and cell state for maintaining information across time. 
This source of inspiration differs from, say, neural inspiration.

Transfer Learning
One way to dichotomize transfer across domains is separating feature-wise transfer (transferring information about relationships between specific features) from structure-wise transfer. Structure-wise transfer involves abstracting up from particular relationships to looking at the types of relationship that exist between sets of features. (Write more about structural transfer, add example (probably word embeddings))

Multi-Task / Multi-Dataset Learning
Learning structure from data rather than encoding it manually will require multiple examples of the type of relationship being learned. This can be exhibited through multiple examples of that kind of relationships between features in a single dataset, but often the structure we care about only exists once inside of a dataset, and so we would need to learn over multiple datasets to learn the structure that transfers across datasets. In general this information exists in the mind of the researcher (who finds datasets that serve as examples of the needing the kind of concept or structure that they’re looking to learn), and so automating this search will require improved dataset representation.

AutoML
Automating machine learning research could dramatically speed up innovation. Approaches to metalearning have been taken through 1, 2 and 3. But learning the model’s structure has much more potential for aligning the model’s structure with the data than tuning hyperparameters of existing structures.
Deciding what algorithm to run on a dataset 

Categories of Structure That Exist, Examples in Data, Mapping to Algorithms



Fact List

Why this matters
Key to a new & powerful category of transfer
Key to strong generalization
Key to low bias models
Excellent intuition for model creation
Critical for metalearning new algorithms
Patterns / Regularities exist at multiple levels of abstraction. Modern machine learning algorithms capture regularities within datasets, but not regularities across datasets.
Transfer at the ‘shared’ feature level, as in CNNs, is powerful if the data is homogenous. But that is a strong limit to the generality of the transfer.
Strong generalization requires a model that captures the actual relationships between features, as opposed to approximating those relationships with a flexible model.
Low bias models come out of alignment between the structure of the model and the structure in the data, rather than simply coming out of more flexibility.
Model creation succeeds when an inductive bias that dramatically cuts down search space is shared by the data. It’s necessary to make true ‘assumptions’ in order to learn at all. But these assumptions don’t need to be made blindly - understanding structure is the way to consistently make correct assumptions.
Common types of structure [Define all, give examples]
Hierarchical / Compositional / Combinatorial Structure
Relational / Graphical Structure
Recursive Structure
Temporal / Sequential Structure
Clustering Structure
Discreteness - quantized, distributions
Continuity - distribution
Smoothness
Sparsity
Locality
Linearity / Polynomial / Exponential Structure
Principles of Structure: (Operate on your operators) [Define all, give examples]
Simplicity vs. complexity
Bias - Variance Decomposition
Abstraction - level of abstraction at which more or less structure, or different types of structure are present
Framed as Compression
Degree of Compression
Directionality
Discrete vs. Continuous
Abstraction - fine vs. coarse grain structure
Similarity, say, with a feature or set of features
Randomness, degree to which there is structure, compressibility of data
Homogeneity - degree to which the same operations can be run over objects in the structure
Dimensionality - Interactions between features vs. single feature structure
Across all types of structure:
Description and examples of structure
Interaction with principles of structure
Properties belonging to that structure
Transfer between differing forms of information that share that structure
Different types of that structure
Properties and Examples of each category of structure
Hierarchical Structure
Bottom Up
Compositional
Width-wise compositional
Depth-wise compositional
Combinatorial
Counters curse of dimensionality with representative capacity
Discrete
Offers multiple levels of abstraction for interaction and prediction
Types of information with Hierarchical Structure
Abstraction
Images
Objects - Object Parts - Shapes - Lines / Curves
Audio
Words - Phonemes
Businesses / Governments
Sciences
Physics
Chemistry
Biology
Ontology of Species
Organ Systems - Organs - Tissues - Cells - Nuclei + Organelles
Brain
Natural Language
Fields - Concepts - Words (Combinatorial as well)
Paragraph - Sentence - Phrase - Word - Character
Time
Centuries - Decades - Years - Months - Weeks - Days - Hours - Minutes - Seconds
Measurement
Kilometers - Meters - Centimeters - Millimeters
Object Oriented Systems
Classes - Objects
Economy
GDP - consumer spending + investment + Government Spending + Exports - Imports
Top Down
Recursion
Homogeneous
Discrete
Generative
Deconstruction
Offers multiple levels of abstraction for interaction and prediction
Relational Structure
Object Oriented Structure
Object (Entity)
X is a Y relationships (Classification, Inheritance)
X has a Y relationships (Composition / Aggregation)
Properties of an Object
Causal Graph - X leads to Y
Dependency - X depends on Y
Subject - Object relationships (in sentences)
Linking verbs - ‘is’, ‘has’, ‘are’, ‘being’, ‘sense’ etc. between Object and Subject
Co-occurrence
Ex. Words mentioned in concert with one another
Link - are connected
Linkage Distribution
Locality
Edge Density
Examples of Relational Structure
Categories
Connections
Similarities between relational and hierarchical structure
Number of connected components
Topology & Graphs (manifold structure)
Temporal / Sequential Structure
Periodicity
Hierarchical Periodicity
Seasonality
Burstiness
Messages
Words in documents
Stationary vs. Non-Stationary Distributions
Permanence / Option Structure
Quantized
Ex. hitting lights when predicting arrival time
Autoregression / Autocovariance
Feedback
Positive Feedback
Negative Feedback
Length of feedback loops
Synchronicity vs. Asynchronicity
Discrete vs. Continuous
Exponential Decay vs. Windowing
Continuity vs. Discreteness
Stability & Equilibrium
Derivatives - change over time
Asymmetry between past and future
Exclusive ability to directly impact present
Strong predictor of causality / anti-causality
Examples - All Data is Time Series Data
Clustering Structure
Distance & Similarity
Interaction with hierarchical structure



Clean vs. Dirty
Explanation of the Reversal

When doing transfer between the notion of abstraction between ‘reductionary’ and ‘pure’ domains like math / computer science, and ‘compositional’ and ‘dirty’ domains like concepts or deep learning, it’s important to realize that there’s a reversal in the direction that’s referred to as ‘higher level’ abstraction.

If you were implementing a DL hierarchy in CS, the most abstract layer would be the first layer, with its edges and curves (say in computer vision). That’s the layer that’s most general across all objects. It just gets more specific as the recombination occurs, in the way that less abstract classes get more specific.

If you fail to realize that this reversal exists, expectations around what can and can’t be transferred can become confused. In DL, the lower levels of the network are more likely to transfer. In CS, the more abstract classes are more likely to transfer between lower level datapoints. (though transfer has a different meaning in this context, as seen below - it’s a very restrictive ‘has these variables / properties / functions’)

In Transfer and Generalization

Take OOP. Abstract classes generalize to new classes, classes generalize to new objects. The assumption is identity, there are no moving parts. When the instances (objects) vary, that variation isn’t captured at all by the abstraction.
Take DL representations. Abstractions are constructed to generalize to datapoints that vary slightly from each other. Variation in the inputs are expected to properly processed by the model.

Heights of Abstraction as operating over more information

Strong distinction here! There’s inversion where in CS, the structure that’s shared across all instances is the highest level of abstraction. But in a conceptual hierarchy, height means a recombination of lower, more general building blocks.This is a dangerous fact that will lead to much confusion in transfer.I believe that James Koppel pointed this out to me a few months ago.

The ‘type’ of abstraction done tends to differ between discrete and continuous hierarchies
Continuous hierarchies are compositional, and consistently use the same type of abstraction all the way up / down the hierarchy
Discrete hierarchies can see abstractions made over different categories or types.
Dirtiness
Notions of similarity can be much stricter over discrete abstractions.
Equivalence
Edit Distance
Number of properties in common
(Having a property in common is similarity over that property)
Continuous notions of similarity
Cosine Distance
Euclidean Distance
KL Divergence / Cross Entropy
Wasserstein Distance
Hinge Loss
Mahalanobis (Distributional Distance)

Groundedness is much stronger in executable domains like CS where every abstract objects gets compiled down to bytecodes that run. There’s reality everywhere. In conceptual space, high level structure can seem to appear when it does not, or when the reverse is true. There’s dirtiness that makes powerful mistake possible, and memes take advantage of that ungroundedness to evolve in ways that allow them to propagate more easily. 

What does the bias-variance tradeoff mean in CS abstraction? Mathematical Abstraction? There’s no attempt at generalization, so it seems like there’s no generalization error to learn from. It’s a different process, computationally.


The thing with perfect abstractions is that often there’s no possible change in generalization. That’s how it works with math or CS - it’s like all that exists is the training data, which is discrete and low dimensional. The value to compression in the abstraction is just taking up less space, it’s not generalization capacity.



Valuable Properties of Representations

Valuable properties of representations, born out of the frustration with the obsession over disentangling representations to the exclusion of other critical concepts. Many of these properties exist, to a greater or lesser extent, in human cognition.

Decomposition of representation
This gives you a controllable, interpretable, recombinable representation
Alignment of representation where shared structure exists
Want concepts with the same mechanisms / structure to update simultaneously when there’s new information that informs their working
Can be through compositionality
Trades off against decomposition?
Modifiability of complexity of the representation depending on task
Representation that becomes more granular upon zooming in
Necessary for computational efficiency
Memory Constraints
Compute Time
Attention Constraints
Ideally would be on a continuum
Give me the n principal components (non-linear) of the representation, while preserving clean conceptual (semantic) decomposition 
Transferability
Ability for the representation to be repurposed for different tasks, generally through learning sufficiently high level structure that there is an appropriate level at which to do transfer between representations of problems and solutions
Appropriate tradeoff of Simplicity / Compressedness vs. Representational capacity
Sparsity
Necessary for the discovery of compute intensive structure (say, graphical / relational / network, or concept recombination) in the representation
Interpretability
Optimizability of representation for interpretability.
Quality translation from representation to natural language.
Clean isolation of parts of the representation (or a sparse approximation of the used representation) for any prediction made or action taken.
Control
Control through modification, freezing, or freeing of sub-parts of the representation
Discrete and Continuous Modes
Discreteness
For Interpretability, self-examination, sparsity.
Continuity
For representational capacity, predictive accuracy.
Fully general translation into and out of the representation
Want to be able to flexibly represent any category of object, situation, etc. in a merged representation
Reserve category errors for a particular mode of action, ‘rigor mode’

Abstraction as Religion

“More beautiful than the vision from any mountain top… is the view of the world from the heights of abstraction.”

There’s a sense of awe that accompanies vastness. The extremes of size, from the vastness of the ocean or the vast blackness of outer space or the vastness of grand armies move us emotionally.

When you move sufficiently high up levels of abstraction, the vastness becomes beautiful and overwhelming.
When you look at reality from multiple levels of abstraction simultaneously, the vastness of perspectives becomes beautiful and overwhelming.

Abstraction is the making of consilience, about the unification of knowledge. With abstraction is an instance of shared structure, binding together that which always was together but had not been recognized to be together. There’s this corrective motion, from the separateness of things to the connectedness of things, which is accompanied by a sense of wholeness.

Abstracting over this process rightfully generates awe. The pattern is that you watch the connections between objects appear over and over again, and you generalize to the sense that even if you’ve failed to see or appreciate it, connections exist between every object. The feeling of ubiquity and the presence of connectedness is that generalization. And so you invert was was a hidden assumption - you move from assuming that connections don’t exist and that boundaries are real as a default to assuming that there is some notion of similarity that will hold between all objects as a default.

It’s fairly ridiculous to claim that two objects have nothing in common (taken literally). Even the existence of boundaries is a type of connectedness. But say it was true, that two objects had nothing in common. That no pattern found in one was found in the other. Then, immediatly, knowledge of one object would give you fascinating knowledge about the other objects. Every pattern that occured in one would be known to not occur in the other. And because many patterns repeat frequently across almost all objects, if the objects had any level of complexity there would be a fascinating challenge in maintaining the patternlessness between them.

There is not disconnectedness (for even disconnection is a form of connection), there is randomness.

There is extraordinary power to seeing the connectedness of things. In many contexts (category theory, neurons) the connectivity structure dominates or is all that matters. You can know an object by what it is connected to - this principle shows up in word vectors, using this strong heuristic to create rich semantic representations of words that can be compared to one another. In a neural network, the learning of the connection strength between neurons is a general path to representing knowledge.

The project of the unification of knowledge is grounded in finding shared representations across domains. Problems can be re-represented as one another, and intermediate, generic abstract representations (ex., data structures like graphs or hierarchies) can link the kinds of solution (algorithms, re-representations) that work across systems that at surface level look distinct.

The project of the unification of knowledge:
Find a sufficiently general knowledge representation
Map it to a body of mathematical structures whose frame can be used to automate transfer
Fill the general knowledge representation with data
Learn a notion of conceptual similarity that allows the comparison of arbitrary words, phrases, sentences, paragraphs, texts
Link this to the internal brain state of a person thinking about the concept (Really, everything)

Abstraction to Transcendence

There are a few conceptions of transcendence which are accomplishable via abstraction.

Gestalts (wholes that are more than sum of parts, via generalization)
Lower state as trivially accomplishable by a higher state
Moving from the concrete to the conceptual
Being unknowable, unmeasurable, unseeable from the lower level
Set theoretic - one dominates the other, in a way that leads to full containment (but also much much more)
Ultimate generality / universality
Generation of universes

For each, 1. why it relates to transcendence and 2. How abstraction accomplishes it:

Gestalts

The creation of wholes that are more than the sum of their parts can be accomplished by abstraction. Take the creation of axes from properties. You can take two or three objects, and notice their shapes. For each aspect of shape (their heights, the eccentricity of their curves, etc.) there’s a particular measurement for each object. But taken together, the objects can be seen as datapoints in a space of possible objects that is defined by the axes that measure the properties that the objects have.
This space is much more general than any of the particular objects, and immediately creates a generative model for new objects: propose a new point in the space, and something new (though admittedly, it’s the restricted newness of interpolation / extrapolation rather than the creation of new axes) is brought into existence.
The perception of a gestalt, that is a more general frame out of access to limited information, is power by the discovery and generalization of shared structure found between sets of facts. It’s the generalization that can follow pattern recognition. 

Lower state as trivially accomplishable from a higher state

In mathematics, representations of operations in the abstract (say, addition or multiplication) are general, and much more valuable than trying to deal with each problem on an ad hoc basis. The transformation of the operations from being about particular objects into numbers in the abstract is what allows umpteen situations to be efficiently compared to one another, turning every particular instance of a problem into a trivial and solved operation. In noticing the shared structure across addition or multiplication problems, and learning to map situations to that abstract representation (and filtering out the details that are irrelevant, say of the kind of object being added or multiplied) we can do strong transfer between umpteen situations. 

Moving from the concrete to the conceptual / spiritual

The conceptual is tied in with the transcendent because until the transcendent level is reached it exists as a conceptual possibility but not concrete reality. 
There’s also a body of properties that concepts have that tie them to religious notions. They exist outside of material reality in that the patterns that are observed (say, the laws of physics) are invariant to any action that we know how to take. Abstract representations of numbers are deeply valuable to us in an immediate way without having a clear material instantiation. And so the sense 1. That these things are real and 2. That we are incapable of interacting with them puts abstraction to them in the regime of the transcendent.

The conceptual and the spiritual are abstract patterns, rather than concrete objects that can be physically intervened on in the way that we are conventionally accustomed to. There’s a sense that the spiritual world (which exists in the minds of believers, as does other currently understood experience in this solipsistic world) is composed of these conceptual objects.


Being unknowable, unmeasurable, unseeable from the lower level

There are operations which can be performed trivially at the abstract level (say, because efficent algorithms have been discovered that operate over a dataset) that would be unseeable from the lower level representation of the problem as seen at first glance. Re-representing the problem in the abstract makes umpteen solutions available (both from transfer and from the way that solutions interact with the new shape of your problem) that makes possible what would feel magical.

Ethics

Expanding the scope of tribal instincts has been a classic path for ethics. Familial and tribal bonds enable tight knit trust and cooperation. Abstracting out to the scale of towns, cities, nations, humanity, and eventually all living beings as a whole has been a natural path for ethicists looking for generality in the principles that govern interactions between living creatures.
Tradeoff Between Concept-relevant data and Precision

One way to see inductive / empirical / analogizing / abstractive thinking is as operating by doing transfer between similar datapoints. (As opposed to causal / deductive / rational mode, though this distinction becomes fluid.)

Abstractions alters 
The amount of data informing inference
The closeness of the connection between the objects in question


Abstraction tries to bridge a similarity gap between datapoints, but simultaneously makes more datapoints accessible for inference.

For example, abstracting from (time, money, attention) up to (resource) gives you many more relevant datapoints, but the intersection that’s relevant shrinks. For example, time as a resource is finite and unchangeable, in a way that money and attention are not. And so in crossing the similarity gap there’s conflation that can damage your ability to think, if you assume that you can always acquire more of a resource and expect that model to cleanly generalize to time. But you do want to generalize concepts like opportunity cost to all of them. 

What is the value of additional data?
When building a model over small data, it’s easy to over fit to those datapoints. Generalization fails because the probability distribution that data is drawn from has a range far outside what exists in the training data.
Small data makes the prior more important, and so the models fit tend to need to be much simpler (often excessively simple) to maintain generalization capacity.


What damage can be done by attempting to bridge the gap?
Conflation of unlike objects can lead to illegitimate inference. It’s critical to know which structure is shared and which is not - this allows clean navigation of the tradeoff, by only doing transfer from datapoints which are similar enough to a new instance to validate the transfer. Or by smoothing over differences between datapoints, giving smaller weight to those that are less similar.

Tradeoff between working memory and conflation

Crudely saving working memory and dropping the distinctions in shared structure is often more efficient, but you eat the tradeoff whole. Doing deconstruction over an abstraction and making the relevant distinctions prior to transfer trades off against computational time and working memory, and so ideally you create abstractions that are clean enough to be efficient. Constantly going back and making distinctions is expensive, and so is the damage done to thought through conflation. 

And so the abstractions that minimize conflation while compressing the representation bridge this tradeoff, improving efficiency and generalization in thought.

Ways in Which Abstraction is Done

I’m going to enumerate the type of abstraction done in each of the examples I have, and attempt to categorize them in some coherent way (taking the idea of abstraction and trying to go to a lower level, dividing it into particular types).

The class dog contains properties of dogs. Instances of dog have individual properties and shared properties. This is an example of going from a set of objects into a concept that unifies them. 
But the other way to abstract is from individuals to species - they’re unified by the ability to interbreed. And so it’s a way to create a subset. 

The appropriate intermediate abstraction here may be set theory - we divide a space into subsets based on some criteria or shared property. 

Orange, Apple, Banana - unified properties

What does a function do, fundamentally? It takes some behavior, and creates a shared structure where the behavior is modified on the basis of arguments. It abstracts over individual instances of the thing that the function does. Say you want to create a box, and the thing that changes is the location. 

The removal of particular aspects of a problem, like generalization in mathematics.

Structure as constraints?
Properties as a particular type of structure (akin to an existence constraint)


Shared Properties
Dog vs. instances of dog (interbreeding)
Dog vs. instances of dog ([categories of property] - shared snout size property, breed property, color property)
The class for Orange, vs. instance of Orange
Apple, vs. instance of Apple
Banana, vs. instance of Banana
Animal, vs instances of animal (dog, cow, etc.) - shared properties (eats, sleeps, makes noise)
Fruits vs. instances of fruit (shared ripeness duration, water content, some color)
Graphic object vs. instances (lines, rectangles, circles) where they share position, orientation, etc.
Shared Structure
Functions, generally
Compositionality



Difficulties in Thinking About Abstraction

What you mean when you say a word is usually to activate some but not all of the words associations. And the distinctions required to disentangle those associations are innumerable.
Multiple objectives to a set of thoughts, say 
to be communicable (that is communicate the right message), 
to be useful in a practical sense, 
to be truthful, 
to be efficiently represented (even though brevity requires abandoning complexity that may be necessary in some situations but not others)
Etc. whose conflict involves tradeoffs where you may be willing to make a number of mistakes so that what you’re saying can be easily understood. But then you start thinking with that representation yourself. 
There are no words which fail to conflate unlike objects that describe what you’re trying to describe
Collapsing a space into a single object
Using the wrong axes to perform an evaluation (ex., how similar are these objects? Is very easy to evaluate in a way that doesn’t respect the goal of the comparison
Worse, the sense that the evaluation is conditional on the purpose of the evaluation may be lost. The notion of similarity will be taken to be objective, true for all possible goals.
Incomplete decomposition, missing important sub-categories that makes the model feel clearly broken (even if close the the principal components for many goals are captured)
OMG, we need a prediction focused PCA which balances the goals of variance maximization and maintaining predictive capacity
I guess that this is what LULZ is supposed to be
Ex., Intelligence -> analytical, creative and practical intelligence (Sternberg)
There’s this immense harm in thinking that knowledge representations need to be literally true. Sternberg’s model may be the most useful for many tasks, efficiently making tradeoffs that are necessary tradeoffs to be made for any model. Brining a strict standard of truth to it and evaluating it on that basis fails to respect the reality that there are multiple objectives to these models.
We end up in a world with mathematics and data are all that fail to die to purity, a world where making conceptual progress is impossible because all concepts can be destroyed by our standards.
Yet every day, we live by these concepts, we think with these concepts. And we’re neutering the process by which we improve them
In so many cases, things aren’t right or wrong but are more right or more wrong. Spheres are reasonable approximations to the space of weights SGD can get to in n steps, even though the reality is much more complicated.


Terms, How People Talk about Abstraction


High Level vs. Low Level
Grain (Coarse Grain vs. Fine Grain)
Broad vs. Specific
General vs. Specific
“Broad brush”
Concepts, Conceptualization (Boyd, Dad)
Comprehensive Whole vs. Particulars (Boyd)


High Level vs. Low Level

There’s the ubiquitous reference dependent ‘high level’ and ‘low level’ type or reference, where the speaker has in mind some reference class level (often contrasting the high using the low as a reference point, and using the high as a reference point to define the low). 

This tends to lead to unnecessarily binarized thinking. Ideally the language would auto-capture that there may be a high level and a low level, but there’s also a level higher than low level but lower than high level, and lower than low level, and higher than high level, etc. The use of almost all of these terms relegates us to two levels by default. Though maybe that makes thining easier for the reader. And also, perhaps it’s not binary but points to a ‘gradient’. More true for coarseness vs. fineness than high vs. low.


Coarseness vs. Fineness (Literally true in the case of abstraction in image processing)
Grain (Coarse Grain vs. Fine Grain)

I really enjoy how this version implies a continuum of abstraction - it’s clear that you can become incrementally more coarse, or incrementally more fine. And so it’s appropriate for those situations where the abstraction is continuous. It’s also flexible, and can be used for discrete situations that are more or less fine / coarse than one another. 
But it struggles in another context, where there’s strong discreteness. Take the version of abstraction involved in creating a function, or in creating a variable instead of using scalar values. The metaphor (coarse vs. fine) starts to break down. 
This is in part because coarseness vs. fineness assumes that the type of abstraction is exactly the same throughout! In the metaphor, you only get more or less resolution. You never switch to a different type of abstraction. And it’s hard to model a binary discrete situation with this, where there are exactly two levels. May be nicer if there are more levels, but we also have to keep the type of abstraction the same.


Broad vs. Specific
General vs. Specific
“Broad brush”
“If you ask a more specific question, I can give you an answer.”, is what Scott Kominers would love to tell me. 
People love to use the term ‘broad brush’ to give themselves permission to not condition on subsets of populations, or to make general claims in a way that’s unrigorous. It’s both valuable and dangerous - dangerous in that they don’t expect to go into details on their claim, which makes these kinds of claim extremely hard to evaluate, verify or argue against. Or often arguing against consists of picking a counterexample, which the person admitted would exist when they said that the statement would be broad brush. It’s valuable in that these summaries across populations end up being critical for decisions that depend on the proclivities of a large number of people. And it becomes extremely difficult to reason about a space if the level or rigor required makes it hard for people to make claims that look true to them. 

Concepts, Conceptualization (Boyd, Dad)

This points to the way that abstract objects often move from particular grounded objects to the immaterial concept of the object. This conceptual frame is often more general but more difficult to operate on - there are generally missing features belong to a particular instance of the concept that would allow operations to be run over that object, at a detailed level.

A conceptual understanding is an understanding of the way that ideas come out of base data, and often the way that those ideas interact with one another. The implication is that you can operate over much more data by abstracting a substantial group of data into a concept and then having that concept interact with other concepts improve at the conceptual level in a way that generalizes to every example of raw data that’s connected to the concept.

Comprehensive Whole vs. Particulars (Boyd)

There’s a wholeness of vision that is capable of considering the interactions of multiple high level objects. Those high level objects (required to see what feels like the whole) have to be constructed out of lower level components in ways that aren’t leaky or overly destructive to predictive ability.

Particulars (ex., detail orientedness) allows for the interaction with the explicit instantiation of your comprehensive whole, usually put together with concepts. 

General-to-specific (Boyd)

Whether the specific is across time, across objects, or other relationships types, the motion from a particular  to a general representation of it (say, form a particular sponge with the concept of sponge)
If you’re trying to re-generate the input we can use a VAE - elsewhiese (for sequence data) and we can do some machine learning over the video, over the content, etc.


Hierarchical Structure

Hierarchical Structure
Bottom Up
Compositional
Width-wise compositional
Depth-wise compositional
Combinatorial
Counters curse of dimensionality with representative capacity
Discrete
Offers multiple levels of abstraction for interaction and prediction
Types of information with Hierarchical Structure
Abstraction
Images
Objects - Object Parts - Shapes - Lines / Curves
Audio
Words - Phonemes
Businesses / Governments
Sciences
Physics
Chemistry
Biology
Ontology of Species
Organ Systems - Organs - Tissues - Cells - Nuclei + Organelles
Brain
Natural Language
Fields - Concepts - Words (Combinatorial as well)
Paragraph - Sentence - Phrase - Word - Character
Time
Centuries - Decades - Years - Months - Weeks - Days - Hours - Minutes - Seconds
Measurement
Kilometers - Meters - Centimeters - Millimeters
Object Oriented Systems
Classes - Objects
Economy
GDP - consumer spending + investment + Government Spending + Exports - Imports
Top Down
Recursion
Homogeneous
Discrete
Generative
Deconstruction
Offers multiple levels of abstraction for interaction and prediction

Bias Variance

Bias-Variance and Abstraction

[Need: The way that Abstraction / Compression increases Bias, Lowers Variance]
There’s a powerful generalization from the bias variance tradeoff in modeling to the standards by which we create concepts and the quality of those concepts representation of the world and generalization through their use in future thought.

When we decide to create a new concept (one quality example is a new word), we use it to tacitly collect data that corresponds to the category that it outlines. Take the concept of dog as a label that shares information through a class of objects that are similar along many axes. It effectively bundles information about that object that will allow anything that’s recognized as being a dog as being likely to share the properties of the other dogs that have been seen in the past.

(Need an example that can demonstrate fluidity more effectively)
One important downside of this binary classification (where all objects are either dogs or not dogs) is that the conflation between different dogs 


Another consequence is that without the creation of a higher level class (say, animal) it isolates the data that belongs to the dog class to that class. Because categories are attractors, it’s not feasible to have a category that’s closeby without it being subsumed / replaced.

It can be useful to share learned information even more br

Bias variance is one instantiation of Occam’s razor.

Point 1: Bias Variance Tradeoff and the variance of a probability distribution
Variance in the bias-variance tradeoff refers to the concept that when you’re searching over models, some models have more flexibility. When they fit a dataset, models with more flexibility tend to overfit, because they find a separating hyperplane that is overly accommodating to particular datapoint. There are many ways to tend to overfit, and variance is an abstraction over all of them. 

There’s valuing fit over smoothness. 
There’s valuing a single datapoint in a region with sparse data over the impact from other datapoint farther away that you can interpolate from or extrapolate from. (Looking too much at particular datapoints)
Arbitrarily overweighting one representation of the features over valuable others, incomplete search over the set of feature representations

Related:
Decomposition over Regularization
https://docs.google.com/document/d/1tCoaZEzERE3XP_4SzJWJhQ17bnY7vfUGYPGnCCEO54I/edit?usp=sharing

Levels of Abstraction, Abstracting Over an Incomplete Subset
https://docs.google.com/document/d/18FvL9mlKTDlxQVXju1v8vOV63U73-6f9WVGh9-d8ScE/edit?usp=sharing

Treating Variance in the bias-variance tradeoff as a concept, there are many ways we could instantiate it.

The standard way, watching your model overfit. This approximation of variance is the difference between the training error and the validation error. (Bias will affect both your training and validation error equally)
Bootstrap sampling variants of the dataset
Split between in and out of bag examples
Train on the training sample, test on the testing sample
Variance is the ordinary (distribution) variance of your predictions on a given datapoint (assuming regression). You can compute the average variance across datapoints for your model’s variance.

The number of hypotheses that can be learned by a model (say, the number of features in a dataset for a decision stump, and all of their interactions for a singly branched tree)
Across different representations of a hypothesis space (parameters, freedom over those parameters, number of parameters, rules, freedom of rules) these are different approximations of the variance. But a wide hypothesis space tends to cause high variance, it’s not variance itself.

Say that your model’s predictions of a datapoint are Cauchy distributed. Would you say that since its variance is undefined, it’s not subject to the bias-variance tradeoff?

Variance of a distribution 


Variance is complex hypothesis classes leading to overfitting

Just because a concept is formalizable doesn’t mean that the concept is its formalization.
There’s something like map-territory here. But it’s higher-map lower-map.
We need a clean way to distinguish between concepts and their formalization.
Would you say that ‘attention’ in deep learning is attention? Of course not. Attention is so much bigger than that.

Examples of Bias Variance, and how Abstraction increases bias while lowering variance:
Myers Briggs works extremely well. 16 categories are structure that introduces bias, due to the difference between the simplification that comes from the assumptions and the variance that comes if you have constant data. You can imagine having 1600 categories and the same amount of data, but matching the underlying structure of personality much more closely. This would be a dramatic reduction of the bias at the cost of blowing up the variance (because very few people would fall into each category, and their idiosyncrasies would overly influence our sense of what each personality category was like).
These categories were created by generating 4 abstract properties of people and looking at the categories that come out of treating those 4 properties as binary, one or the other switches. Extroverted or introverted. Feeling vs. Thinking. When we overcategorize (say, generating orders of magnitude more properties of personality) we thin out the data of people in each category (and so may need a system that can effectively do transfer from similar-but-not-identical categories). 


If you fixate in system 2 type thinking, logical, delibarate thinking, you have high variance. You don’t have variance problems that you can point to directly, just in the way that any single predictor will be higher variance than if it’s part of an ensemble. 

But you also have massive pointable-to bias problems if you’re a man with a hammer. It means that the assumptions that you make to apply your hammer are out of line with the underlying reality. Man with a hammer syndrome points to high bias resulting from misfits in model and the world.

Basically the goal is to put all of the relevant (where relevant is defined as sufficiently low bias, where the assumptions fit the situation) models into an ensemble that can be low variance as well and so generate accurate predictions.

Abstraction and Systems Thinking

Proper level of abstraction example is to think about the economy - at the entrepreneur's level, you dislike volatility, as it kills you. But at the level of the system, volatility leads to growth. [Taleb]

The way that systems operate is general, in a way that abstracts away from the details of systems in particular. This makes it a beautiful example of thinking at multiple levels of analysis. 
One quality example is the entrepreneur (object level) vs the system (say, the body of businesses and the capitalistic system driving them).
What is good for the system and what is good for the individual are often in conflict. Similarly to the way that an individual animal is unlikely to benefit from the mutations that lead to variability in its genome relative to its brethren, entrepreneurs don’t benefit from the reality that they are likely to die in the same way that the system as a whole benefits from their collective risks. 
This is a beautiful explication of transfer. By abstracting from the indiviual level to the system level, we can compare patterns across systems as diverse as evolutionary processes and the growth of a capitalistic economy and the personal journies we all find ourslves on.

Beautiful Example of Shared Structure in Systems

There are a number of interrelated ideas that I’d like to connect. Those are Optionality, Trial and Error, Exploration-Exploitation, Experimentation, Natural Selection, Comfort Zones, Creative Destruction, and certainly a swath of other critical ideas. These are unified by the notion of volatility, and the effect that volatility has at the level of every system that’s impacted by these concepts.
 
The central idea is Optionality - in many cases, you get the upside from volatility. You sample over and over from a distribution (you can imagine meeting potential friends/romantic partners, or trying out classes or a major at college, or there being many mutations of a gene in a population) and take the best, or at least the better, option.
 
In all situations like this (and they are everywhere), volatility is more important than the average.
In Exploration-Exploitation, optionality lets you exploit by taking the best solution thusfar and using it as your model for behavior. When there’s high variance in what you’re exploring - say you’re sampling different dishes at a restaurant - if some dishes are amazing and some are awful, you get the upside - amazing dishes all the time - as soon as you start exploiting. If there isn’t much volatility - if every dish is basically the same - even if the dishes are quite good, you don’t end up as well off as when there’s variation that you can take advantage of.
Personal experimentation is a form of exploration, where you try out a new behavior, style of living, or a new habit. When there’s more variation in the change in life quality, you get much more out of experimentation.
Natural selection benefits from high levels of mutation in a population, because that allows for faster adaptation to an environment and faster improvements in fitness at the species level.
In Trial and Error, there’s a binary outcome and you sample over and over until you get a success. Then you can use that success again and again.
People who are said to be staying inside their comfort zones are suffering from the absence of optionality - by refusing to explore the space, they end up with a weak payoff.
Creative destruction is critical for the growth of economic systems, and thrives off of the volatility inherent in the life and death of industry. By taking the upside to variance, capitalistic societies grow off of optionality.
This foundational principle underlies almost all value creation. It calls for us to optimize systems for volatility, not average capacity. Education, business, personal lifestyle - all of these have much to gain from volatility. And so the common heuristic that volatility is bad or dangerous or scary is only true at the lower fractal level. At the system one level up, the variance is essential to growth.
 
Search as Abstraction
 
We can see search as a problem that cuts across many domains, where once we re-represent our problem as being search lends itself to immediate and powerful transfer from every other domain where the problem has been solved.
 
Search in artificial intelligence, social communities, and physical reality all share upmteen properties. The way that you map currently seen options, evaluate future opportuniteis for search (option value in behavioral economics, where there is an expected value to uncovering new information), the way that successful search leads to the ability to double and triple down on successful options - all of these domains share enough properties that by having a term that we apply to all of them we can start doing implicit transfer, and where if we apply ourselves we can achieve strong gains by doing explicit transfer.
 
The shared structure in the problems looks like a number of points (in person space, real space, model space) which have some cost of transport to other points and some revealed value of those poins as the space is explored.


Knowledge Representation, Reasoning and Question Answering

Deep learning has been successful in natural language processing in large part due to embeddings for words and for symbols. Research on creating embeddings for phrases and for facts is important for the future of knowledge representation.

It would be great to be able to represent relationships between objects. Say, represent relationships between numbers or between mammals. The relationship of less than or greater than or belonging to the same set.

We can represent this information in a structured language format that has a verb (that defines the relation) as well as a subject (the first entity) and an object (the related entity).
There is a second kind of relationship, an attribute, where a subject has an attribute. 

The ‘relational database’ is generally used to store these types of relationship.

Change - Dude. They use “Neural Language Models” again to represent word vectors, and much more explicitly here - “learn a vector that provides a distributed representation of each word”. This so needlessly breaks with the way that every other resource talks about this concept.

Knowledge bases are large sets of these types of relations. 

It would be great if we could use relations in a knowledge base as training labels in tandem with a large corpus of text (say, wikipedia) and learn new relations automatically with high probability to fill out the knowledge base.

Knowledge bases have also been used for word-sense disambiguation.


Fundamental Questions in Representation Learning

Why Representation Learning?

The way that a problem is represented can dramatically change our perceptions of what the problem is and how to solve it. Problems that look nearly impossible, if re-represented, suddenly become tractable.

One obvious gap is from a conceptual representation of the problem to a mathematical one. Representing a social network or communications network as a graph allows us to do operations like search or optimization over the representation. Representing a person by their connections with a vector lets us measure the similarity between ostensibly very different people quickly and efficiently. Representing a word as a vector that depends on its surrounding words does the same.

There always is a representation. And so you can improve your ability to solve a problem representation side (by reformulating the problem) or on the solution side (by reformulating your solution assuming the given representation).
The reason for representation learning is that you can optimize the representation of the problem for the task at hand, with a particular parameterization of the space of possible representations of the problem.

Downstream from a quality representation is the ability to re-use parts of that representation to quickly adapt to new environments, experiences and tasks. And so learning modular representations is critical. Humans have modularity built into our grammar, and so can use language to effectively slot descriptions of actions objects into our conceptual and communicative scheme. Attempting to transfer with a representation that is at the wrong level of analysis will fail, and so the best representations allow for flexible motion between multiple levels of analysis which create a surface for transfer. 


Why Learn Discrete / Sparse Representations?

Once you have a low dimensional discrete representation, a wide body of important algorithms are made available. 

Concept recombination
With sparsity it’s possible to run inefficient algorithms, for example looking to the set of combinations of a set of concepts. Those interactions can only be looked at for a small subset of the feature space - doing it at the level of pixels and in a continuous space would be computationally intractable. 
Causality and its establishment
If you want to do counterfactual learning, you have to find an abstractive representation of time (both the time over the action and over the outcome) and you have to find an abstractive representation of the action space.
Creating a causal graph requires a high level representation of parts of your environment and actions in that environment.
Credit assignment (to higher level objects) made efficient
Hierarchical control
Decision making over conceptual blocks of actions
Higher level planning

Why Learn Continuous Representations?

In a continuous representation, one option you have is to have each axis represent a quality that can be had in greater or lesser proportion. And so you represent your object as a vector of many qualities (decomposition) which vary across a continuum (fluidity) and so have extraordinary flexibility.

An example of that flexibility is that if you have two object, alike in some ways but different in others, whose similarities you want to take advantage of in some contexts (say, the weight of two balls being similar, but their colors being different) you can represent that with a two dimensional vector with a continuous representation of the balls. In a discrete representation, both color and weight are represented very differently (with approximations or collapses) and can’t be merged in useful ways.

In the continuous representation you can also re-combine the representation in umpteen ways. You can you masking to average some vectors and not average others (when merging two concepts) to create novel vectors which a generative model can create a low-level representation of and which can be compared (in terms of its performance on some downstream objective) to the concepts that are already in your representation.

When you’re abstracting, you want to notice where there’s conflation and where there’s shared structure.

I’d like to note that this is an example of a dense continuous representation. There are sparse discrete and sparse continuous representations as well.

The data is also often high dimensional, with each high level concept having innumerable sub-concepts or attributes or properties that can be seen as axes in the concept vector. 






Notes & Thoughts
I may want to rename this book to ‘Representation’
And also orient the content towards that
That’s the true motivating idea
I care about decomposition / deconstruction as well as abstraction
New definition - Abstraction is going to the general from the specific.
I need a section on how abstraction is core to intelligence, core to thinking
I need a section on how language and writing facilitate abstract thought
Another good source of examples: The creation of Theories (that unify) out of sparse facts is one of the most powerful examples of abstraction.
Take evolution. It’s was generalizing from the way that Darwin’s finch #1 and finch #2 populations transformed over time to the way that every single living creature has transformed across time.
It would have been interesting, if Darwin learned something about the way that finch populations transition across time. Some early Zoologists may have been fascinated. But it’s the motion of abstraction and generalization that makes what he did immensely powerful.
Now when we come to a new animal we’re loaded with generalities (like evolution) about the way that creatures like that work which allow us to much more efficiently model what is happening with ostensibly ‘new’ data.
Elucidate the differences between abstraction and compression
Find cases where the whole is more than the sum of the parts. This is an upside to abstraction (emergence! Get this from particle physics and anywhere else that it’s grounded) that I haven’t elucidated (or seen, tbh)
Ideas

Trade-off between compositionality in a concept representation and appropriate engagement, so that well delineated concepts can be flexibly recombined to hit a large part of semantic space and so that updates to concepts that have shared structure affect all of the concepts with that structure.
There are some context where ‘idealized abstraction’ just looks like going to the lowest level possible and dealing with all of the information that exists (say, you could write one-off code for every object you create). There are other contexts where the higher level representation (say, groups of people) have impacts as a collective that don’t exist at a lower level, and so the only accurate model of the system needs to abstract, understand the impact of the collective on the individual, and generalize from that. 
The mysticism around ‘Emergence’ is just a modeling error where people only abstract in one way (say, down to cells) and don’t include something important like the interaction between cells in their reductionist model of the system. It’s like creating a graph without the edges. And so when those effects have manifest consequences at a higher level, it feels like they appeared as if by magic. 
The ‘type’ of abstraction done as a structure that is transferred between domains. Ex, the function of the lower level, the units at the lower level, the properties of objects at the lower level.
Perhaps, in the abstract, we can enumerate many / most of the types
Can think of abstraction as used to learn a representation that we can use non-compositional, non-hierarchical structures to reason about (as abstraction to the appropriate level analysis reveals the structure that allows the problem representation and solution to be compressed / maximally efficient.
A notion of cognitive fit is a general felt sense representation of similarity. Another form of tacit abstraction, without concretely knowing what the abstract object is.
Two modes - Hierarchical Compression, Shared Structure
Shared Structure can be out of the use of a tool or concept, the components that make up the tool or structure
Inverse Abstraction (Deconstruction, or Instantiation)
Generative - Creates new information
Break into component pieces, in multiple directions
Ex. Machine learning becomes Linear Algebra + Calculus + Probability Theory + Computer Science, which break into their own subregions
Ex. Scientific Field becomes Major Papers + Categories of the topic + Conferences + Major Researchers + Quality Sites
Biology, in creating an ontology, has tried to find unambiguous set separators with some success. Examine this abstraction in detail, it has very interesting properties.
Evolution divied up the space for us to come and make abstractions over.
Need to distinguish between composition and abstraction. Composition implies hierarchy (even 1D), but abstraction is just an instance of hierarchy - not all hierarchies are abstraction.
Distinction between abstractions that cover all possible subsets, vs. abstractions that are ‘dirtier’
Proper level of abstraction example is to think about the economy - at the entrepreneur's level, you dislike volatility, as it kills you. But at the level of the system, volatility leads to growth. [Taleb]
Difference in kind when your abstraction models the causal model for the data, as opposed to some derivative features.
(Perhaps) You can only switch between type of abstraction if you use discrete steps. If it’s like coarseness vs. fineness, or on a continuum, you don’t run into the switching between types of abstraction problem.
Chunking in the memory literature as a form of abstraction, where patterns found in information let a person create a group that distinguishes those bits of information.
Contrast between variance as information and true probability distributions. 
You can use the probabilities that people assign to events as well as their beliefs to infer the abstractions that they created over subsets of a class.
The ways that people violate results from set theory in the way that they use / apply abstractions as a source of content (in the same way that behavioral econ looked for violations of probability theory)
Language is an example of where abstraction has occurred in going from higher to lower levels; there are common roots to words, which were later differentiated to form specific use cases.
Chemistry and the naming of chemical compounds (IUPAC) has a very explicit way of doing this, and is a formal system
Speaking of differentiation, stem cells!
Idea: modularity (taking advantage of combinatorial structure)
Computer Science (Libraries, microcomponents, functions, etc.)
All of language (words as modules that are combined in flexible ways)
Chemistry Compounds
Fractal / layers of abstraction. Also, conceptualization. So many different words for referring to levels of abstraction.
Appropriate level of abstraction for economic intervention by the government - changing the structure of economic growth (legal system, economic freedom, monetary policy) rather than direct intervention in particular economic spaces (stimulus, public works, subsidies)
Tradeoff between volatility and expected value in improving your representations of concepts
Diminishing marginal returns to search - high expected value ideas first
Transfer and Metalearning are downstream from richer and dissectable representations, especially concept-level representations.
Some words are concepts themselves, but sentence and paragraph level representations let you encode the concepts that are a recombination of words.
Concept-level representations are the appropriate level of abstraction to transfer across domains and between modes in a world model, including transfer to human minds (interpretability) necessary for alignment, interruptibility, etc.
Ontological mistakes in thinking about representation learning
Concept Learning
Ungrounded
New embeddings from relational structure in knowledge bases
Concept Parsing
Heuristics for separating out concepts in a sentence. Or label it and learn to separate concepts, perhaps integrating part of speech tagging.
With concept parser, create concept embeddings
Grounded
Cross modal transfer for interpretable representations
Concept Level Representations through NMT
Optimize representations for transferability between tasks. This is “the real key” to useful abstract knowledge.
It’s a representation optimized for performance across many many tasks. That’s how you know which abstractions are worthwhile, which ones are shared.
Remembering the thought that probability distributions should be parameterized and approximate rather than assumed to be gaussian or whatever. Look at the empirical distribution and map it with a parameterized histogram or something like that.
It’s sad that generative outputs are either continuous or discrete. Both will be missing an important category of representation.
High and low in the network gets conflated with high and low in abstract space. In that space, the most general features (that are shared among many datapoints) are curves and edges, and the less general features are class-specific. Which are the more abstract? The recombination of the input features? Or the more general features? If abstraction is that which is shared among datapoints, 
By definition, concepts (like classes) are abstract. Lines and curves are concrete.
Topics in Computer Science
Abstraction and de-duplication
The way abstraction can simplifies representations (simplifies code)
The way abstraction can make interfaces flexible (with a single interface working well for all sub-cases, rather than many interfaces for all sub-cases)
Full survey of data structures as examples of abstraction and representation
Functional programming (monads)
Hiding implementation (as a downside)
Allowing flexible modification of implementation (without the users of the abstract interface having to modify behavior)
Classes as examples of abstraction
Functions /methods as examples of abstraction
See generalization as 1. Having something that generalizes and 2. Something to generalize over.
X generalizes to Y
See generalization itself as an operator that relates a thing that generalizes to a thing being generalized over.
How do we operate over that operator?
Generalization is a function. What higher level function takes that function as input, and operates over it?
What changes can be made to generalization itself?
What is generalization an example of, a single datapoint of?

Related Fields / Idea Spaces to Cover

Object oriented programming
Bayesian Probability Theory
Set Theory	
Language
Connotation
Analogizing (As an instance of transfer, read Douglas Hofstadter on the topic)

Resources Worth Creating

To Create: Fundamental Questions in Representation Learning
Create a list of accepted truths in DL. Especially those believed by the high status (Hinton, Bengio, Lecun, etc.) Ask which accepted truths researchers believe are wrong and why. Invert all. 
I want to create a curriculum that’s OLD. Exclusively papers from 2000 or earlier. (Hint: Old papers only cite other old papers. And check ICA.)
Take every objective in ‘What Makes a Representation Good’, add my own objectives, and for each one specify:
A way (or set of ways) to measure the objective
Distinguish between the concept of the objective and the mathematical instantiation of the objective (unless they’re truly identical)
The downstream consequences of doing better or worse on the objective
Compare two different networks over the objective
The rationale (and intuition pumps) for the objective
The counterarguments
Apply inversion to all of the ideas in a frontline paper. When it works well, you’ve discovered something you think is true that others disagree with. And if it’s a foundational assumption, you can get started on making progress.
How do we know what we claim to know? Ask this of a shortlist of ‘sacred beliefs’.
Create a ‘sacred beliefs’ in representation learning list.
Create a ‘consistently questioned beliefs’ in representation learning list.
Why learn Discrete / Sparse Representations? Be able to give a fully fledged, fully throated defence and attack.
Why ‘representation’ is this crazily important concept. The dramatic, windfall differences that come out of slightly different representations.
Survey all possible papers I could push hard at in Abstract Representation Learning
Explicate all my categories of idea as low level ideas
Generate new categories of idea
List out all of the goals for representation learning as a field and multiple pathways that would fulfill each goal
Order the goals in terms of importance
List out the unknowns, the missing categories, the assumptions behind the goals,  and the mistakes
List of likely to be true / likely to be false assumptions, and ways to prove or disprove each assumption
Transfer between each related field and representation learning
Decide what the goal is. Work backwards to research paths that accomplish the goal. Value parts of the research frontier insofar as they relate to the goal.

Book Organization

At this point I’d like to structure things more finely. Look at what’s general across what I’ve written, and get to a set of unifying high level concepts to make chapters out of. I’m going to list the painfully obvious and necessary topics (in order of necessity) first.

Similarity
Transfer / Generalization
Compression
Properties of Representations
Composition
Modularity
Discreteness vs. Continuity
Structure / Invariances / Types of Relationship / Pattern Recognition
Pitfalls & Failure Modes
Conflation
Due to over-compression
Leakiness
Grounded vs. Ungrounded


Potential chapters
The way that abstraction in language leads to unnoticed poor models of systems (abstraction in social systems, politics)
The value of abstraction in transfer, in generalizing across tasks
Power of abstraction, being able to represent huge amounts of information (information theoretic perspective) with extremely succinct concepts, being able to build on those representations 
Working memory limitations and the use of abstraction to overcome it
Leaky Abstractions, which seem to summarize information but in reality expose the underlying information in a way that forces the user of the abstraction to be extremely careful with it - danger of building on top of leaky abstractions
Importance of operating at multiple levels of abstraction. Bottom up and top down, for full understanding of systems.
Doing tasks / communicating / operating at the proper level of abstraction, and the results when this is done at the wrong level (ex, human language being too high level for many tasks)
Example from Physics - Newton is right at one level of abstraction, and wrong at another level of abstraction
Truth is only right or wrong after you choose a level of abstraction at which to determine truth. 
The ways in which you verify alignment of an idea with reality change depending on the level.
The discreteness of abstraction
The idea that a canonical solution to the level of abstraction problem is to go to the lowest possible level, and this being prohibited by the discrete nature of reality
The true representation of concepts is continuous (in the brain) and then discrete again - we’re operating two levels above the true representation. 
Scientific disciplines as distinguished by the grade at which we interact with reality, from lower level to higher level, and the relative ease of formalizing lower levels of abstraction
The planning process and the way that we treat near concrete events at a low level and far events at a high level
Holistic reasoning (broad, System 1) vs. sequential (Analytic, causal, System 2) reasoning
Causal models, and the way we chain through reasoning up chain of abstraction
Contrast causal inference with intuitive, probabilistic inference over some high dimensional ‘feeling about’ or ‘sense of’. Transfer between these types of domains is very different, as is the way we reason about the role of abstraction in them.
Abstraction and generalization - generalization as a way to evaluate abstraction quality
The discrete quality of abstraction, and the problems that result
At a high enough level questions start to encompass values, which are not objective, and people often don’t notice when their question is so abstract that it involves values that are arbitrary and the q has become subjective
The way that information is lost up the chain of abstraction. Coarseness and fineness. Fundamental tradeoff between amount of compute necessary and the accuracy of the abstractions reasoned over.
Abstraction and variance - because information is in variance, the high variance (not necessarily representative) portions of an abstraction may take over the conception of a system or a set of people. Contrast between variance as information and true probability distributions. 
Abstraction as compression. And compression as basically everything.
When faced with a bad abstraction, people pick sides on how to think about the bad abstraction instead of going a level lower and in so doing immediately resolving all disagreement. (in the case of Islam, religion (which implies false equivalence between islam and christianity which doesn’t capture the differences in secularization, enlightenment, empire (caliphate) building and sharia)
Empiricism at different levels of abstraction -
Language as a proxy for thought, and the way the the link of abstraction between thought and language shapes the way we experience ideas and communication.
Inferential distance, where ideas build on each other and the lack of foundation makes it impossible to move forward with a particular idea.
Overview of the fundamentally related big ideas - composition, hierarchy, transfer, causality, structure, compression, math, cognitive biases, information availability, memory, attention
The construction of mathematics as an explicit capture of abstraction models - also, analogies between mathematics and other abstraction processes (NB, this is fundamentally doing mathematics, but philosophy aside…)
Models - Mental models, predictive models, causal models - any map of a territory - as an act of abstraction
Need for Abstraction in formal systems - defining something like a utility (Econ), an environment (RL), etc.
Distinction between objects and relationships - graphical / relational frame, differences in abstraction necessary to account for this
Clustering (or feature group clustering) as abstraction
Temporal Abstraction
As necessary for causal inference
Alien philosophy - Can never do similarity without the generative process
Operate without operating - doing transfer / rerepresenting one as another does this
Intelligence Relevant Topics
Having a model
Abstract Knowledge Representation
Ability to Generalize
Learning / Adaptive
Creativity
Information processing
Computation
Goal accomplishment (ugh)
Generality (over environments, tasks, representations)
Memory (Working, Episodic, Long Term)
Attention (though this feels like a limitation)
To turn into general versions:
Sensitivity score (maml based).
Re-framed for abstraction: think of representation sensitifity as a way to do transfer. By finding the representation that is most adaptable (say, you have a body of recombinable primatives that effectively capture a decomposed representation of whatever your target is) it’s easier to quickly learn to deal with something unique. There are properties of representations that make this easier or harder. In many ways, overfitting looks like representing the world in a way that makes information about particular tasks difficult to reuse for other tasks. You can see episodic memory systems as enabling very fast learning and fitting, but also as representing informaiton in a way that will be more difficult to generalize.
Do close analysis of how the representation represents a single image.
Credit assignment over particular filters.
Look at the way the filters are recombined with one another - find simple examples of composition that models a particular part of the image.
It’s useful to know which sub-parts of a representation are involved (say, causally) in making a prediction. If you can do that credit assignment, you can know which parts of the represenation aren’t worth keeping (say, if you have constraints on total memory) where ex. The avaliability heuristic pushes parts of the potential representation to spaces that are less accessible to attention the more time that has passed since those circuits have been activated. 
It can also be made clear where the representation can / should be made richer. Say you’re using a part of the representation that hasn’t been self reflected on deeply over and over and over again. When you decide to thicken the quality of the representation, those parts will be the low hanging fruit, the best place to start.
Some filters will be composed with more or less other filters, which is a different metric than their importance. Which filters activate over the most images? At each level of the network?
Can we use this metric of generality as a heuristic for transfer? Say, only filters that are sufficiently general get used in transfer?
You want to see which parts of your representation get their value directly vs. getting their value through recombination with other parts of the representation. The parts that underperform in recombination may need to be made more modular or interacted with at a lower level of analysis as a standard step in improving the quality of the representation.
Find ‘conflation’ in a representation. (this may be hard)
Have a notion of which features should be recombined to create a higher level feature
Look for overlapping activations where they should not exist (misclassified examples should be really good for this)
Get to a ‘why’ for misclassified examples
Look at the ways that the representation couldn’t distinguish between particular parts of an input, look at the mistakes made over 4-5 examples and diagnose them
Are you allowed to publish a paper titled ‘why our networks fail?’
This may be hard to get causal on, but could be extremely useful.
It’s important to be able to introspect on the thinking that led to a particular decision so that the appropriate part of it can be updated (credit assignment style). In the absence of that, the entire mode of thinking or body of interconnected thoughts needs to take the update. 
Do VQ-VAE, but with a forward predictive model. Generative model of future, rather than present. Auto-regressive generative model.
I guess this is what the forward predictive lstm over VAE state is, in a way.
Take Ben Poole’s Gaussian Mixture Model VQ-VAE and apply it to something like world models (where you want this ability to go discrete or continuous)
Is this idea for generative future prediction a thing in general? VAE + LSTM to do it is awesome, but is it the best in its class for that task?
Check manifold learning hypothesis
Dog manifold on animal manifold, for example
Causal representation learning - which filtermaps have counterfactual impact on the output?
Use filter-level dropout to estimate this
Metric Learning is beautiful because similarity is foundational to compression, abstraction, and generalization, and the kinds of similarity that your representation exposes is a critical property of your representation. It’s an attempt to answer the question of what the most relevant axes for comparison are. The concepts that are necessary are the ones that look at similarity along one or a handful of features, not all of them, which abstractions or concepts can be seen as a multitude of learned similarity metrics across different subsets of features of the data.

Potential Interactions: 
Properties of Thought & Information Processing

Uncategorized:
Transfer
Creativity
Feedback
Positive Feedback
Negative Feedback
Applicability (getting to the right level of abstraction)
Generalization Error
Extrapolation
Interpolation
Observation
Regularity
Prediction / Inference
Validation
Common Sense
Logic
Induction
Deduction
Tradeoffs
Arbitrage (Between two models)
Exploration - Exploitation
Smoothness
Manifolds
Sparsity


Biases
Selection Bias
Measurement Error
Latent Variables (in a causal context)
Autocorrelation
Distribution Error
False Assumption

Structure / Reframes
Graphical / Relational Structure
Hierarchical Structure
Temporal Structure
Positive / Negative Feedback
Recursive Structure
Discreteness / Continuity
Causal Structure
Combinatorial Structure

Tools:
Distributions
Gaussian Distribution
Pareto / Power Law Distribution 
First Principles
Invert - Reverses the impact of a card
Counterfactual
Elucidate Assumptions

Increase Bias, Lower Variance
Abstraction
Compression
Dimensionality Reduction
Regularization
Linearity
Discreteness
Binary / Multinomial

Increase Variance, Lower Bias
Continuity
Nonlinearity
Conditional / Distinction
Nuance?

Resources
Working Memory
Long-Term Memory
Attention
Processing Speed

Attributes
Creativity?
Curiosity / Intrinsic reward for compression progress
Education

Outcomes
Interestingness
Novelty
Feeling of Compressing model
Originality / Uniqueness
Interpretability


Citations
(As well as links to as many things I’ve read in writing this as possible)
Concepts - Stanford Encyclopedia
Abstraction - Wikipedia

Reading List
Philosophy
Concepts - Stanford Encyclopedia
Abstract Objects - Stanford Encyclopedia
Abstraction - Wikipedia
Books
Fluid Concepts and Creative Analogies [Hofstadter]
The Philosophy of Information [Floridi]
Philosophers
Plato (Forms)
A Human’s Guide to Words (LW Sequence)
Cognitive Science
Knowledge, Concepts and Categories [Lamberts]
They wrote me down
Knowledge Representation [Markman]
Cognition and Categorization [Rosch]
Categories and Concepts [Smith]
The Big Book of Concepts [Murphy]
The Origin of Concepts [Carey]
Concepts [Margolis]
Machine Learning & Artificial Intelligence
Bengio, Courville, Vincent (2014)
Building Machines that Learn and Think Like People
Generality in Artificial Intelligence
SCAN: Learning Abstract Hierarchical Compositional Visual Concepts
Driven by Compression Progress
Universal Intelligence: A Definition of Machine Intelligence
Concepts, Ontologies, and Knowledge Representation [Jakus]
A Survey on Metric Learning for Feature Vectors and Structured Data (Learned Similarity)
Learning a Similarity Metric
Linguistics
Computer Science
Simple Made Easy
The Complexity Trap
Can Programming Be Liberated from the Von Neumann style?
Uncategorized
Old Draft
Old Draft Table of Contents
What is Abstraction?
Introduction
How to Think About Abstraction
Hierarchical Compression
Shared properties of compression
Shared Structure
Similarity
Pure abstractions, CS & Mathematics
Which properties transfer across these definitions through examples
Map / Territory
Where people have seen abstraction / how it’s talked about
Types of Abstraction
Examples
Base unit - lowest level for composition
Consistency - whether the type of object is the same down to the base unit
Discreteness vs Continuous
Comprehensive (covers entire space) vs. cleaner generalization
Power
Transfer & Generalization
Metaphor as tacit abstraction
Causal vs. Intuitive vs. Probabilistic vs. Structural Transfer
Importance of appropriate level of abstraction
Tractability with reality
Representation heights as powerful
Hierarchical Structure
Memory, Computation
Multiple levels of abstraction
Moving between levels of abstraction
Abstracting away reality
Creativity
Creativity as transfer
Creativity as recombination of representations
Creativity as deconstruction
Pitfalls
Unlike Object & False Transfer
Memetics
Excessive Height
Abstraction as an unseen assumption
Reductionism
Lack of grounding to abstractions
Social reality
Conflation
Construction & Deconstruction
Processes that create abstractions
Intuitive
Intentional
Engineering abstractions for outcomes
Using Abstraction
Improving abstractions
Feedback
Consistency
Groundedness
Noticing breakdowns
Overly coarse
Optimal Reactions
Overly fine
Optimal reactions
Seeing the level of abstraction being used
Choosing the level of abstraction to use
Frame
Future
Machine Intelligence & Representation
Future of academic fields damned by the consequences of dirty abstractions
Conceptual past and future


Thoughts list
Category errors as failure in abstraction type
Business leaders as using high level abstractions over low level behavior
Constant question is where / if their abstractions break or become ungrounded



What is Abstraction?

Introduction

Idea List
Nice anecdote / grounding
Motivation
power of height & representation, 
transfer, generalization, 
problem solving, 
working memory,
creativity, 
interestingness and intellectual beauty, 
deconstructing disagreement & confusion,
structure of reality
Lines -
Abstraction as synonymous with evasiveness, a lack of clarity
Abstraction as about untamed power

How to Think About Abstraction - Abstraction as an Abstraction

Idea List
Overview Hierarchical, shared structure, purity, transfer

As a term that unifies shared structure, abstraction sits above a number of critical compressive forces that underlie thought. 

Shared structure means that when looking at a set of objects, you’ll invariably find some objects that have similarities to one another. Those objects are ‘closer’ to one another, and sometimes they’re close enough that it makes sense to summarize their closeness (and reduce the number of objects that you need to keep in mind) by giving them a shared name.

Shared structure can be thought of as a simple form of hierarchical compression, in the case where there’s only one lower level layer and a single higher level concept. But that’s rarely where things end - as soon as you have abstracted, you’re looking at a new object. And yet more compressive power can be found in abstracting recursively, generating another layer and adding depth the the hierarchy. 
That said, there are other forms of hierarchical compression that distinguish it from shared structure. Often, unlike objects will be composed into a cohesive and coherent higher level object, and so we’ll abstract over unlike objects that work together in a way that makes it efficient to compress them, often in terms of their function. A laptop is a great example of this. It brings together wiring, a compute chip, memory, tools for interaction like your keypad and mouse, a glass screen, and more. We abstract over all of this, calling the object a laptop. This compression is important so that the level at which we interact with the object is simple and consistent with the tools being used to do the interaction - moving the object from place to place in a bag, buying or selling the object, or clarifying its presence or absence.

There’s a purity that comes out of abstracting in a way that doesn’t dirty things up. It’s hard to come by that purity in the world (say, when abstracting over things like shapes, objects, or emotions) but it happens all the time in mathematics or computer science. Mathematical functions as the abstraction of an operation, say - we take many instances of addition and abstract it into a function that operates over any data. That abstraction is pure in that it’s clear what the shared structure is between instances of addition, and it transfers cleanly (all of the properties are maintained) to a new setting. This purity comes out of the limitedness of the abstraction, as well as doing it in an abstract context (math) rather than in reality, where something like adding groups of animal together may be done heuristically and imperfectly rather than mathematically - especially for groups that haven’t developed a number system.

Across these definitions of abstraction, there are properties of abstraction hold like compression and informational power (due to height allowing one to operate over many more objects). But other properties break down - the abstraction over unlike objects that perform a unified task gives the user of the abstraction a new and improved level at which to interact with reality. But it’s not pure in the way that a type system in computer science is pure, where you abstract over the bit representation of integers, or characters, and so are confident that you can operate over every instance of that abstraction in an identical way. 

Hierarchical Compression
Idea List
Compositionality 
Curse of dimensionality
Width-wise and depth-wise compositionality
Recursivity
Unifying lower level structure vs. breaking down higher level structure
Read Bengio on hierarchical compression

There’s amazing power to hierarchy, in that it can introduce relatively complex models that tame an extremely high dimensional and complex world. 

A classic example of hierarchical compression comes from vision, where it’s used to create state of the art computer vision systems. Images at a low level can be filtered for lines and curves - in a cat’s mind (and likely ours) the the visual system lights up in the presence of edges in a way that doesn’t happen for other extremely low level shapes.
Those edges and curves can be re-composed into shapes. And those shapes are composed into parts of objects, which can be composed again into higher level objects.
These all expose grains at which to interact with reality. 

That’s an example of bottom up hierarchical compression, but we’re also familiar with going top down - being introduced to a high level concept (say, in the form of language) and over time needing to fill in the details. 



Shared Structure
Similarity

Cognitive Fit
Distance Metrics (As examples of different types of similarity)
Edit Distance vs. Euclidian Distance vs. Geometric Distance vs. Angles vs. Shape vs. Color vs. KL Divergence, etc.

Pure Abstractions
Transfer, Across Definitions
Idea List
Idea list this!
Compression transfers	
Operating recursively sometimes transfers


Shared Structure
Pure abstractions, CS & Mathematics
Which properties transfer across these definitions through examples
Map / Territory


Transfer of properties of abstraction across definitions

Definitions - is-a relationships (math, object oriented) vs. hierarchical compression (in my mind just unidirectional, but what we care about is shared properties). Abstraction necessarily virtual? How virtual, do we execute it to be consistent with the data generating process and so map cleanly to the territory, or is a map clearly apart from the territory that we don’t expect to adhere to things perfectly? Different expectations of abstraction in math/physics/cs vs the dirty version everywhere else.

Shared between math / physics / cs abstraction (is-a relationship, purity, consistency with territory, always recursively executable)
Hierarchical Compression

Both involve:
Compression
Level of analysis at which to interact
Though math / physics / cs will throw category errors if you try to interact at the wrong level of analysis
Heights of abstraction operate over more information
Leakiness
A problem in (and defined by) CS APIs. APIs as an abstraction over implementations. 
Though perhaps worse in hierarchical compression, where there’s so much more behind the abstractions. 




Distinctions:
Transfer and generalization
Math / object oriented cs (not machine learning!) / physics have very narrow and precise rules around transfer and generalization. And they throw category errors when those rules are unmet.
Hierarchical compression works in looser ways in a statistical sense. You can generate a representation of a concept and use it in extremely refined or less refined ways, to better or worse results.
Base units
Consistently build up compositionally from base units in math / physics / cs. Not true elsewhere - can start at an intermediate or high level and go down, or start low and go up. Reductionism is much less effective elsewhere. You can’t transfer reductionism across domains, because the systems aren’t constructed (or physics) and so you don’t know what all of the ways to abstract down are.
Discreteness vs. Continuity
Usually discrete in language and in math / physics / cs, continuous in machine learning / in our minds. There’s a fuzziness that lets us do cross-domain ‘cognitive fit’.
Dirtiness
Math / physics / cs is extremely clean (even pure), elsewhere people are happy to recombine distributed representations of concepts
Limited vs. Defined and Loose
Extremely limited in math / physics / cs. Category errors, discretely represented.
Groundedness
Often ungrounded in hierarchical compression space, you don’t even really need to know the low level.
Can be ungrounded in physics (say, before we knew about atoms), but very grounded in math (bottom-up construction from axioms) and in object oriented programming (regardless of the true data being modeled, the cs representation is grounded in bits)
Mental modeling as abstraction often doesn’t expect to conform to the territory. Math / CS / Physics try to create abstractions that correspond very closely to the territory, and to the process that generated the data being modeled.

Types of Abstraction

Examples
Base Unit

Base Units show up to ground abstractions in physics (often atoms), mathematics (axioms) and computer science (bits). There will be abstractions built over these base units (say, molecules, theorems & functions, or types) and the system will follow hierarchically through composition of base units. These systems have strong ties to causal structure, where outcomes are the result of sequential operations over lower level units.

There’s another representation that’s much less grounded that we can use for comparison - ensemble modeling. Rather than mapping out a space from first principles, generate a set of representations that seems to break the space up (much like we’re doing here, breaking abstractions into types to compare their properties)

Consistency

There are different types of abstraction that show up in conceptual abstraction space. Types can either be mixed with one another, or done with consistency. [Add motivation]

For example, take a big organization. We can break it into a sales division, and an engineering division, and a marketing division, etc. The type of abstraction that this is a function of what the parts of the company do for the company.

Say now that you want to measure the extraversion of these groups. This involves a different type of abstraction, down to the individual people in each group, and then a function (measure of extroversion, with an average) over the set of individual people.

We’re mixing:
Function done in the company
Set of People in group

And could have continued going to function at a lower level (say sales is divided into sales managers, sales call persons, lead generation people). And for some operations, like management structure, this is the appropriate way to deconstruct the space.

This works cleanly because the sets that underlie the abstractions are cleanly separated from one another. 




Discreteness vs. Continuity

Terms, How People Talk about Abstraction

High Level vs. Low Level
Grain (Coarse Grain vs. Fine Grain)
Broad vs. Specific
General vs. Specific
“Broad brush”
Concepts, Conceptualization (Boyd, Dad)
Comprehensive Whole vs. Particulars (Boyd)

High Level vs. Low Level

There’s the ubiquitous reference dependent ‘high level’ and ‘low level’ type or reference, where the speaker has in mind some reference class level (often contrasting the high using the low as a reference point, and using the high as a reference point to define the low). 

This tends to lead to unnecessarily binarized thinking. Ideally the language would auto-capture that there may be a high level and a low level, but there’s also a level higher than low level but lower than high level, and lower than low level, and higher than high level, etc. The use of almost all of these terms relegates us to two levels by default. Though maybe that makes thining easier for the reader. And also, perhaps it’s not binary but points to a ‘gradient’. More true for coarseness vs. fineness than high vs. low.


Coarseness vs. Fineness (Literally true in the case of abstraction in image processing)
Grain (Coarse Grain vs. Fine Grain)

I really enjoy how this version implies a continuum of abstraction - it’s clear that you can become incrementally more coarse, or incrementally more fine. And so it’s appropriate for those situations where the abstraction is continuous. It’s also flexible, and can be used for discrete situations that are more or less fine / coarse than one another. 
But it struggles in another context, where there’s strong discreteness. Take the version of abstraction involved in creating a function, or in creating a variable instead of using scalar values. The metaphor (coarse vs. fine) starts to break down. 
This is in part because coarseness vs. fineness assumes that the type of abstraction is exaclty the same throughout! In the metaphor, you only get more or less resolution. You never switch to a different type of abstraction. And it’s hard to model a binary discrete situation with this, where there are exactly two levels. May be nicer if there are more levels, but we also have to keep the type of abstraction the same.


Broad vs. Specific
General vs. Specific
“Broad brush”

“If you ask a more specific question, I can give you an answer.”, is what Scott Kominers would love to tell me.  People love to use the term ‘broad brush’ to give themselves permission to not condition on subsets of populations, or to make general claims in a way that’s unrigorous. It’s both valuable and dangerous - dangerous in that they don’t expect to go into details on their claim, which makes these kinds of claim extremely hard to evaluate, verify or argue against. Or often arguing against consists of picking a counterexample, which the person admitted would exist when they said that the statement would be broad brush. It’s valuable in that these summaries across populations end up being critical for decisions that depend on the proclivities of a large number of people. And it becomes extremely difficult to reason about a space if the level or rigor required makes it hard for people to make claims that look true to them. 

Concepts, Conceptualization (Boyd, Dad)
Comprehensive Whole vs. Particulars (Boyd)
General-to-specific (Boyd)



Power

Transfer and Generalization

Idea List
What transfer is, implications for generalization (non-local / out-of-domain transfer)
Generalization accuracy as a standard for abstraction quality
Metaphor as tacit abstraction
Causal vs. Intuitive vs. Probabilistic vs. Structural Transfer
Importance of appropriate level of abstraction
Tractability with reality



Transfer & Generalization
Metaphor as tacit abstraction
Causal vs. Intuitive vs. Probabilistic vs. Structural Transfer
Importance of appropriate level of abstraction
Tractability with reality


Transferring learned knowledge across domains requires abstraction, explicitly or implicitly. The abstractions are the shared structure within domains that allow the knowledge gained from one domain to transfer to another.

What is transfer?

Great examples of this are planning, pattern recognition (transfer between datapoints)

In planning, there’s a hierarchy of tasks over which you can do transfer. Say you need to save someone just hit by a car by getting them to the hospital.

At a high level, there’s a transportation problem. It can be instantiated in a few ways - ambulance, car-transport, etc. Ambulance breaks down into calling 911, identifying your current location (orienting to the street signs), communicating with the emergency operator, etc. Those are composed of lower level actions which often disappear beneath conscious awareness, say taking out a phone, opening the interface, opening the phone app, pressing the keys, putting it to your head, etc. This process is modular and transfers across domains. Regardless of who you’re calling, when you’re calling, the motions are the same. And so you think in terms of the abstracted motion (call this person / number). 

What is generalization?

The critical property of an abstraction is its ability to generalize. 

Within a domain, learning often looks like generalization - in sports, you pattern match one situation to similar past situations, and react instinctively in a way that your intuition hopes will lead to success. In mathematics, solving a problem with an algebraic manipulation once lets you recognize that type of manipulation in other situations. And often so you abstract the manipulation into a rule or into an operation that you can run more flexibly.

But you’d also like to do out of domain generalization - learn something in one context and apply it to an entirely different context. Learning language in one domain (say, in a home) and then applying it at school, or with friends rather than parents, or in speeches. Take the concept of specialization and lift it from economics to understanding sexual dimorphism in evolution. Taking the concepts of a replicator and differential selection from evolution and apply it to ideas and tunes and fashions that replicate by imitation.

Generalization as a Standard

Generalization accuracy is a great standard to hold abstractions to. What we want is for our representations to aid us in problem solving, which often takes the form of prediction what the impact of our actions will be or predicting what the state of our system will be in future.

When adjudicating between representations and when constructing them, we’ll optimize for the representation that is easy to evaluate (simplicity heuristic) and that makes the most accurate predictions. And simplicity is also a part of accuracy - models that are simpler have the advantages of capturing more data (because in general they’re more abstract), being more robust to small differences between observations and so better able to capture the higher level regularity, and being straightforward to update when they’re mistaken.

Implicit Transfer

Metaphors are examples of transfer that at first look to be free of abstraction, but as they’re drawing their power from shared structure between the domains we can use them as using abstraction implicitly.

One result is that metaphors are a source of explicit abstractions so that representations and solutions can be extended to their farthest reaches.
Often the emphasis is on emotional transfer, and so the metaphor communicates more than pure information. But that transfer matters too - communication is extremely high dimensional, and the felt dimensions are more important for compelling action and building understanding than pure understanding. More on this in engineering abstractions.

Take a classic christian verse, “we are the clay, you are our potter”. There’s implicit abstraction around agency vs. the acted upon, intentionality, moldability, and craftsmanship, as well as the load of connotations that go along with the profession and the nature of the objects.

Giving examples as grounding to abstraction is common practice. Often more than one example is required to pull generalization off properly, as there will be details for particular examples that don’t necessarily generalize and transfer that can be omitted from a second or third example.

Glorious Heights of Representation

There’s power to the heights of abstraction. As the height grows, the number of objects being acted over grows. There are a huge number of nodes in a belief structure, and the impact of information grows as it becomes relevant to every node in that structure.

Say you learn something about capitalism. All of a sudden your model of every single transaction that has occurred across time, and the implications of those transactions updates. There’s power here insofar as one can take a new concept and notice the breadth of implications that come with it.

The way to generate power from lower level information is by abstracting. Say you notice that when someone takes a lower-paying job they don’t have as much time to apply and interview for higher paying jobs. This is a nice insight which may help you make that tradeoff more effectively in your life, by being aware of it. But the power comes out of abstracting this concept to opportunity cost, and realizing what the implications of opportunity cost are for the application of every finite resource (time, attention, energy, money). Even resource in that previous sentence is an abstraction over a world of objects that often need to be explicated if the impact of an update to that abstraction are going to be understood, experienced and lead to a better planning process.


Pitfalls

Transfer and Generalization

Overfitting / Bias-Variance Tradeoff
Grab not enough datapoints, create a complex model and assume that it will transfer cross-domain
As the level of abstraction rises, there’s more data to be seen and so it’s easier to create a biased sample accidentally
Large data also allows you to more accurately validate the abstraction
Magic numbers… everything feels overfit
Each Abstraction has to trade generality for nuance
Without complexity (conditionals, context dependence, additional features / factors)
Forming an abstraction in a way such that it fails to transfer
Ex., Statistics / Probability Theory
Wrong level of analysis to see across many tasks




Information Loss

Information lost in classification, or as we move up levels of abstraction
Ex, so much more information in a particular dog (its color, its personality, its sound) than in the category of dog in general.
Information lost in binning
Major pitfall is to have lost so much information that the representation isn’t predictive of important outcomes anymore
Computational difficulties in maintaining information
If you abstract over every property of the underlying object and hold the intersection of all of those abstractions, you may be able to keep the same amount of information. But now your model is a different type of complex.

Conflation, Unlike Objects & False Transfer

Labeling a group by abstracting over objects that share one property but not others creates conflation between the unlike properties
Properties shared among some but not all group members get generalized to being a property of the group
When two objects share a property, a metaphor can be made between them. But the metaphor breaks down over some properties and not others. And so recognizing the limitations of transfer is a process in and of itself, that can fail and lead to erroneous generalization.
Classic example is a metaphor to a positively connoted thing, to compliment or make something good. Or a metaphor to a negatively connoted thing.
Russell conjugates in description (making the metaphor’s implicit abstraction concrete) are also good examples of the manipulability of transfer.

Excessive Height

Height obscures underlying content, making grounding more difficult
Greater height exposes more datapoints, making it easier to tell a story for any thesis
Height demands more rigorous statistical claims
Positive example generation is the default mode in making arguments / thinking about theses, and is much easier at height
‘Category error’ problems start to get bad…
What is a category error? It implies logic, or fit, or rules / constraints around objects… There’s this question 
Ex., adding unlike units together, adding pressure to height
Not all category errors made equal. Adding a height to a volume is understandable… it can give you an approximation of another volume. 
At a higher level of analysis, adding ‘space’ to ‘space’ seems fine… And so abstraction can fuzz the details.
Often there are multiple representations, at different levels of fuzz, and you pick the one that allows it to make sense…
Sympathetic view - Structure is preserved among unlike objects
Sometimes, adding height to volume gives you stronger predictive validity
Unsympathetic view - The heights of abstraction obscure the category errors that would be clear at a lower level
With height, more category errors occur - breakdowns in the fit between objects at lower levels of analysis.


Abstraction as an Unseen Assumption
Lack of Grounding

Remembering the model, forgetting the data
Generalization from few (1) datapoint
Lack of depth means it’s difficult to expose failed transfer



Unlike Object & False Transfer
Memetics
Excessive Height
Abstraction as an unseen assumption
Reductionism
Lack of grounding to abstractions
Social reality
Conflation

