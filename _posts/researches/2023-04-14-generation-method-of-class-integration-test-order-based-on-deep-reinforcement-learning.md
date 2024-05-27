---
layout: post
title: "Generation Method of Class Integration Test Order Based on
Deep Reinforcement Learning"
author: Yinghui Zhang, Yanmei Zhang, Zhicheng Zhang, Shujuan Jiang, Yanru Ding, Guan Yuan
date: 2023-04-14 00:00:00 +0800
tags: [Research]
excerpt_separator: <!--excerpt-->
comments: true
excerpt: A papar has been accepted by Acta Electronica Sinica.
sticky: false
---
<!--excerpt-->
The generation of class integration test order is the key step in object-oriented software testing. When the class integration test order is different, the corresponding test cost is different. Generating a reasonable class integration test order in integration testing can effectively reduce the cost of software testing. This paper applies the advantage actor-critic algorithm in deep reinforcement learning to solve the problem of class integration test order generation. Firstly, the environment model of interaction with agents is constructed by using various dependencies between classes. Then, the path of the agent from the initial state to the termination state is recorded, that is, each selected action corresponds to each selected class number integrated into the order. Finally, the final class integration test order is obtained. The experimental results show that the total test stubs complexity of class integration test order cost obtained by the method in this paper has the best performance in 5 out of 7 selected subjects, and the average performance in the remaining 2 subjects.

<div style="text-align: center;">
    <p><img src="{{"assets\img\posts\2023-04-14-generation-method-of-class-integration-test-order-based-on-deep-reinforcement-learning.png" | relative_url}}" style="height: 20rem;"></p>
</div>