---
title: "Research"
draft: false

lightgallery: true

math:
  enable: true
---

At SCALE group, we have a diverse and continuously expanding scope of research interests spanning the theoretical and algorithm development aspects of  the new generation of AI powered research paradigm that integrates scientific and engineering knowledge into Machine learning and Generative AI. Our team is dedicated to research at the intersection of machine learning, non-parametric statistics, applied probability, and numerical analysis. Our primary focus lies in developing algorithmic and theoretical foundations for modern domains such as `Deep Learning`, `Generative AI`, and `AI4Science`.

![Research](./framework.png)

**Potential Topics:** Large Foundation Models for Science, Computational Complexity for Scientific Computing, Banach Space Geometry, Simulation Free (Diffusion) Models for Science, Trustworthy Machine Learning and Calibration

## Theory-Inspired and Physics-Informed Inference Time Scaling

In this project, we think of AI predictions as a trusted guide rather than the final decision-maker. Imagine planning a journey where your friend suggests a route based on experience, but you still double-check with a map. In our work, AI can offer useful hints or forecasts that help kick-start a more traditional method. These traditional techniques then take that initial insight and fine-tune it, leading to better and more reliable outcomes. Over time, as the AI's suggestions become more refined with extra data, they can further speed up the process, creating a helpful loop that improves overall accuracy without ever replacing the careful work of conventional methods. Furthermore, by integrating a chain-of-thought approach—where the AI's step-by-step reasoning informs each iteration—we can theoretically achieve faster convergence rates, and in some contexts, this acceleration is essential for reaching an optimal solution.

## Preconditioned Optimizer for Deep Learning

Recent advances in deep learning optimization have increasingly emphasized the role of preconditioning to accelerate convergence and improve training stability by leveraging second-order information. Early innovations like AdaGrad laid the groundwork by adapting learning rates on a per-parameter basis, while subsequent methods such as Shampoo extended these ideas to incorporate richer curvature approximations, leading to more robust optimization in high-dimensional spaces. The recent introduction of the Muon optimizer has further demonstrated the potential of advanced preconditioning techniques to harness second-order dynamics, significantly enhancing training efficiency. Despite these developments, the field still lacks a unified, principled framework to guide the design of such optimizers. Leveraging IEMS’s deep expertise in optimization and machine learning, we aim to establish new, rigorously grounded guidelines that will drive the next generation of deep learning optimization strategies.

## Scaling Law of LLM Agents and Scientific Machine Learning

How large the sample size and how much computational power are needed to reach a prescribed performance level for a physic problem? In machine learning, a neural scaling law (one of the secrete makes language model works) is a scaling law relating parameters of a family of neural networks. We are interested in how physics will affect the scaling law.

<div style="text-align: right;">
<a href="/posts/scalinglaw/">Read more <i class="fas fa-angle-double-right fa-fw"></i></a>
</div>

## Foundation of Machine Learning

Machine learning has achieved great success in many applications such as image recognition and language models. However, the reason why machine learning is so powerful remains elusive. One of the secrete behind this is machine learning provides powerful function/functional approximator in high dimension. Our group aims to understand the mysterious of machine learning using `functional analysis`, `high-dimensional statistics` and `high-dimensional probability`.


## Robust Machine Learning

Overparametraization, i.e, having more model parameters than necessary, is the core factor behind the success of modern machine learning. However, overparametraization also enables the model to fit any noisy signal which makes the model extremely vulnerable. Our research aims to build robust overparametrized model via understanding the inductive bias.

