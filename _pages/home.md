---
title: "Home"
layout: homelay
sitemap: false
permalink: /
---

<div style="height: 25px;"></div>

Hi, and welcome to my homepage! I am a Ph.D. student at the University of Illinois Urbana-Champaign. I am advised by [Matthew West](http://lagrange.mechse.illinois.edu/), and broadly speaking, I work on optimizing PDE solvers using machine learning. In particular, I have used techniques such as unsupervised and reinforcement learning (RL), along with graph neural networks (GNN), to optimize numerical PDE solvers.

<div style="height: 5px;"></div>

In a study published at [NeurIPS 2021](https://neurips.cc/virtual/2021/poster/25928), I utilized RL and GNN to optimize coarse grid selecetion in algebraic multigrid (AMG, a famous numerical PDE solver), with theoritical guarantees for convergence of the obtained method. Feel free to check out the paper [here](https://openreview.net/pdf?id=xXYjxli-2i). 

In another study published at [NeurIPS 2022](https://neurips.cc/virtual/2022/poster/53135), I utilized unsupervised learning and GNN to learn and optimize domain decomposition PDE solvers (DDMs). The unsupervised loss funciton introduced in this study provides theoritical guarantee to converge to the global optimum in limits. Feel free to check out the paper [here](https://openreview.net/pdf?id=FvdOlVWL-w).


<div class="container">
<div class="row">
<center>
<img src="{{ site.url }}{{ site.baseurl }}/images/mggnn.jpg" width="100%"/><br/>
Hierarchy of grids obtained from a PDE passing through GNNs. <br/>
</center>

<div style="height: 15px;"></div>

I have recently been working on a follow up study on learning domain decomposition solvers, and have developed a new GNN architecture to learn to optimize multilevel DDMs. I have also improved the unsupervised loss function to adapt to multilevel training scheme, wich also enjoys theoritical guarantee to converge to the global optimum in limits. Feel free to check out the preprint [here]().

</div>
</div>
<br/>

<!-- <div class="row" style="text-align:center">
  <iframe style="display:inline-block; border-radius: 5px; border:0px solid #FFF; width: 95%; height: 246px" src="https://www.youtube.com/embed/W2VWLYnTYrM?playlist=W2VWLYnTYrM&loop=1&autoplay=1&mute=1" frameborder="0" allowfullscreen></iframe>

  Demo of [coupled simulator](https://github.com/bazilinskyy/coupled-sim) with 3 agents in the same traffic scene.
</div>
 -->
