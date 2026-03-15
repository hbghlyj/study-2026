# Problem 1.
(a) True or False: the functor $`M \mapsto\{x \in M: 2 x=0\}`$ from the category of abelian groups to the category of sets is representable.

**Answer**
True. The functor $`M \mapsto\{x \in M: 2 x=0\}`$ is isomorphic to $`M \mapsto\mathrm{Hom}(\mathbb{Z}/2,M)`$. 

(b) True or False: $\mathbb{R}[x, y]$ is a flat $\mathbb{R}[x]$-module (it should be clear what the module structure is).

**Answer**
True. It is a free module, hence flat. As an $\mathbb{R}[x]$-module, it has infinite rank with basis \{$1, y, y^2, \dots$\}.

(c) True or False: if $R$ is a UFD and $\mathfrak{p} \subset R$ is a prime ideal, then $R / \mathfrak{p}$ is a UFD.

(d) Give an example of a ring $R$ such that $(x) \subset R[x]$ is not a prime ideal.

**Answer**

Any integral domain $R$. For example $R=\mathbb{Z}/6$.

(e) What is the cardinality of $((\mathbb{Z} / 10 \mathbb{Z}) \oplus(\mathbb{Z} / 100 \mathbb{Z})) \otimes_{\mathbb{Z}}((\mathbb{Z} / 20 \mathbb{Z}) \oplus(\mathbb{Z} / 25 \mathbb{Z}))$ ?

**Answer**

$\gcd(10,20) \times \gcd(10,25) \times \gcd(100,20) \times \gcd(100,25) = 10 \times 5 \times 20 \times 25 = 25000$

# Problem 2.
Consider the rings $R=\mathbb{Q}[x]$ and $S=\mathbb{Q}[t]$. Turn $S$ into an $R$-algebra using the homomorphism

$$
\phi: R \rightarrow S: f(x) \mapsto f\left(t^3\right) .
$$

(a) Fix $a \in \mathbb{Q}$, and consider the ring

$$
S_a=S \otimes_R R /(x-a) .
$$

How many maximal ideals does the ring have? (The answer may depend on $a$.)

(b) Find values of $a \in \mathbb{Q}$ for which is $S_a$ is not reduced (i.e., it has nilpotents), and describe the nilradical $\operatorname{nil}\left(S_a\right)$.

# Problem 3.
Let $R \subset S$ be a subring. Suppose that $S$ is generated as an $R$-algebra by one element $x \in S$ (so that $S$ may be viewed as a quotient of the polynomial algebra $R[x]$ ). Show that the following two statements are equivalent:

(a) $S$ is a finitely generated $R$-module.

(b) There exists a monic polynomial $p(t) \in R[t]$ such that $p(x)=0$ (in this case, we say that $x$ is integral over $R$ ).

# Problem 4.
A ring $R$ is said to be Artinian if any descending chain of ideals

$$
R \supset I_1 \supset \cdots \supset I_k \supset \ldots
$$

stabilizes.

(a) Show that if a domain is Artinian, it must be a field.

(b) Show that in an Artinian ring, the Jacobson radical coincides with the nilradical.

The remaining problems use the following definition:

Let $R$ be a ring. A class of modules $\mathcal{T} \subset R\text{-mod}$ is called a torsion theory if it satisfies the following conditions:

- $\mathcal{T}$ is closed under extensions and quotients: that is, given a short exact sequence of $R$-modules
  
  $$
  0 \rightarrow M_1 \rightarrow M_2 \rightarrow M_3 \rightarrow 0
  $$
  
  if $M_1, M_3 \in \mathcal{T}$, then $M_2 \in \mathcal{T}$, and if $M_2 \in \mathcal{T}$, then $M_3 \in \mathcal{T}$;
- $\mathcal{T}$ is closed under direct sums: for any collection $`\left\{M_\alpha \in \mathcal{T}\right\}`$, we have $\bigoplus M_\alpha \in \mathcal{T}$. In particular, $0 \in \mathcal{T}$.

  (An example is that if $R$ a domain, we can take $\mathcal{T}$ to be the class of all torsion modules. This example appeared in the homework.)

# Problem 5.
Show that any torsion theory $\mathcal{T} \subset R\text{-mod}$ is a "tensor ideal": for any $M \in \mathcal{T}$ and $N \in R\text{-mod}$, we have $M \otimes N \in \mathcal{T}$.

# Problem 6.
Let $\mathcal{T} \in R\text{-mod}$ be a torsion theory.

(a) Show that any $M \in R\text{-mod}$ contains a largest torsion submodule $M_{\mathcal{T}} \subset M$ : that is, $M_{\mathcal{T}}$ is largest among all submodules $N \subset M$ such that $N \in \mathcal{T}$. (Keep in mind that "largest" is stronger than "maximal"; in particular, there can be at most one largest submodule.)

(b) Show that the correspondence $M \rightarrow M_{\mathcal{T}}$ defines a functor. (By the way, the functor is automatically left exact, but you don't have to prove this.)
