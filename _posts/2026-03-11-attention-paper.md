---
layout: default
title: "Finally paying attention"
tags: [ "computing" ]
---

I finally got around to reading the "Attention Is All You Need" paper by Vaswani et al.
 I had tried reading it before but in each attempt I would stop at Section 3.2.1 and would hence end up at the beginning (1).

I will avoid explaining the content or discussing the paper in detail, since there are N pages on it. This blog is mostly my journal of what I derived from the paper.

This time around, I generally followed a very blind-eye approach. I went in without any thoughts of whether I know the pre-requisites, background or if I will derive some benefits from reading it. A small disclaimer: My main interests are in Networks/Network Systems hence ML is more of me peeking at the advancements of current technology.

So to start, for me the entire idea was a direct analogy to smart bruteforcing. We have an 'attention' subroutine (going by the scaled dot-product attention) that compares every element with every other element where nothing is pruned or left out, and from these comparisons derives a sense of importance for each element's representation through the resulting weights.

However, attention alone operates in a single representational view. To allow the model to learn from multiple perspectives simultaneously, we use multi-head attention which performs linear projections of Q, K and V into multiple subspaces, each head attending in parallel. Each head can focus on different types of relationships, and the results are later combined into a unified global representation. 

To me this is very much like a task where we definitely need to compare with everyone else so bruteforce is inevitable but the smartness of weighing eventually clears out the foggy relationships and establishes which parts will dominate. There is no discrimination before the comparisons happen, but the resulting weights introduce the partiality that determines which relations dominate.

The rest of the paper then delves into further details on usage, speed and results and the why of self attention. A surprising lesson for me, however, was how attention can replace convolution and recurrence alone. It is strange to see attention itself but to think of it being solely the engine capable of defeating the older approaches is probably the deeper lesson for me.

Next up would be me reading the two State Space Model papers (by Gu et al. and Gu & Dao). I am slightly curious if the weights can be represented differently and what that might imply. Simple vectors are nice but beyond them?

Hope to see you next time!
