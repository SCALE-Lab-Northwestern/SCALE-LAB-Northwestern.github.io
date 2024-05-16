# Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space


This article introduces Reproducing Kernel Hilbert Space and Reproducing Kernel Banach Space.

## Reproducing Kernel Banach Space

{{< admonition definition >}}
:(far fa-bookmark fa-fw): A reproducing kernel Banach space \( \BT \) on a prescribed nonempty set \( X \) is a Banach space of certain functions on \( X \) such that every point evaluation functional \( \delta_x \), \( x \in X \) on \( B \) is continuous, that is, there exists a positive constant \( C_x \) such that
\[ \left| \delta_x(f) \right| = \left| f(x) \right| \leq C_x \| f \|_\BT \text{ for all } f \in B. \]
{{< /admonition >}}


Note that in all Representer Kernel Banach Space \( \mathcal{B} \) on \( X \) norm-convergence implies pointwise convergence, that is, if \( (f_n) \subset \mathcal{B}  \) is a sequence converging to some \( f \in \mathcal{B}  \) in the sense of \( \|f_n - f\|_{\mathcal{B} } \rightarrow 0 \), then \( f_n(x) \rightarrow f(x) \) for all \( x \in X \).

### Construction of Reproducing Kernel Banach Space

{{< admonition tip >}}
 For a Banach space $\WT$, let $ [ \cdot, \cdot ]_\WT:\WT'\times \WT\rightarrow \mathbb{R} $ be its duality pairing. Suppose there exist an nonempty set \( \Omega \) and a corresponding feature mappings $\Phi : \Omega \to \WT',$.  We can  construct a Reproducing Kernel Banach Space as $$\mathcal{B} := \left\{ f_v(x) := [ \Phi(x), v ]_{\WT} : v \in \WT, x \in \Omega \right\}  $$
with norm$\|f_v\|_{\mathcal{B}} := \inf\{\|v\|_{\WT}: v\in W\ \text{ with }\ f=[ \Phi(\cdot), v ]_{\WT}\}.$
{{< /admonition >}}



### Examples of RKBS

#### Neural Networks

