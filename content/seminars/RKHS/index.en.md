---
weight: 4
title: "Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space"
date: 2024-05-02T09:40:28+08:00
draft: false
author: "Yiping"
description: "This article introduce Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space."
resources:
- name: "featured-image"
  src: "featured-image.png"

tags: ["Statistics", "Kernel"]

lightgallery: true
---

This article introduces Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space.

## Reproducing Kernel Banach Space

{{< admonition note "Definition" >}}
:(far fa-bookmark fa-fw): A reproducing kernel Banach space \\( B \\) on a prescribed nonempty set \\( X \\) is a Banach space of certain functions on \\( X \\) such that every point evaluation functional \\( \delta_x \\), \\( x \in X \\) on \\( B \\) is continuous, that is, there exists a positive constant \\( C_x \\) such that
\\[ \left| \delta_x(f) \right| = \left| f(x) \right| \leq C_x \| f \|_B \text{ for all } f \in B. \\]
{{< /admonition >}}


Note that in all Representer Kernel Banach Space \\( B \\) on \\( X \\) norm-convergence implies pointwise convergence, that is, if \\( (f_n) \subset B  \\) is a sequence converging to some \\( f \in  B  \\) in the sense of \\( \|f_n - f\|_{B} \rightarrow 0 \\), then \\( f_n(x) \rightarrow f(x) \\) for all \\( x \in X \\).

### Construction of Reproducing Kernel Banach Space

{{< admonition note "Construction" >}}
 For a Banach space $W$, let $\[\cdot,\cdot\]$  be its duality pairing which is a bi-linear maps from $W\times W'$ to real number. Suppose there exist an nonempty set \\( X \\) and a corresponding feature mappings $\Phi : X \rightarrow W',$.  We can  construct a Reproducing Kernel Banach Space as 
 \\[B := \\{ f_v(x) :=[\phi(x),v] : v \in W, x \in X \\} \\]
 
with norm \\(\|{f_v}\|_B := \text{inf} \\{\|v\|_W: v\in W\ \text{ with }\ f=[ \Phi(\cdot), v ]\\}.\\)
{{< /admonition >}}



### Examples of RKBS

#### Neural Networks
