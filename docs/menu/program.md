---
layout: page
title: Program
permalink: /program
---

* Introduction (15 min)
* Part 1: Sparse and Structured Transformations (45 min)
  - Sparse transformations: ReLU, sparsemax, Ω-argmax
  - Sparse attention and adaptively sparse transformers
  - Structured and sparse differentiable layers
  - Sparse associative memories and ∞-former
  - Mixed discrete/continuous latent models: Hard Concrete, Gaussian-Sparsemax
  - Learning sparse policies in RL and future directions
* Part 2: Sparse Architecures and Representations in Foundation Models (45 min)
  - Sparse Mixtures of Experts: from LSTM MoEs to Mixtral
  - Conditional computation and early exit: Mixture of Depths
  - Sparse memories: Cache Eviction Policies, Dynamic Memory Compression
  - Modular deep learning and sparse mixtures of adapters
* Q&A (15 min) 
* Panel with Sara Hooker and Alessandro Sordoni (30 min)

<h1>Panellists</h1>
<ul>
  {% for author in site.panellists %}
    <h2><a href="{{ author.website }}">{{ author.name }}</a></h2>
        <h3>{{ author.position }}</h3>
    <li style="display: flex; align-items: flex-start; margin-bottom: 20px;">
      <div style="margin-right: 20px;">
        <img src="assets/img/{{ author.image }}" alt="{{ author.name }}" style="width: 2500px; height: 300px; object-fit: cover;">
      </div>
      <div>
        <p>{{ author.content | markdownify }}</p>
      </div>
    </li>
  {% endfor %}
</ul>