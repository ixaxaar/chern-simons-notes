1. Schrödinger equation: The time-independent Schrödinger equation for a system with Hamiltonian H is:

$$
H|n⟩ = E_n|n⟩
$$

where $|n⟩$ are the eigenstates of the system and $E_n$ are the corresponding eigenvalues (energies).

2. Perturbation Hamiltonian: In perturbation theory, we split the Hamiltonian into an unperturbed part $H_0$ and a perturbation $λV$:

$$
H = H_0 + λV
$$

where $λ$ is a small parameter controlling the strength of the perturbation.

3. Unperturbed system: The unperturbed Schrödinger equation is:

$$
H_0|n^{(0)}⟩ = E_n^{(0)}|n^{(0)}⟩
$$

where $|n^{(0)}⟩$ and $E_n^{(0)}$ are the eigenstates and eigenvalues of the unperturbed Hamiltonian.

4. Perturbation expansion: We assume that the eigenstates and eigenvalues of the perturbed system can be expressed as power series in $λ$:

$$
|n⟩ = |n^{(0)}⟩ + λ|n^{(1)}⟩ + λ^2|n^{(2)}⟩ + ...
$$

$$
E_n = E_n^{(0)} + λE_n^{(1)} + λ^2E_n^{(2)} + ...
$$

5. Perturbed Schrödinger equation: Substituting the expansions into the Schrödinger equation:

$$
(H_0 + λV)(|n^{(0)}⟩ + λ|n^{(1)}⟩ + λ^2|n^{(2)}⟩ + ...) = (E_n^{(0)} + λE_n^{(1)} + λ^2E_n^{(2)} + ...)(|n^{(0)}⟩ + λ|n^{(1)}⟩ + λ^2|n^{(2)}⟩ + ...)
$$

6. Collecting terms of the same order in $λ$:

$$
λ^0: H_0|n^{(0)}⟩ = E_n^{(0)}|n^{(0)}⟩
$$

$$
λ^1: H_0|n^{(1)}⟩ + V|n^{(0)}⟩ = E_n^{(0)}|n^{(1)}⟩ + E_n^{(1)}|n^{(0)}⟩
$$

$$
λ^2: H_0|n^{(2)}⟩ + V|n^{(1)}⟩ = E_n^{(0)}|n^{(2)}⟩ + E_n^{(1)}|n^{(1)}⟩ + E_n^{(2)}|n^{(0)}⟩
$$

