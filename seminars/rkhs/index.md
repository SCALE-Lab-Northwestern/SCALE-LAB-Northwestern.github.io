# Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space


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


---

### Examples of RKBS

#### Neural Networks

> Bartolucci, Francesca, et al. "Understanding neural networks with reproducing kernel Banach spaces." Applied and Computational Harmonic Analysis.
> 
> Bartolucci, Francesca, et al. "Neural reproducing kernel Banach spaces and representer theorems for deep networks." arXiv:2403.08750 .


#### \\(L_p\\)-Type RKBS

---

## Representer Theorem 

> Unser, Michael. "A unifying representer theorem for inverse problems and machine learning." Foundations of Computational Mathematics 2021.


---

## Reproducing Kernel Hilbert Space


### Eigendecay and effective rank


## Characterization of Reproducing Kernel Banach Space using Metric Entropy

