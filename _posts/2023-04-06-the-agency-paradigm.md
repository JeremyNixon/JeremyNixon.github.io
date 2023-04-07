---
layout: post
title:  "Agentic AI"
date:   2023-04-06
categories: thinking
---

Deep learning has changed a lot in 2 years. I’m writing this so that I can fully realize just how starkly different the agentic large language model paradigm is when compared with the old deep learning paradigm. I’d like to officially recognize several new subfields of machine learning research. So much old thinking needs to be updated, and we need to make these updates quickly.

I’m tempted to call this the Agency paradigm - it does feel clear, in comparison with the past paradigm, that this one will give rise to general learning systems that automate 90+% of the knowledge work economy. It is possible, though not inevitable, that this will happen very quickly - on the order of the next 2 years. It may take as long as 6-8 years to get to a reliability level that allows for full automation rather than mere augmentation of every knowledge work task.

The Agency Paradigm is replacing an old paradigm, which I represent with the [Machine Intelligence Research Frontier](https://docs.google.com/document/d/13fpaiiGrGq71ZZLh5cQc_CMpdltfPJfRC8774fwzfBc/edit).

Similar concepts: [Foundation](https://en.wikipedia.org/wiki/Foundation_models) [Models](https://arxiv.org/pdf/2108.07258.pdf).

The new paradigm:
- Chains
    - Planning
    - Agents
    - Self-Correction: Automatic Evaluation, Self-Awareness.
    - Tool Use
    - Composition: APIs & API Chaining
- Pre-Training [Base Models]
    - Transformers & Attention Mechanisms
    - Diffusion Models
    - Multi-Modality
- Post-pre-training
    - RLHF [Reinforcement Learning from Human Feedback]
    - Instruct Fine-Tuning
- Information Access
    - Context Length + Memory Implementations
    - Search: Data & Dataset Access & Choice, RAG [Retrieval Augmented Generation]
- Meta Software
    - Neural Program Synthesis
    - Prompting: Prompt Generation & Automated Prompting, Meta-Prompt


Chaining - taking sequences of actions in the face of a single request from the user of an ML system - is newly possible because the reliability of single action is now high enough that the multiplicative interactions do not necessarily do undue damage to the final output. HIgh task reliability means that planning - both short and long term - becomes a task with merit. Creating plans that are achievable, reliable, self-correctable, and that fulfill the goal for which the plan is made is now a central problem in building AGI. Without it, the intelligent system will not have a clear view of the sequence of actions that are necessary for it to fulfill its mission. 

Agentic behavior exhibiting creativity, decisive action, identity, and decision making is possible in the face of foundation model improvements. Models are finally making the jump from tools to living beings, in the sense of their ability to replicate, have a survival drive, and maintain their goals across multiple experiences.

Self-awareness and environmental awareness allows for a transformation to the way that models act and behave. Self-correction, or evaluation of whether or not its performance fulfills the goal or requirements given, means that models can ‘think longer’, ‘work longer’, and compile actions or insights that fulfill much more complex tasks than they were previously given.

Learning to use tools is an essential part of completing important tasks in every human knowledge worker’s life. Communication is paramount in coordinating large-scale activity. Email, slack, text messaging, and other communication tools will clearly be essential to LLM agents looking to gather information from or send commands to other people. Getting the information required to make decisions, take actions that influence the environment, or answer questions often requires using search tools like web search systems or searching over private databases. Putting multiple machine learning techniques together - for example, speech to text for taking a command from a human user combined with text to speech to responding, allows for complex & integrated agents to achieve complex tasks with multiple types of output (messaging, code writing & execution, payments).

The composition of these techniques - of arbitrary ML APIs with tools with self-modifications with planning - will continually unlock unknown capabilities.



## Agency Literature Review
- Chains
    - Planning
    - [ReAct](https://www.google.com/url?q=https://arxiv.org/pdf/2210.03629.pdf&sa=D&source=editors&ust=1680834271934927&usg=AOvVaw3Ej_pdGoAg2yDVE9sWpIYB)
    - Prompting: Prompt Generation & Automated Prompting, Meta-Prompt
    - [PromptChainer](https://www.google.com/url?q=https://arxiv.org/pdf/2203.06566.pdf&sa=D&source=editors&ust=1680834271935263&usg=AOvVaw0zHk0DO5X74gTten07psJ8)
- Agents
    - [ReAct](https://www.google.com/url?q=https://arxiv.org/pdf/2210.03629.pdf&sa=D&source=editors&ust=1680834271935529&usg=AOvVaw3JpLCvoQjCT6JXLoLhVEBP)
- Self-Correction: Automatic Evaluation, Self-Awareness, Tool Use
    - [Toolformer](https://www.google.com/url?q=https://arxiv.org/abs/2302.04761&sa=D&source=editors&ust=1680834271935859&usg=AOvVaw1PlmsiEAClJtw-NvM3RjMN)
    - Essential Tools List
- Composition: APIs & API Chaining
- Pre-Training [Base Models]
    - Transformers & Attention Mechanisms
    - [BERT](https://www.google.com/url?q=https://arxiv.org/abs/1810.04805&sa=D&source=editors&ust=1680834271936334&usg=AOvVaw12LVYPXPZsF_7wUwu4C5Vg)
    - Diffusion Models
- Multi-Modality
- Post-pre-training
    - RLHF: [Deep RL from Human Preferences](https://www.google.com/url?q=https://arxiv.org/abs/1706.03741&sa=D&source=editors&ust=1680834271936749&usg=AOvVaw1zfuwiDsfVbYSX7MWGzJAs)
    - Instruct Fine-Tuning: [Training Language Models to Follow Instructions with Human Feedback](https://www.google.com/url?q=https://arxiv.org/abs/2203.02155&sa=D&source=editors&ust=1680834271937037&usg=AOvVaw0zkEF0Ou1CDAxWYxdi5QFz)
- Information Access
    - Context Length
        - [FlashAttention](https://www.google.com/url?q=https://arxiv.org/abs/2205.14135&sa=D&source=editors&ust=1680834271937350&usg=AOvVaw32F7NHErYB0bgrghTIatLl)
        - [Sparse Transformer](https://www.google.com/url?q=https://arxiv.org/abs/1904.10509&amp;sa=D&amp;source=editors&amp;ust=168083427193)
    - Memory Implementations
    - Search: Data & Dataset Access & Choice, RAG [Retrieval Augmented Generation]
    - Retrieval-Augmented Generation
- Meta Software
    - Neural Program Synthesis




