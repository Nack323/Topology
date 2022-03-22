---
title: Topology Notes
---

# Homeomorphisms

## Subspaces

**Defn** Take $(X, \tau)$ and $Y \subseteq X$. Then $\tau_y = \{U \cap
Y : O \in \tau\}$ is the subspace topology

## Homeomorphisms

**Defn** $f: X \to Y$ is a *homeomorphism* if $f$ is bijective and 

i) $\forall U \in \tau_1, f^{-1}(U)\in \tau$
ii) $\forall V \in \tau, f(V) \in \tau_1$

**Properties preserved by homeomorphism**:

* $T_0$ Space
* $T_1$ Space
* $T_2$ Space
* $T_3$ Space
* Regular space
* Discrete
* Indiscrete
* Finite closed
* Countable Closed
* Connected

**Defn** $S \subseteq \mathbb R$ is an interval if $\forall x, y \in
S$, $x < a < z \implies a \in S$

**Propn** A subset of $\mathbb R$ is connected iff it's an interval 

# Continuous Mappings

**Defn** Let $(X, \tau), (Y, \tau_1)$. $f: (X, \tau) \to (Y, \tau_1)$
is continuous if $\forall U \in \tau_1$, $f^{-1}(U) \in \tau$
*every open subset has an open inverse image*

**Propn** $f$ is continuous iff $\forall x \in X$ and $\forall U
\in \tau'$ that contains $f(x)$, $\exists V \in \tau$ st $x \in V,
f(V) \subseteq U$

**Propn** The composition of continuous mappings is continuous

**Propn** The definition of continuous also works when replacing open
with closed

## IVT

**Propn** Any continuous image of a connected space is connected. For
that to work, the continuous function has to be surjective.

**Propn** Intermediave value theorem (remember the picture)


# Chapter 6: Metric spaces

## 6.1 Metric spaces

**Definition** $d$ is a metric iff

* $d(a, b) \leq 0$ and $d(a, b) = 0$ iff $a = b$

* $d(a, b) = d(b, a)$

* $d(a, c) \leq d(a, b) + d(b, c)$ (triangle inequality)

**Definition** the open ball about $a \in X$ of radius $r$ is $B_r(a) = \{x : x
\in X \land d(a, x) < r\}$

**Definition** The collection of open balls in $(X, d)$ forms a basis for a
topology in $X$ called the *induced topology*

**Definition** Two metrics are equivalent if they induce the same topology

**Proposition** $(X, d)$ with the induced topology$\tau$. Then $U \subseteq X$
is open in $\tau$ iff $\forall a \in U$ there exists $\epsilon > 0$ st
$B_\epsilon (a) \subseteq U$

**Definition** $(X, \tau)$ is $T_2$ if for any pair a, b of distinct points
there exists $U, V \in \tau$ st $a \in U$, $b \in V$ and $U \cap V = \emptyset$ 

**Definition** a space is *metrizable* if there exists a metrix that induces
the topology

Note: not every T2 space is metrizable

## 6.2 Convergence of Sequences

**Definition** let $\{x_1, ..., x_n, ...\}$ be a sequence of points in $X$. The
sequence *converges* to $x \in X$ if $\forall \epsilon > 0$, there exists $n_0$
such that $n > n_0 \implies d(x, x_n) < \epsilon$. When that happens, we can
write $x_n \to x$

**Proposition** if $x_n \to x$ and $x_n \to y$ then $x = y$

**Proposition** $A \subseteq X$ is closed in $(X, d)$ iff every convergent
sequence of points in $A$ converges to a point in $A$. 

**Proposition** take $(X, d)$ and $(Y, d_1)$ be metric spaces and $f: X \to Y$.
$f$ is continuous iff $x_n \to x \implies f(x_n) \to f(x)$.


## 6.3 Completeness

**Definition** A sequence $x_1, ...$ is a *Cauchy Sequence* if for any $\epsilon>0$ there exists $n_0$ such that $m, n > n_0$ implies $d(x_m, x_n) < \epsilon$.

**Proposition** A sequence that converges in a metric space is a Cauchy Sequence.

*Note*: The converse is not always true

**Definition** A metric space is *complete* if every Cauchy sequence converges

**Definition** If $\{x_n\}$ is a sequence, then $x_{n_1}, x_{n_1}, ...$ is a subsequence.

**Definition** If the sequence is in $\mathbb{R}$ and $x_n \leq x_{n + 1}$ then it's said to be increasing. The same for decreasing. If it's increasing or decreasing, it's said to be monotonic

**Lemma** Every sequence has a monotonic subsequence

**Proposition** if $\{x_n\}$ is a monotonic sequence in $R$ then it converges iff it's bounded.

**Bolzano Weierstrass** Every boundad sequence in $\mathbb{R}$ has a convergent subsequence.

**Theorem** R is complete

**Definition** Completely metrizable if there is a complete metric that induces the topology

**Definition** Separable if it has a countable dense subset.

**Definition** Polish space if it's separable and completely metrizable

**Definition** Suslin space if it's Hausdorff and a continuous image of a polish space. 

**Definition** Analytic set (check later)

**Definition** A surjective mapping $f: X \to Y$ such that for all $x, y$, $d(x, y) = d_1(f(x), f(y))$ is called an *Isometry*

**Definition** A metric space $Y$ is called a completion if there exists an isometry $f$ into $Y$ such that $f(X)$ is dense in $Y$.

