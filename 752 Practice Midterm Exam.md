# 1.
Is the Hopf map

$f: S^3 \subset \mathbb{C}^2 \rightarrow S^2=\mathbb{C} \cup\{\infty\}, \quad(z, w) \mapsto \frac{z}{w}$

nullhomotopic? Explain.
# 2.
Let $\Sigma X$ be the suspension of a topological space $X$. If $\alpha \in H^k(\Sigma X)$ and $\beta \in H^l(\Sigma X)$ with $k, l \geq 1$, what is $\alpha \cup \beta$ ? Explain your answer.
# 3.
Is there a continuous map $f: X \rightarrow Y$ inducing isomorphisms on all of the cohomology groups (i.e., $f^*: H^i(Y ; \mathbb{Z}) \xrightarrow{\cong} H^i(X ; \mathbb{Z})$, for all $i$) but $X$ and $Y$ do not have isomorphic cohomology rings (with $\mathbb{Z}$ coefficients)? Explain your answer.
# 4.
If $U \subset \mathbb{R}^n$ and $V \subset \mathbb{R}^m$ are homeomorphic open subsets, is it true that $n=m$? Explain your answer.

**Proof**

Yes, this is true. Let $f: U \to V$ be the homeomorphism. For any point $x \in U$, $f$ induces an isomorphism on local cohomology groups:
$$`f^*: H^k(V, V \setminus \{f(x)\}) \xrightarrow{\cong} H^k(U, U \setminus \{x\})`$$
We know that $`H^k(U, U \setminus \{x\}) \cong \mathbb{Z}`$ for $k=n$ and is $0$ otherwise. Similarly, $`H^k(V, V \setminus \{f(x)\}) \cong \mathbb{Z}`$ for $k=m$ and is $0$ otherwise.
For the groups to be isomorphic for all $k$, we must have $n=m.
