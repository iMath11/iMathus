# Fundamental Theorem of Algebra

**Định lý cơ bản của Đại số** (Gauss, 1799): Every non-constant polynomial with complex coefficients has at least one complex root.[web:57]

## Historical Context
- First proved by Carl Friedrich Gauss at age 22
- 5 different proofs by Gauss himself
- Connects algebra, analysis, topology[web:54]

## Statement

**Theorem**: Let $p(z) = a_n z^n + \cdots + a_1 z + a_0$ be a polynomial of degree $n \geq 1$ with complex coefficients, $a_n \neq 0$. Then $p$ has a root in $\mathbb{C}$.

**Corollary**: $p(z)$ factors completely: $p(z) = a_n (z - r_1)\cdots(z - r_n)$.

## Proof (Analytic - Liouville's Theorem)

### Step 1: Assume No Roots
Suppose $p(z) \neq 0$ for all $z \in \mathbb{C}$. Define
$$f(z) = \frac{1}{p(z)}.$$

### Step 2: Bound at Infinity
For $|z| > R$ large:
$$|p(z)| = |a_n| |z|^n (1 + O(1/|z|)) > |a_0|/2.$$
Thus $|f(z)| < 2/|a_0| |z|^{-n} \to 0$ as $|z| \to \infty$.

### Step 3: Minimum Modulus
$f$ continuous on compact sets. On $|z| \leq R$, $|f|$ attains minimum $m > 0$. But $|f| \to 0$ at $\infty$, contradiction unless $f$ constant.

### Step 4: Polynomial Implies Non-Constant
If $f$ constant, $p$ constant, contradicting $n \geq 1$.

**Thus $p$ has a root!** Factor $p(z) = (z - \alpha) q(z)$, induct on degree.[web:48][web:54]

## Example
$$p(z) = z^3 - 1 = (z-1)(z - e^{2\pi i/3})(z - e^{4\pi i/3}).$$

## Applications
- Every polynomial splits in $\mathbb{C}[z]$
- Field extensions, Galois theory foundation
- Complex analysis (argument principle)[web:57]

**References**: Gauss (1799), Ahlfors Complex Analysis.[web:43][web:57]
