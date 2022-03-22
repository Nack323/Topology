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
