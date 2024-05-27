- [Lesson 1: Review of Gauge Theory](#lesson-1-review-of-gauge-theory)
  - [1. Principal Bundles and Connections](#1-principal-bundles-and-connections)
    - [Historical Context](#historical-context)
    - [Principal Bundles and Gauge Fields](#principal-bundles-and-gauge-fields)
    - [Principal Bundles: Components and Significance](#principal-bundles-components-and-significance)
      - [1. The Base Manifold ( M )](#1-the-base-manifold--m-)
      - [2. The Total Space ( P )](#2-the-total-space--p-)
      - [Principal Bundle Structure:](#principal-bundle-structure)
      - [Connection 1-Form:](#connection-1-form)
      - [Examples and Intuition:](#examples-and-intuition)
  - [2. Lie Groups and Lie Algebras](#2-lie-groups-and-lie-algebras)
  - [3. Yang-Mills Theory Basics](#3-yang-mills-theory-basics)
- [Exercises](#exercises)

# Lesson 1: Review of Gauge Theory

## 1. Principal Bundles and Connections

### Historical Context

The concept of principal bundles and connections originates from the need to generalize classical field theories to include more complex geometric structures. Principal bundles provide a natural framework for describing gauge fields in theoretical physics, where the gauge group represents the symmetries of the system.

### Principal Bundles and Gauge Fields

Principal bundles provide a natural framework for describing gauge fields because they allow us to formalize the concept of a gauge field as a connection on a bundle. In physics, gauge fields are used to model forces like electromagnetism and the interactions described by the Standard Model. These fields are mathematically described as connections on principal bundles, which capture how fields transform under gauge transformations (symmetries).

### Principal Bundles: Components and Significance

#### 1. The Base Manifold \( M \)

**What It Is:**

- The base manifold \( M \) is the underlying space on which the physical theory is defined.
- In gauge theory, \( M \) typically represents spacetime, with each point in \( M \) corresponding to a location in space and time.

**Significance:**

- The base manifold \( M \) provides the stage on which the physical fields and particles live.
- The structure of \( M \) determines the dimensionality and topology of the physical theory.
- For example, in four-dimensional spacetime, \( M \) would be \(\mathbb{R}^4\) or a more complex manifold with the same dimensionality.

#### 2. The Total Space \( P \)

**What It Is:**

- The total space \( P \) is the space of all possible states of the gauge field over the base manifold \( M \).
- It includes not only the base points in \( M \) but also an additional "fiber" attached to each point in \( M \), representing the possible gauge states.

**Significance:**

- \( P \) incorporates both the geometry of the base space \( M \) and the internal symmetry structure described by the gauge group \( G \).
- Each point in \( P \) corresponds to a pair \((x, g)\) where \( x \in M \) and \( g \in G \). The projection map \(\pi: P \to M\) takes \( (x, g) \) to \( x \).

**Example in Electromagnetism:**

- For electromagnetism, the gauge group is \( U(1) \).
- The base manifold \( M \) is spacetime.
- The total space \( P \) includes all possible phases (elements of \( U(1) \)) at each point in spacetime.
- Each fiber \( G \) (in this case \( U(1) \)) represents the possible values of the gauge field (the electromagnetic potential).

#### Principal Bundle Structure:

A principal \( G \)-bundle \( P(M, G) \) is formally defined by:

1. **Base Manifold \( M \)**:

   - The physical space or spacetime where the theory is formulated.
   - Example: \( M = \mathbb{R}^4 \) for four-dimensional spacetime.

2. **Total Space \( P \)**:

   - The space that combines the base manifold with the gauge group.
   - Each point in \( M \) has a fiber attached, which is a copy of the gauge group \( G \).
   - Example: If \( G = U(1) \), each point in \( M \) is associated with a phase factor \( e^{i\theta} \).

3. **Structure Group \( G \)**:

   - The group representing the symmetries of the gauge field.
   - Example: \( G = SU(2) \) in the context of the weak nuclear force.

4. **Projection Map \( \pi: P \to M \)**:
   - A smooth map that projects each point in the total space \( P \) to the base manifold \( M \).
   - For a point \( p \in P \), \(\pi(p) \in M\).
   - Example: In the Hopf fibration, \( \pi: \mathbb{S}^3 \to \mathbb{S}^2 \) maps each point on \(\mathbb{S}^3\) to \(\mathbb{S}^2\), with fibers being circles \( \mathbb{S}^1 \).

#### Connection 1-Form:

The connection 1-form \( A \in \Omega^1(P, \mathfrak{g}) \) helps in defining parallel transport and curvature in the context of gauge fields.
-> what is omega? g?

- **Local Trivializations**:
  - In each local trivialization \( U_i \times G \), the connection 1-form \( A \) can be represented locally.
  - Transition functions \( g_{ij}: U_i \cap U_j \to G \) describe how to move from one local trivialization to another.
    -> what does this mean?

**Transformation Under Gauge Symmetry:**

The connection 1-form \( A \) transforms as:
\[ A \mapsto g^{-1} A g + g^{-1} dg \]
--> whats d? whats this connection 1-form?

#### Examples and Intuition:

- **Electromagnetic Potential (U(1) Gauge Theory)**:

  - The electromagnetic potential $ A_{\mu} $ can be viewed as a connection 1-form on a \( U(1) \)-bundle.
  - The total space \( P \) includes all possible values of the electromagnetic potential at each point in spacetime \( M \).

- **Yang-Mills Theory**:
  - For non-Abelian gauge groups like \( SU(2) \) or \( SU(3) \), the gauge fields are connections on principal bundles with these groups.
  - The structure of \( P \) reflects the internal degrees of freedom associated with the gauge symmetry.

--> describe all the physical forces and theoir group structure in detail

**Local Trivialization:**

Locally, a principal bundle looks like \(U \times G\), where \(U \subset M\) is an open set. The transition functions \(g_{ij} : U_i \cap U_j \to G\) specify how to glue these local trivializations together. This can be visualized as overlapping charts on a manifold, each chart being "decorated" by the group \(G\).

**Connection 1-Form:**

A connection on a principal bundle is given by a connection 1-form \(A \in \Omega^1(P, \mathfrak{g})\), where \(\mathfrak{g}\) is the Lie algebra of \(G\). The connection 1-form \(A\) helps define a horizontal subspace in the tangent space of \(P\), allowing for parallel transport of elements in the fiber bundle.

**Transformation of Connection 1-Form:**

The connection 1-form transforms under the action of \(G\) as follows:
\[ A \mapsto g^{-1} A g + g^{-1} dg \]
This transformation rule ensures that the connection is compatible with the gauge symmetry of the system.

**Example: Principal \(U(1)\)-Bundle Over \(\mathbb{S}^2\):**

Consider the Hopf fibration, which is a principal \(U(1)\)-bundle over the 2-sphere \(\mathbb{S}^2\). The total space is \(\mathbb{S}^3\), the base space is \(\mathbb{S}^2\), and the fiber is \(U(1)\). The projection map \(\pi: \mathbb{S}^3 \to \mathbb{S}^2\) describes how each point on \(\mathbb{S}^3\) is mapped to \(\mathbb{S}^2\), with fibers corresponding to the orbits of the \(U(1)\) action.

## 2. Lie Groups and Lie Algebras

**Historical Context:**

Lie groups and Lie algebras were developed in the late 19th and early 20th centuries by Sophus Lie and others. They were originally used to study continuous symmetries of differential equations and have since become fundamental in many areas of mathematics and theoretical physics.

**Lie Groups:**

A Lie group \(G\) is a group that is also a smooth manifold, where the group operations (multiplication and inversion) are smooth maps. Examples include \(SU(2)\), \(SO(3)\), and \(U(1)\).

--> I dont know what SO, SU etc are!

**Lie Algebras:**

The Lie algebra \(\mathfrak{g}\) of a Lie group \(G\) is the tangent space at the identity element, equipped with a bilinear operation called the Lie bracket \([ \cdot, \cdot ]: \mathfrak{g} \times \mathfrak{g} \to \mathfrak{g}\). The Lie bracket satisfies the Jacobi identity and is antisymmetric.

**Example: Lie Algebra \(\mathfrak{su}(2)\):**

The Lie algebra \(\mathfrak{su}(2)\) consists of all \(2 \times 2\) skew-Hermitian matrices with trace zero. A basis for \(\mathfrak{su}(2)\) is given by the Pauli matrices:
\[ T_1 = \frac{1}{2} \begin{pmatrix} 0 & i \\ i & 0 \end{pmatrix}, \quad T_2 = \frac{1}{2} \begin{pmatrix} 0 & 1 \\ -1 & 0 \end{pmatrix}, \quad T_3 = \frac{1}{2} \begin{pmatrix} i & 0 \\ 0 & -i \end{pmatrix} \]

The Lie bracket for \(\mathfrak{su}(2)\) is:
\[ [T_i, T_j] = \epsilon*{ijk} T_k \]
where \(\epsilon*{ijk}\) is the Levi-Civita symbol.

## 3. Yang-Mills Theory Basics

**Historical Context:**

Yang-Mills theory was developed by Chen Ning Yang and Robert Mills in the 1950s as a generalization of electromagnetism to non-Abelian gauge groups. It forms the foundation of the Standard Model of particle physics, describing the strong and weak nuclear forces.

**Gauge Fields:**

A gauge field is a connection on a principal bundle. In physics, gauge fields describe the interactions of elementary particles via gauge symmetries.

--> whats a connection

**Curvature (Field Strength):**

The curvature (or field strength) of a connection \(A\) is a 2-form \(F\) defined by:
\[ F = dA + A \wedge A \]
This 2-form \(F\) measures the failure of \(A\) to be locally flat and generalizes the electromagnetic field tensor.

--> describe the equation, what are those operators?

**Example: Curvature of an \(SU(2)\) Connection:**

Given a connection \(A = A^a_\mu T_a dx^\mu\) on a principal \(SU(2)\)-bundle, the curvature \(F\) is:
\[ F = \left( dA^a + \frac{1}{2} \epsilon^{abc} A^b \wedge A^c \right) T_a \]

**Yang-Mills Action:**

The Yang-Mills action for a gauge field \(A\) is given by:
\[ S_{\text{YM}} = \frac{1}{2g^2} \int_M \text{Tr}(F \wedge \ast F) \]
where \(g\) is the coupling constant, \(F\) is the curvature, and \(\ast\) is the Hodge star operator.

--> whats the significance of this? show its usage

**Derivation of Yang-Mills Equations:**

The Yang-Mills equations are derived by varying the Yang-Mills action with respect to the connection \(A\). The variation \(\delta S_{\text{YM}} = 0\) yields:
\[ D_A \ast F = 0 \]
where \(D_A\) is the covariant derivative with respect to \(A\).

--> whats the significance of this? show its usage

# Exercises

1. **Principal Bundle Construction:**

   - Construct a principal \(U(1)\)-bundle over \(\mathbb{S}^2\). Describe the local trivializations and transition functions.

   **Solution:**
   The Hopf fibration \(\mathbb{S}^3 \to \mathbb{S}^2\) can be described using local trivializations. Consider \(\mathbb{S}^2\) as the Riemann sphere, with stereographic projections from the north and south poles. Transition functions between these charts correspond to \(U(1)\) actions that describe rotations in the fiber.

2. **Connection 1-Form:**

   - Given a principal \(SU(2)\)-bundle over \(\mathbb{R}^4\), write down an explicit connection 1-form and compute its curvature 2-form.

   **Solution:**
   An example connection 1-form for \(SU(2)\) could be \(A = A^a_\mu T_a dx^\mu\). The curvature is computed as \(F = dA + A \wedge A\).

3. **Lie Algebras:**

   - Compute the Lie bracket for the Lie algebra \(\mathfrak{su}(2)\). Verify the Jacobi identity for this algebra.

   **Solution:**
   Using the Pauli matrices, compute \([T_i, T_j] = \epsilon_{ijk} T_k\). Verify \([T_i, [T_j, T_k]] + [T_j, [T_k, T_i]] + [T_k, [T_i, T_j]] = 0\).

4. **Yang-Mills Action:**

   - Derive the equations of motion (Yang-Mills equations) from the Yang-Mills action.

   **Solution:**
   Vary \(S*{\text{YM}}\) with respect to \(A\) and set \(\delta S*{\text{YM}} = 0\). Use integration by parts and the properties of the Hodge star operator to derive \(D_A \ast F = 0\).
