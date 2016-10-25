---
layout: post
title: "We can't optimize what we can't measure"
date: 2016-10-25
---

Bohte and Gruning list three principles in their paper "Spiking Neural Networks:
 Principles and Challenges" to guide researchers how to make spiking neural network 
 communities better.

* Comparability.

* Generality.

* Formulation.

I think these three princeples can be generalized to various areas.

* Comparability. We need to compare different works in a reasonable way. So to 
 realize in which situation which solution works better. To acheive comparability,
  we also need measurability. With measuability, we give each solution a score, so
  we can compare these solution. Also, we cannot optimize solution if we cannot 
  measure solutions.

* Generality. I think a good area or algorithm or framework, should be general. 
 General solution has good flexibility and can be used in various situation with 
 proper modification. A good example is backpropagation algorithm in neural network.

* Formulation means that we should be able to extract clear rules or principles from 
  experiments. Although with comparability, we can work in a build solution->compare score 
  with other solution->optimize way. Good formulation helps us find the underlying valuable 
  part from good solutions and build better solution with a heuristic way.

It's hard to meet all these three principles. However, I think, with comparability we are in a 
right way. General framework or algorithm will come out soon or later. Then with enough good solutions,
 formulation can be figured out.

