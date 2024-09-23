---
{"dg-publish":true,"permalink":"/physics/qm/time-evolution-operator/"}
---

###### Bing's Response
The time evolution operator in quantum mechanics is a unitary operator that describes how the state of a quantum system changes over time. It is usually denoted by
$$U(t) \qquad \text{or} \qquad U(t,t_0)$$where $t$ is the final time and $t_0$ is the initial time. The time evolution operator satisfies the following properties:
1. It reduces to the identity operator when
  $$t=t_0 \longrightarrow U(t_0,t_0) = I$$
2. It preserves the norm of the state vector
  $$\langle \psi(t)|\psi(t)\rangle = \langle \psi(t_0)|\psi(t_0)\rangle$$ for any state vector $|\psi\rangle$. This implies that $U(t,t_0)$ is unitary, that is, $$U^\dagger (t,t_0) = U^{-1}(t,t_0)$$
3. It satisfies the composition rule
   $$U(t_2,t_1)U(t_1,t_0) = U(t_2,t_0)$$for any times $t_0 \leq t_1 \leq t_2$. This means that the time evolution operator is independent of the intermediate steps.

The time evolution operator can be derived from the Schrödinger equation:
$$i\hbar \frac{d}{dt}|\psi(t)\rangle = H(t)|\psi(t)\rangle$$
The Hamiltonian may or may not depend on time explicitly. The solution of the Schrödinger equation can be expressed in terms of the time evolution operator as
$$|\psi(t)\rangle = U(t,t_0)|\psi(t_0)\rangle$$
where $|\psi(t_0)\rangle$ is the initial state of the system.
- If the Hamiltonian is time-independent, then the time evolution operator can be written as
  $$U(t,t_0) = e^{-iH(t-t_0)/\hbar}$$
- If the Hamiltonian is time-dependent, then the time evolution operator can be written as
  $$U(t,t_0) = T e^{-i/\hbar \int_{t_0}^t H(\tau)d\tau}$$
  where $T$ denotes the <span style="background:#00ff00;font-weight:bold"> time-ordering operator </span>, which arranges the terms in the exponential in order of decreasing time. The time-ordering operator ensures that the operators at later times are applied before the operators at earlier times.

The time evolution operator can also be used to define different pictures of quantum mechanics, which are different ways of representing the dynamics of quantum systems. The most common pictures are:

- The Schrödinger picture, in which the state vectors depend on time and the observables are constant. This is the picture we have been using so far.
- The Heisenberg picture, in which the state vectors are constant and the observables depend on time. The observables evolve according to the Heisenberg equation of motion, which can be derived from applying the time evolution operator to both sides of an expectation value.
- The interaction picture, in which both the state vectors and the observables depend on time, but in a simpler way than in the Schrödinger picture. <u>The interaction picture is useful for studying systems that have a separable Hamiltonian into a free part and an interaction part.</u>