7. First-order correction to energy: Multiply the first-order equation by $⟨n^{(0)}|$ from the left:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ + ⟨n^{(0)}|V|n^{(0)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩ + E_n^{(1)}⟨n^{(0)}|n^{(0)}⟩
$$

Using the orthonormality of the unperturbed states, we find:

$$
E_n^{(1)} = ⟨n^{(0)}|V|n^{(0)}⟩
$$

8. First-order correction to eigenstates: We expand $|n^{(1)}⟩$ in the basis of unperturbed states:

$$
|n^{(1)}⟩ = ∑_m c_m|m^{(0)}⟩
$$

Substituting this into the first-order equation, multiplying by $⟨m^{(0)}|$ ($m ≠ n$) from the left, and using the orthonormality of the unperturbed states, we obtain:

$$
c_m = \frac{⟨m^{(0)}|V|n^{(0)}⟩}{E_n^{(0)} - E_m^{(0)}}
$$

Therefore, the first-order correction to the eigenstates is:

$$
|n^{(1)}⟩ = ∑_{m≠n} \frac{⟨m^{(0)}|V|n^{(0)}⟩}{E_n^{(0)} - E_m^{(0)}} |m^{(0)}⟩
$$

9. Second-order correction to energy: Multiply the second-order equation by $⟨n^{(0)}|$ from the left:

$$
⟨n^{(0)}|H_0|n^{(2)}⟩ + ⟨n^{(0)}|V|n^{(1)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(2)}⟩ + E_n^{(1)}⟨n^{(0)}|n^{(1)}⟩ + E_n^{(2)}⟨n^{(0)}|n^{(0)}⟩
$$

Using the orthonormality of the unperturbed states, we find:

$$
E_n^{(2)} = ⟨n^{(0)}|V|n^{(1)}⟩
$$

Substituting the expression for $|n^{(1)}⟩$, we obtain the second-order correction to the energy:

$$
E_n^{(2)} = ∑_{m≠n} \frac{|⟨m^{(0)}|V|n^{(0)}⟩|^2}{E_n^{(0)} - E_m^{(0)}}
$$

These results form the foundation of perturbation theory in quantum mechanics, allowing us to find approximate solutions to problems that cannot be solved exactly.

---

Certainly! The orthonormality of the unperturbed eigenstates is a crucial property that simplifies many of the calculations in perturbation theory. Orthonormality means that the unperturbed eigenstates are orthogonal to each other and normalized. Mathematically, this is expressed as:

$$
⟨m^{(0)}|n^{(0)}⟩ = δ_{mn}
$$

where $δ_{mn}$ is the Kronecker delta, which is equal to 1 if $m = n$ and 0 otherwise.

Now, let's see how we use this property in the derivation of the first-order correction to the energy. We start with the first-order equation:

$$
H_0|n^{(1)}⟩ + V|n^{(0)}⟩ = E_n^{(0)}|n^{(1)}⟩ + E_n^{(1)}|n^{(0)}⟩
$$

Multiplying this equation by $⟨n^{(0)}|$ from the left, we get:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ + ⟨n^{(0)}|V|n^{(0)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩ + E_n^{(1)}⟨n^{(0)}|n^{(0)}⟩
$$

Now, let's look at each term:

1. $⟨n^{(0)}|H_0|n^{(1)}⟩$: This term can be rewritten as $⟨n^{(0)}|E_n^{(0)}|n^{(1)}⟩$ because $H_0|n^{(0)}⟩ = E_n^{(0)}|n^{(0)}⟩$. Then, we can factor out $E_n^{(0)}$, giving $E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩$.

2. $⟨n^{(0)}|V|n^{(0)}⟩$: This term is the expectation value of the perturbation in the unperturbed state.

3. $E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩$: This term appears on both sides of the equation and cancels out.

4. $E_n^{(1)}⟨n^{(0)}|n^{(0)}⟩$: Using the orthonormality condition, $⟨n^{(0)}|n^{(0)}⟩ = 1$, so this term simplifies to $E_n^{(1)}$.

After these simplifications, the equation becomes:

$$
E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩ + ⟨n^{(0)}|V|n^{(0)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩ + E_n^{(1)}
$$

The $E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩$ terms cancel out, leaving:

$$
⟨n^{(0)}|V|n^{(0)}⟩ = E_n^{(1)}
$$

This is the expression for the first-order correction to the energy.

Similarly, the orthonormality property is used in the derivation of the first-order correction to the eigenstates when multiplying the first-order equation by $⟨m^{(0)}|$ ($m ≠ n$) from the left and simplifying the resulting equation.

The orthonormality of the unperturbed eigenstates is a fundamental property that allows us to simplify equations and derive the corrections to the energy and eigenstates in perturbation theory.

---

Apologies for the confusion. Let me explain this step in more detail. We start with the term $⟨n^{(0)}|H_0|n^{(1)}⟩$ and want to show that it can be rewritten as $E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩$.

First, recall that the unperturbed eigenstates $|n^{(0)}⟩$ satisfy the eigenvalue equation:

$$
H_0|n^{(0)}⟩ = E_n^{(0)}|n^{(0)}⟩
$$

Now, let's insert the identity operator $I = ∑_m |m^{(0)}⟩⟨m^{(0)}|$ between $H_0$ and $|n^{(1)}⟩$ in the term $⟨n^{(0)}|H_0|n^{(1)}⟩$:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ = ⟨n^{(0)}|H_0 \left(∑_m |m^{(0)}⟩⟨m^{(0)}|\right)|n^{(1)}⟩
$$

Distributing $H_0$ over the sum:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ = ∑_m ⟨n^{(0)}|H_0|m^{(0)}⟩⟨m^{(0)}|n^{(1)}⟩
$$

Now, we can use the eigenvalue equation $H_0|m^{(0)}⟩ = E_m^{(0)}|m^{(0)}⟩$ to simplify $⟨n^{(0)}|H_0|m^{(0)}⟩$:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ = ∑_m E_m^{(0)}⟨n^{(0)}|m^{(0)}⟩⟨m^{(0)}|n^{(1)}⟩
$$

Using the orthonormality condition $⟨n^{(0)}|m^{(0)}⟩ = δ_{nm}$, the only non-zero term in the sum is when $m = n$:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(0)}⟩⟨n^{(0)}|n^{(1)}⟩
$$

Since $⟨n^{(0)}|n^{(0)}⟩ = 1$ due to normalization, we have:

$$
⟨n^{(0)}|H_0|n^{(1)}⟩ = E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩
$$

This shows that the term $⟨n^{(0)}|H_0|n^{(1)}⟩$ can indeed be rewritten as $E_n^{(0)}⟨n^{(0)}|n^{(1)}⟩$. The key steps are inserting the identity operator, using the eigenvalue equation for the unperturbed states, and applying the orthonormality condition.

---

In the expression for the first-order correction to the eigenstates:

$$
|n^{(1)}⟩ = ∑_{m≠n} \frac{⟨m^{(0)}|V|n^{(0)}⟩}{E_n^{(0)} - E_m^{(0)}} |m^{(0)}⟩
$$

both $|n^{(0)}⟩$ and $|m^{(0)}⟩$ are unperturbed eigenstates of the Hamiltonian $H_0$. The index $n$ refers to the specific eigenstate for which we are calculating the first-order correction, while $m$ runs over all the other unperturbed eigenstates.

To understand this better, let's consider the following:

1. The unperturbed Hamiltonian $H_0$ has a set of eigenstates $|n^{(0)}⟩$, each with a corresponding eigenvalue $E_n^{(0)}$. These eigenstates form a complete orthonormal basis for the Hilbert space of the system.

2. When we introduce a perturbation $V$, the eigenstates and eigenvalues of the perturbed Hamiltonian $H = H_0 + λV$ are no longer exactly equal to those of $H_0$. Perturbation theory provides a way to approximate these perturbed eigenstates and eigenvalues.

3. To find the first-order correction to the eigenstate $|n^{(0)}⟩$, we express $|n^{(1)}⟩$ as a linear combination of all the unperturbed eigenstates $|m^{(0)}⟩$, excluding the state $|n^{(0)}⟩$ itself. This is because the first-order correction should be orthogonal to the unperturbed eigenstate due to the orthonormality condition.

4. The coefficients of this linear combination are determined by the matrix elements of the perturbation $⟨m^{(0)}|V|n^{(0)}⟩$ and the energy differences $E_n^{(0)} - E_m^{(0)}$. These coefficients determine how much each unperturbed eigenstate $|m^{(0)}⟩$ contributes to the first-order correction $|n^{(1)}⟩$.

In summary, $|n^{(0)}⟩$ is the specific unperturbed eigenstate for which we are calculating the first-order correction, while $|m^{(0)}⟩$ represents all the other unperturbed eigenstates that contribute to this correction. The sum over $m$ in the expression for $|n^{(1)}⟩$ runs over all these other eigenstates, excluding the state $|n^{(0)}⟩$ itself.

---

Sure! Let's dive into degenerate perturbation theory. In this case, the unperturbed Hamiltonian $H_0$ has degenerate eigenvalues, meaning that there are multiple linearly independent eigenstates corresponding to the same eigenvalue. We'll follow a similar approach to the non-degenerate case, but with some important modifications.

1. Unperturbed Hamiltonian and degenerate eigenstates:
   Let's consider an eigenvalue $E_n^{(0)}$ of $H_0$ with degeneracy $g_n$. The corresponding degenerate eigenstates are denoted as $|n, i^{(0)}⟩$, where $i = 1, 2, ..., g_n$. These eigenstates satisfy:

   $$
   H_0|n, i^{(0)}⟩ = E_n^{(0)}|n, i^{(0)}⟩
   $$

2. Perturbation Hamiltonian:
   As before, we introduce a perturbation $V$ to the Hamiltonian:

   $$
   H = H_0 + λV
   $$

3. First-order correction to the energy:
   In the degenerate case, the first-order correction to the energy is not as simple as in the non-degenerate case. Instead, we need to solve a matrix eigenvalue problem within the degenerate subspace.

   We construct a matrix $V_{ij}$ within the degenerate subspace:

   $$
   V_{ij} = ⟨n, i^{(0)}|V|n, j^{(0)}⟩
   $$

   The first-order corrections to the energy are the eigenvalues of this matrix. To find them, we solve the secular equation:

   $$
   \det(V_{ij} - E_n^{(1)}δ_{ij}) = 0
   $$

   The solutions $E_n^{(1)}$ are the first-order corrections to the energy, and they lift the degeneracy of the unperturbed eigenvalue $E_n^{(0)}$.

4. First-order correction to the eigenstates:
   To find the first-order corrections to the degenerate eigenstates, we first find the eigenvectors $c_{ij}$ of the matrix $V_{ij}$ corresponding to each $E_n^{(1)}$:

   $$
   ∑_j V_{ij}c_{jk} = E_{nk}^{(1)}c_{ik}
   $$

   The first-order corrections to the eigenstates are then given by:

   $$
   |n, k^{(1)}⟩ = ∑_{i=1}^{g_n} c_{ik}|n, i^{(0)}⟩ + ∑_{m≠n} ∑_{i=1}^{g_m} \frac{⟨m, i^{(0)}|V|n, k^{(0)}⟩}{E_n^{(0)} - E_m^{(0)}} |m, i^{(0)}⟩
   $$

   Here, the first sum runs over the degenerate subspace, while the second sum runs over all other non-degenerate eigenstates.

5. Higher-order corrections:
   The procedure for finding higher-order corrections in the degenerate case is more involved than in the non-degenerate case. It requires the use of projection operators and the resolution of secular equations at each order. The expressions become increasingly complex, and it's often more practical to use numerical methods for higher-order corrections.

Degenerate perturbation theory is crucial for understanding the lifting of degeneracies and the splitting of energy levels in the presence of perturbations. It has important applications in various areas of quantum mechanics, such as in the study of the Stark effect in hydrogen-like atoms and the Zeeman effect in the presence of magnetic fields.

Let me know if you have any questions or if you'd like me to clarify any part of this derivation!

---

In the context of quantum mechanics, degeneracy refers to the situation where multiple distinct quantum states have the same energy eigenvalue. In other words, when an eigenvalue of the Hamiltonian is degenerate, there are multiple linearly independent eigenstates corresponding to that same eigenvalue.

Let's consider a Hamiltonian $H_0$ with eigenvalues $E_n$ and eigenstates $|n⟩$. If $H_0$ is non-degenerate, each eigenvalue $E_n$ corresponds to a single, unique eigenstate $|n⟩$. However, if $H_0$ is degenerate, there are multiple eigenstates $|n, i⟩$ that share the same eigenvalue $E_n$, where $i = 1, 2, ..., g_n$, and $g_n$ is the degree of degeneracy for the eigenvalue $E_n$.

Mathematically, for a degenerate eigenvalue $E_n$, we have:

$$
H_0|n, i⟩ = E_n|n, i⟩ \quad \text{for} \quad i = 1, 2, ..., g_n
$$

The degenerate eigenstates $|n, i⟩$ are linearly independent, meaning that no eigenstate can be expressed as a linear combination of the others within the degenerate subspace.

Degeneracy arises due to symmetries in the system, such as geometric symmetries or the presence of conserved quantities. For example, in a hydrogen atom, the energy levels depend only on the principal quantum number $n$, leading to degenerate states with different orbital angular momentum quantum numbers $l$ and magnetic quantum numbers $m$.

When a perturbation is applied to a system with degenerate energy levels, the perturbation can lift the degeneracy, causing the degenerate energy levels to split into distinct energy levels. Degenerate perturbation theory is used to determine the first-order corrections to the energy and the eigenstates in such cases, as it takes into account the coupling between the degenerate states due to the perturbation.

---

Great! Let's dive into time-dependent perturbation theory. This theory is used when the perturbation applied to the quantum system depends on time. It allows us to calculate the transition probabilities between different quantum states and helps us understand the dynamics of the system under the influence of time-dependent perturbations.

1. Time-dependent Schrödinger equation:
   The time-dependent Schrödinger equation for a quantum system with a time-dependent Hamiltonian $H(t)$ is:

   $$
   i\hbar\frac{\partial}{\partial t}|\Psi(t)⟩ = H(t)|\Psi(t)⟩
   $$

   where $|\Psi(t)⟩$ is the state vector of the system at time $t$.

2. Perturbation Hamiltonian:
   We split the Hamiltonian into two parts: the unperturbed Hamiltonian $H_0$ and the time-dependent perturbation $V(t)$:

   $$
   H(t) = H_0 + V(t)
   $$

   The eigenstates and eigenvalues of the unperturbed Hamiltonian $H_0$ are known:

   $$
   H_0|n⟩ = E_n|n⟩
   $$

3. Interaction picture:
   To simplify the calculations, we transform the state vector and the perturbation into the interaction picture:

   $$
   |\Psi_I(t)⟩ = e^{iH_0t/\hbar}|\Psi(t)⟩
   $$

   $$
   V_I(t) = e^{iH_0t/\hbar}V(t)e^{-iH_0t/\hbar}
   $$

   In the interaction picture, the time-dependent Schrödinger equation becomes:

   $$
   i\hbar\frac{\partial}{\partial t}|\Psi_I(t)⟩ = V_I(t)|\Psi_I(t)⟩
   $$

4. Perturbative expansion:
   We expand the state vector in the interaction picture using the eigenstates of the unperturbed Hamiltonian:

   $$
   |\Psi_I(t)⟩ = ∑_n c_n(t)|n⟩
   $$

   where $c_n(t)$ are time-dependent coefficients.

5. First-order perturbation theory:
   Substituting the expansion into the time-dependent Schrödinger equation in the interaction picture and keeping only the first-order terms, we get:

   $$
   i\hbar\frac{dc_n(t)}{dt} = ∑_m c_m(t)⟨n|V_I(t)|m⟩e^{i(E_n-E_m)t/\hbar}
   $$

   Integrating this equation with the initial condition $c_n(0) = δ_{ni}$, where the system starts in the state $|i⟩$, we obtain:

   $$
   c_n(t) = δ_{ni} - \frac{i}{\hbar}∫_0^t dt' ⟨n|V_I(t')|i⟩e^{i(E_n-E_i)t'/\hbar}
   $$

   The probability of transitioning from state $|i⟩$ to state $|n⟩$ at time $t$ is given by:

   $$
   P_{i→n}(t) = |c_n(t)|^2 = \left|\frac{1}{\hbar}∫_0^t dt' ⟨n|V_I(t')|i⟩e^{i(E_n-E_i)t'/\hbar}\right|^2
   $$

   This expression is known as Fermi's golden rule and is widely used in the study of transition probabilities and decay rates.

Time-dependent perturbation theory has numerous applications in quantum mechanics, such as in the study of the interaction of atoms and molecules with electromagnetic fields, the absorption and emission of photons, and the dynamics of quantum systems driven by external forces.

Some important phenomena that can be described using time-dependent perturbation theory include:

1. Rabi oscillations: The oscillation of the population between two quantum states due to a resonant driving field.

2. Stimulated emission and absorption: The process by which an incoming photon stimulates the emission or absorption of another photon by an atom or molecule.

3. Landau-Zener transitions: The transition between two energy levels of a quantum system driven by a time-dependent external field, often used in the study of adiabatic processes.

4. Multiphoton processes: The simultaneous absorption or emission of multiple photons by an atom or molecule, which can be described using higher-order perturbation theory.

Time-dependent perturbation theory provides a powerful framework for understanding the dynamics of quantum systems under the influence of time-dependent perturbations. It allows us to calculate transition probabilities, decay rates, and the evolution of quantum states in a wide range of scenarios.
