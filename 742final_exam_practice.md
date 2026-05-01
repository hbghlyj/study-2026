# 1
Which of the following fields are isomorphic to a subfield of $\mathbb{C}$?

1. $\overline{\mathbb{Q}}$ (the algebraic closure of $\mathbb{Q}$),
2. $\mathbb{Q}(z)$ (the field of rational functions over $\mathbb{Q}$),
3. $\overline{\mathbb{Q}(z)}$,
4. $\mathbb{Z} / p \mathbb{Z}(z)$ where $p$ is a prime number.

(Side remark: a more challenging question would be about $\mathbb{R}(z)$, or the field of $p$-adic numbers, but this is not part of the problem.)

1. Yes, since $\mathbb{Q}$ is a subfield of $\mathbb{C}$ and $\mathbb{C}$ is algebraically closed.
2. Yes, $\mathbb{Q}(\pi)$
3. Yes, since $\mathbb{Q}(\pi)$ is a subfield of $\mathbb{C}$ and $\mathbb{C}$ is algebraically closed.
4. No, characteristic $p$ subfield cannot be a subfield of characteristic 0 field.

# 2
Set $\alpha=\sqrt{2-\sqrt{2}}$.

1. Find the minimal polynomial of $\alpha$ over $\mathbb{Q}$.
2. Show that $\mathbb{Q}(\alpha) \supset \mathbb{Q}$ is a Galois extension.
3. Find the Galois group $\operatorname{Gal}(\mathbb{Q}(\alpha) / \mathbb{Q})$.

**Proof**
1. Let $f(x) = x^4 - 4x^2 + 2$. Since $2 | 0$ (coefficient of $x^3$), $2 | -4$, $2 | 0$ (coefficient of $x$), $2 | 2$, and $2^2 \nmid 2$, $f(x)$ is irreducible over $\mathbb{Q}$ by Eisenstein's criterion with $p=2$.
2. The roots of $x^4-4x^2+2$ are $\pm \alpha$ and $\pm \beta$ where $\beta = \sqrt{2+\sqrt{2}}$. Since $\alpha\beta = \sqrt{2} = 2-\alpha^2$, we have $\beta = (2-\alpha^2)/\alpha \in \mathbb{Q}(\alpha)$. Thus the polynomial splits in $\mathbb{Q}(\alpha)$. So $\mathbb{Q}(\alpha) \supset \mathbb{Q}$ is a Galois extension.
3. The extension is degree 4. Define $\sigma: \mathbb{Q}(\alpha) \to \mathbb{Q}(\alpha)$ by $\sigma(\alpha) = \beta = (2-\alpha^2)/\alpha$. Then $\sigma^2(\alpha) = \sigma(\beta) = \sigma((2-\alpha^2)/\alpha) = (2-\beta^2)/\beta = (2-(2+\sqrt{2}))/\beta = -\sqrt{2}/\beta = -\alpha$. Since $\sigma^2(\alpha) = -\alpha$, $\sigma^4(\alpha) = \alpha$, so $\sigma$ has order 4 and $\operatorname{Gal}(\mathbb{Q}(\alpha) / \mathbb{Q}) \cong C_4$.
# 3
Let $E \supset \mathbb{Q}$ be a degree four extension. Show that it is impossible for it to have exactly two intermediate fields

$\mathbb{Q} \subsetneq M \subsetneq E .$

(Side remark: the only possibilities for the number of intermediate fields in this situation are $0, 1,$ or $3$.)

**Proof**
Suppose there are at least two distinct intermediate fields $M_1, M_2$. Since the degree of an intermediate extension must divide $[E:\mathbb{Q}]=4$, we have $[M_i:\mathbb{Q}]=2$. Thus $M_1 = \mathbb{Q}(\sqrt{d_1})$ and $M_2 = \mathbb{Q}(\sqrt{d_2})$ for distinct square-free integers $`d_1, d_2 \in \mathbb{Z} \setminus \{1\}`$.

Since $M_1, M_2 \subseteq E$ and $[M_1 M_2 : \mathbb{Q}] = 4$, we have $E = \mathbb{Q}(\sqrt{d_1}, \sqrt{d_2})$. Then $M_3 = \mathbb{Q}(\sqrt{d_1 d_2})$ is also a subfield of $E$. Note that $M_3$ is distinct from $M_1$ and $M_2$: if $\sqrt{d_1 d_2} \in \mathbb{Q}(\sqrt{d_1})$, then $\sqrt{d_2} \in \mathbb{Q}(\sqrt{d_1})$, which contradicts the fact that $x^2 - d_2$ is irreducible over $\mathbb{Q}(\sqrt{d_1})$ for distinct square-free $d_1, d_2$. Thus, if there are at least two intermediate fields, there are at least three.

# 4
Let $n>1$, and set $E=\mathbb{C}(x)$ and $F=\mathbb{R}(x^n)$ (note the fields of coefficients are different!) Prove that $E \supset F$ is a finite Galois extension and find its Galois group.

**Proof**

$E$ is the splitting field of $(X^n-x^n)(X^n+1)$ over $F$, so $E/F$ is Galois.

$\deg(X^2+1)=2$, so $[\mathbb{C}(x^n):\mathbb{R}(x^n)]=2$

$\deg(X^n-x^n)=n$, so $[E:\mathbb{C}(x^n)]=n$

so $[E:F]=[E:\mathbb{C}(x^n)][\mathbb{C}(x^n):\mathbb{R}(x^n)]=2n$.

Define $\sigma\in\mathrm{Gal}(E/\mathbb{R}(x))$ by $\sigma(i)=-i$.

Define $\tau\in\mathrm{Gal}(E/\mathbb{C}(x^n))$ by $\tau(x)=\zeta_n x$.

$\sigma\tau(x)=\zeta_n^{-1}x=\tau^{-1}\sigma(x)$

$\sigma\tau(i)=-i=\tau\sigma(i)$

The map $\phi: D_{2n} \to \mathrm{Gal}(E/F)$ defined by $r \mapsto \sigma, s \mapsto \tau$ is an isomorphism with inverse $\sigma \mapsto r, \tau \mapsto s$.

# 5
Let $E \supset F$ be a Galois extension such that $\operatorname{Gal}(E / F) \simeq S_5$. Prove that $E$ is the splitting field of a degree five polynomial over $F$.

# 6
Let $E \supset F$ be a finite Galois extension, and suppose $f(x) \in F[x]$ is an irreducible polynomial. Let

$f(x)=f_1(x) f_2(x) \cdots f_k(x)$

be the factorization of $f(x)$ in $E[x]$. Prove that all polynomials $f_i$ have the same degree, and that $k \mid[E: F]$.
