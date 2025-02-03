# linear algebra 2: lecture 1

- grading: final and midterm exam (70/30, but midterm only if it helps)
- no homework

## chapter 1.1: vector spaces
- $\mathbb{R}^n$ is a vector space of all vectors using reals
- this allows addition and scalar multiplication
- can also be complex: $\mathbb{C}^n$
- either of these $\mathbb{R}$ or $\mathbb{C}$ can be denoted as $\mathbb{F}$, with then a set called $\mathcal{V}$ which is a vector space over $\mathbb{F}^n$
- we can define two operations:
    - addition: $u \bigoplus v$
    - scalar multiplication: $c \bigodot v$
- $\mathcal{V}$ must satisfy 8 axioms ot be a vector space:
    1. must have a zero vector (additive identity)
    2. must be commutative (e.g. $u \bigoplus v = v \bigoplus u$)
    3. must be additively associative (e.g. $(u \bigoplus v) \bigoplus w = u \bigoplus (v \bigoplus w)$)
    4. must have an additive inverse (e.g. $\forall v \in \mathbb{F}\exists u \in \mathbb{F} : u \bigoplus v = \mathbf{0}$)
    5. must have a multiplicative identity (e.g. $1 \bigodot v = v$)
    6. must be multiplicative associative (e.g. $c \bigodot (d \bigodot v) = (c \bigodot d) \bigodot v$, $c$ & $d$ are scalars)
    7. must be distributive for scalar multiplication (e.g. $c \bigodot (u \bigoplus v) = c \bigodot u \bigoplus c \bigodot v$)
    8. must be distributive for vector addition (e.g. $(c + d) \bigodot v = c \bigodot v \bigoplus d \bigodot v$)
- so, $\mathbb{F}^n$ is a vector space ($\mathbb{F} = \mathbb{R}$ or $\mathbb{C}$)
- there are some properties to know
- theorem: let $\mathcal{V}$ be a vector space and $u\in \mathcal{V}$
    - $\mathbf{0}$ is unique
    - proof: consider two zero vectors $\vec{0_1}, \vec{0_2}$, both of which must have $\vec{0_i} \bigoplus u = u$. Thus $\vec{0_1} \bigoplus \vec{0_2} = \vec{0_1}$, and $\vec{0_2} \bigoplus \vec{0_1} = \vec{0_2}$. $\vec{0_1} \bigoplus \vec{0_2} = \vec{0_2} \bigoplus \vec{0_1}$ from axiom ii. Thus $\vec{0_1} = \vec{0_2}$
    - $\mathbf{0} \bigodot u = \mathbf{0}$
    - the additive inverse of $u$, $z$, is unique
    - $z = -1 \bigodot u$
    - look up the proofs of the latter three
- for simplicity, we will write $u +v$ instead of $u \bigoplus v$ and $cu$ instead of $c \bigodot u$
- additionally, $-u = (-1)u$ and sometimes $\mathbf{0}$ is $0$

## chapter 1.3: subspaces
- let $\mathcal{V}$ be a vector space over $\mathbb{F}$ and $\mathcal{U}$ be a subset of $\mathcal{V}$: $\mathcal{U} \subseteq \mathcal{V}$. $\mathcal{U}$ is a subspace of $\mathcal{V}$ if $\mathcal{U}$ is a vector space over $\mathbb{F}$ with the same operations as $\mathcal{V}$
- trivial examples: $\mathcal{V}$ and $\mathbf{0}$ are subspaces of $\mathcal{V}$
- we can streamline the verification process. $\mathcal{U}$ is a subspace of $\mathcal{V}$ iff:
    1. $\mathcal{U} \neq \emptyset$
    2. $\forall u, v \in \mathcal{U} : u + v \in \mathcal{U}$
    3. $\forall u \in \mathcal{U}, c \in \mathbb{F} : cu \in \mathcal{U}$
- proof: we need to show axioms i and iv hold for $\mathcal{U}$. let $u \in \mathcal{U}$. We know $0 \in \mathbb{F}$. We also know $0u = \mathbf{0}$. Thus, $\mathbf{0} \in \mathcal{U}$. to show iv, it's enough to show that for any $u \in \mathcal{U}$, $-u \in \mathcal{U}$. We know $-u = (-1)u$. Thus, $-u \in \mathcal{U}$. Thus, $\mathcal{U}$ is a subspace of $\mathcal{V}$. $\blacksquare$

- he gave a bunch of examples but i didnt understand them :(
- 