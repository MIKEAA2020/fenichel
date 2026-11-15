# Cohomological Inverses and Fractional Jet Spectra in Banach-Space Normally Hyperbolic Persistence

## Abstract

We develop a modular Banach-bundle framework for compact normally hyperbolic persistence in Banach-space dynamics. The framework decomposes the proof into linear cohomological inversion, HPS invariant-section matching, roughness of exponential dichotomies, Perron constructions for strong fibres, and regularity obstructions in induced jet cocycles. The main new analytic contribution is a fractional jet-spectrum theorem for the cohomological operator

\[
\mathcal A\zeta=\zeta\circ f-B\zeta:
\]

bounded invertibility on \(C^{k,\alpha}\) sections follows from a subunit spectral radius of the exact Green summand operators on Hölder jet bundles. We also prove a periodic triangular jet-resonance obstruction to \(C^k\)-surjectivity and a compact-return Fredholm refinement. These linear results are placed within the standard HPS/Banach invariant-section architecture for normally hyperbolic persistence; the full two-sided nonlinear graph transform is used as an external structural input. Supporting modules include Banach-bundle \(C^k\) inversion, Perron strong fibres, dichotomy roughness, parameter expansions, flow reduction, global stable sets, and a noncompact bounded-geometry linear theory. The broader parabolic, random, delay, quasilinear, noncompact nonlinear, and Banach-dimensional settings are presented as conditional extension architectures with their required additional hypotheses.

---

## 1. Introduction

Fenichel theory describes the persistence of normally hyperbolic invariant manifolds under small perturbations, together with the persistence of their stable and unstable laminations. In finite dimensions the theory is classical; see Fenichel [1] and Hirsch, Pugh, and Shub [2]. In Banach spaces the same geometric principle survives, but the proof must be reorganized. Local compactness of the ambient phase space is unavailable; invariant splittings and graph transforms must be controlled by completeness, uniform bundle estimates, Green operators, and Perron contractions rather than by compact neighbourhood arguments.

This paper presents that organization as a modular architecture. The compact persistence theorem itself uses the standard full two-sided HPS invariant-section theorem as a structural input. Around this nonlinear input we prove the linear and semi-linear analytic modules that make the Banach-bundle formulation explicit: cohomological Green inverses, fractional jet spectra, resonance obstructions, roughness of exponential dichotomies, strong-fibre Perron constructions, parameter expansions, flow reduction, and noncompact bounded-geometry linear inverses.

The main new analytic module is the fractional jet-spectrum theorem for the cohomological operator. Instead of measuring regularity only through integer one-step bunching inequalities, we define the exact stable and unstable Green summand operators on Hölder jet sections and use their exponential operator radii to obtain bounded inverse estimates on \(C^{k,\alpha}\). Periodic triangular jet resonances give converse obstructions to \(C^k\)-surjectivity of the linearized cohomological equation. This linear theory does not replace the nonlinear HPS theorem; rather, it sharpens the regularity mechanism that feeds into any HPS or Perron persistence argument in the corresponding Hölder category.

The claims in the paper are organized into four categories.

| Category | Role in the paper |
|---|---|
| Proved modules | Green inverses, fractional jet spectra, resonance obstructions, Perron fibres, roughness estimates, parameter expansions, flow reduction, global stable sets, and noncompact linear inverses. |
| Structural input | The full two-sided HPS/Banach invariant-section theorem used to pass from the linear inverse to the invariant graph. |
| Conditional consequences | Hölder nonlinear regularity and broader extension settings, conditional on the corresponding HPS, semigroup, random, bounded-geometry, or tame estimates. |
| Programmatic extensions | Parabolic, quasilinear, delay, random, noncompact nonlinear, and Banach-dimensional variants, stated with the additional hypotheses they require. |

Section 2 introduces the geometric and dynamical hypotheses. Section 3 proves the linear cohomological inverse theorem and points to the fractional refinement. Section 4 states the HPS invariant-section theorem as a structural input. Section 5 derives compact Fenichel persistence and the conditional nonlinear regularity spectrum. Section 6 constructs stable and unstable fibres. Section 7 treats flows. Section 8 collects the main extension architectures. Section 9 records open problems and spectral directions. Section 10 summarizes the proof architecture. Appendices A--K provide the supporting proofs and the fractional jet-spectrum theorem.

### Notation

For a Banach bundle \(E\to M\), \(\Gamma^k(E)\) denotes the space of \(C^k\) sections. If \(M\) is noncompact, \(C_b^k(M,E)\) denotes bounded \(C^k\) sections with bounded derivatives in uniformly controlled charts. The pullback bundle over \(M\) is denoted \(f^*E\). The cocycle generated by the normal linear maps \(B_m\) is denoted \(\Phi(n,k)\). Stable and unstable projections are denoted by \(P^s\) and \(P^u\). For fibre constructions, \(E^{cu}=TM\oplus E^u\) and \(E^{cs}=TM\oplus E^s\). Weighted sequence and trajectory spaces use the decay exponent as a subscript, for example \(\ell_\gamma^+\).

---

## 2. Geometric and dynamical framework

Let \(X\) be a Banach space. Let \(M\subset X\) be a compact finite-dimensional \(C^{r+1}\) embedded submanifold without boundary, where \(r\ge 1\). Assume that \(M\) admits a split \(C^{r+1}\) tubular neighbourhood. Thus there exists a Banach bundle

\[
E\to M
\]

and a \(C^{r+1}\) tubular embedding

\[
\Theta:U_E\to U_X\subset X,
\qquad
\Theta(m,0)=m,
\]

from a neighbourhood \(U_E\) of the zero section onto a neighbourhood \(U_X\) of \(M\).

Assume that \(E\) has a \(C^r\) connection. Equivalently, we may work in a finite \(C^{r+1}\) bundle atlas with uniformly controlled transition maps. For nearby points \(x,y\in M\), let

\[
P_{x\leftarrow y}:E_y\to E_x
\]

denote the chosen fibre identification, and define

\[
\tau_{y\leftarrow x}:=P_{x\leftarrow y}^{-1}:E_x\to E_y.
\]

For a section \(h:M\to E\), define its transported difference by

\[
\Delta_y^x h
:=
P_{x\leftarrow y}h(y)-h(x)
\in E_x.
\]

We compare bundle-valued quantities using these transported differences.

Let

\[
F_\varepsilon:U_X\to X
\]

be a family of \(C^{r+1}\) local diffeomorphisms defined on a common neighbourhood of \(M\), where \(\varepsilon\) denotes a small parameter. In tubular coordinates, write

\[
\widehat F_\varepsilon
=
\Theta^{-1}\circ F_\varepsilon\circ\Theta,
\]

and

\[
\widehat F_\varepsilon(m,\eta)
=
\bigl(b_\varepsilon(m,\eta),g_\varepsilon(m,\eta)\bigr),
\]

where

\[
b_\varepsilon(m,\eta)\in M,
\qquad
g_\varepsilon(m,\eta)\in E_{b_\varepsilon(m,\eta)}.
\]

Assume that for \(\varepsilon=0\),

\[
b_0(m,0)=f(m),
\qquad
g_0(m,0)=0,
\]

where

\[
f:M\to M
\]

is a \(C^{r+1}\) diffeomorphism. Thus \(M\) is invariant under \(F_0\).

Assume that along \(M\), the tangent space splits as

\[
T_mX=T_mM\oplus E_m^s\oplus E_m^u,
\]

and that this splitting is invariant under \(DF_0\):

\[
DF_0(m)T_mM=T_{f(m)}M,
\]

\[
DF_0(m)E_m^\sigma=E_{f(m)}^\sigma,
\qquad
\sigma\in\{s,u\}.
\]

In tubular coordinates this implies

\[
D_\eta b_0(m,0)=0.
\]

Define the normal linear cocycle

\[
B_m:=D_\eta g_0(m,0):E_m\to E_{f(m)}.
\]

Because \(F_0\) is a local diffeomorphism and the splitting is invariant, \(B_m\) is an isomorphism; the restrictions

\[
B_m^s:E_m^s\to E_{f(m)}^s,
\qquad
B_m^u:E_m^u\to E_{f(m)}^u
\]

are isomorphisms.

---

### 2.1. Exponential dichotomy

For \(m\in M\), write

\[
m_n=f^n(m).
\]

Let

\[
\Phi(n,k):E_{m_k}\to E_{m_n}
\]

denote the evolution operator associated with \(B\). Thus

\[
\Phi(n,k)=B_{m_{n-1}}\cdots B_{m_k},
\qquad
n>k,
\]

and \(\Phi(k,k)=I\).

Assume that \(B\) admits a continuous invariant exponential dichotomy. Thus there exist uniformly bounded projections

\[
P_m^s:E_m\to E_m^s,
\qquad
P_m^u:E_m\to E_m^u
\]

and constants \(C>0\), \(0<\lambda<1\), such that for all \(n\ge k\),

\[
\|\Phi(n,k)P_k^s\|
\le
C\lambda^{n-k},
\]

and

\[
\|\Phi(k,n)P_n^u\|
\le
C\lambda^{n-k}.
\]

Equivalently, the stable evolution contracts forward in time, while the unstable evolution contracts backward in time.

---

### 2.2. Bunching assumptions

The persistence of \(C^r\) regularity requires bunching inequalities. We use the following coordinate-invariant formulation. For each \(0\le j\le r\), assume that there exist constants \(C_j>0\) and \(\theta_j\in(0,1)\) such that, along every orbit \(m_n=f^n(m)\),

\[
\|\Phi(n,0)|_{E_m^s}\|\,
\|Df^{-n}(m_n)\|^j
\le
C_j\theta_j^n,
\qquad n\ge0,
\]

and

\[
\|\Phi(-n,0)|_{E_m^u}\|\,
\|Df^n(m)\|^j
\le
C_j\theta_j^n,
\qquad n\ge0.
\]

Here \(\Phi(-n,0)\) denotes the inverse unstable evolution from \(E_m^u\) to \(E_{m_{-n}}^u\). A convenient sufficient one-step form is

\[
\sup_{m\in M}
\|B_m^s\|\,\|Df(m)^{-1}\|^j
<1,
\]

and

\[
\sup_{m\in M}
\|(B_m^u)^{-1}\|\,\|Df(m)\|^j
<1.
\]

One often obtains this one-step form after passing to an iterate and introducing an adapted norm. If adapted norms or iterates are used, one must verify that the adapted norms are uniformly equivalent to the original norms and that the perturbation remains small in the adapted topology. Otherwise the quantitative \(C^r\) estimates may not transfer back to the original topology.

The integer bunching inequalities are convenient sufficient conditions. Appendix K gives a sharper linear formulation in Hölder spaces: the boundedness of the Green inverse on \(C^{k,\alpha}\) is controlled by the exponential growth radius of the exact Green summand operators on Hölder \(k\)-jet sections. This fractional jet spectrum includes Hölder distortion of the cocycle, projections, derivative iterates, and bundle transports.

---

## 3. The linear cohomological inverse theorem

Let \(\Gamma^k(E)\) denote the Banach space of \(C^k\) sections of \(E\), and let \(\Gamma^k(f^*E)\) denote the corresponding space of sections of the pullback bundle \(f^*E\). Since \(f\) is a diffeomorphism, \(\Gamma^k(f^*E)\) is canonically isomorphic to \(\Gamma^k(E)\) after relabelling the base point.

Define the cohomological operator

\[
\mathcal A:\Gamma^k(E)\to\Gamma^k(f^*E)
\]

by

\[
(\mathcal A\zeta)(m)
=
\zeta(f(m))-B_m\zeta(m).
\]

The linear theorem is the following.

---

### Theorem 3.1. Linear cohomological inverse

Assume that \(B\) has an exponential dichotomy and satisfies the \(j\)-bunching inequalities for every \(0\le j\le r\). In the self-contained smooth-splitting version, assume moreover that the invariant splitting and the dichotomy projections have the required \(C^r\) regularity with uniformly bounded derivatives in the chosen bundle atlas. Then for every \(0\le k\le r\), the operator

\[
\mathcal A:\Gamma^k(E)\to\Gamma^k(f^*E)
\]

is an isomorphism. Its inverse

\[
\mathcal G:\Gamma^k(f^*E)\to\Gamma^k(E)
\]

is bounded:

\[
\|\mathcal Gq\|_{C^k}
\le
C_k\|q\|_{C^k}.
\]

If the dichotomy projections are only continuous, this differentiable-projection proof should be replaced by the HPS transported difference-quotient theorem. Continuity of the projections alone is not asserted to imply \(C^k\) regularity; the continuous-splitting statement is understood only under the corresponding HPS difference-quotient hypotheses.

If \(q\) depends on a parameter and the dichotomy and bunching estimates are uniform, then parameter regularity follows to the extent supplied by the corresponding mixed base/parameter estimates.

---

### Proof

We first prove the \(C^0\) statement.

Let \(q\in\Gamma^0(f^*E)\). For \(m\in M\), set

\[
m_n=f^n(m),
\qquad
q_n=q(m_n)\in E_{m_{n+1}}.
\]

The equation

\[
\zeta(f(m))-B_m\zeta(m)=q(m)
\]

becomes along the orbit

\[
\zeta_{n+1}-B_{m_n}\zeta_n=q_n.
\]

Decompose

\[
q_n=q_n^s+q_n^u,
\qquad
q_n^\sigma=P_{m_{n+1}}^\sigma q_n,
\]

since \(q_n\in E_{m_{n+1}}\).

Define

\[
\zeta_n^s
=
\sum_{j=-\infty}^{n-1}
\Phi^s(n,j+1)q_j^s,
\]

and

\[
\zeta_n^u
=
-
\sum_{j=n}^{\infty}
\Phi^u(n,j+1)q_j^u.
\]

Finally set

\[
\zeta_n=\zeta_n^s+\zeta_n^u.
\]

The exponential dichotomy gives

\[
\|\Phi^s(n,j+1)q_j^s\|
\le
C\lambda^{n-j-1}\|q_j^s\|,
\]

and therefore

\[
\|\zeta_n^s\|
\le
C\|P^s\|
\sum_{j=-\infty}^{n-1}\lambda^{n-j-1}
\|q\|_{C^0}.
\]

Changing variables \(\ell=n-j-1\), we obtain

\[
\sum_{j=-\infty}^{n-1}\lambda^{n-j-1}
=
\sum_{\ell=0}^{\infty}\lambda^\ell
=
\frac1{1-\lambda}.
\]

Thus

\[
\|\zeta_n^s\|
\le
\frac{C\|P^s\|}{1-\lambda}\|q\|_{C^0}.
\]

Similarly,

\[
\|\zeta_n^u\|
\le
\frac{C\|P^u\|}{1-\lambda}\|q\|_{C^0}.
\]

Consequently,

\[
\|\zeta_n\|
\le
C_G\|q\|_{C^0},
\]

where

\[
C_G
=
\frac{C(\|P^s\|+\|P^u\|)}{1-\lambda}.
\]

Define

\[
(\mathcal Gq)(m):=\zeta_0.
\]

We verify that \(\mathcal A\mathcal Gq=q\). For the stable part,

\[
\zeta_{n+1}^s
=
\sum_{j=-\infty}^{n}
\Phi^s(n+1,j+1)q_j^s,
\]

while

\[
B_{m_n}\zeta_n^s
=
\sum_{j=-\infty}^{n-1}
\Phi^s(n+1,j+1)q_j^s.
\]

Therefore,

\[
\zeta_{n+1}^s-B_{m_n}\zeta_n^s
=
q_n^s.
\]

For the unstable part,

\[
\zeta_{n+1}^u
=
-
\sum_{j=n+1}^{\infty}
\Phi^u(n+1,j+1)q_j^u,
\]

and

\[
B_{m_n}\zeta_n^u
=
-
\sum_{j=n}^{\infty}
\Phi^u(n+1,j+1)q_j^u.
\]

Hence

\[
\zeta_{n+1}^u-B_{m_n}\zeta_n^u
=
q_n^u.
\]

Adding the stable and unstable parts yields

\[
\zeta_{n+1}-B_{m_n}\zeta_n=q_n.
\]

At \(n=0\), this is precisely

\[
\zeta(f(m))-B_m\zeta(m)=q(m).
\]

Thus

\[
\mathcal A\mathcal Gq=q.
\]

We next prove uniqueness of bounded solutions. Suppose \(\zeta\) is a bounded bi-infinite solution of the homogeneous equation

\[
\zeta_{n+1}=B_{m_n}\zeta_n.
\]

Decompose \(\zeta_n=\zeta_n^s+\zeta_n^u\). For the stable part, for \(k\le n\),

\[
\zeta_n^s=\Phi^s(n,k)\zeta_k^s.
\]

Therefore,

\[
\|\zeta_n^s\|
\le
C\lambda^{n-k}\|\zeta_k^s\|.
\]

Since \(\zeta\) is bounded, letting \(k\to-\infty\) gives \(\zeta_n^s=0\). For the unstable part, for \(k\ge n\),

\[
\zeta_n^u=\Phi^u(n,k)\zeta_k^u,
\]

where \(\Phi^u(n,k)\) denotes backward unstable evolution. Then

\[
\|\zeta_n^u\|
\le
C\lambda^{k-n}\|\zeta_k^u\|.
\]

Letting \(k\to+\infty\) gives \(\zeta_n^u=0\). Hence the bounded homogeneous solution is trivial.

We verify that \(\mathcal Gq\) is continuous. For fixed integers \(j,n\), the map

\[
m\mapsto \Phi(n,j+1)P_{m_{j+1}}q(m_j)
\]

is continuous. The stable and unstable sums converge uniformly in \(m\) because of the exponential estimates and compactness of \(M\). Therefore \(\mathcal Gq\) is continuous. This proves the \(C^0\) theorem.

For \(C^k\) regularity, we use the induced jet equations. If the dichotomy projections and invariant splitting have the corresponding regularity, one may differentiate the cohomological equation directly. If the projections are only continuous, the same argument is formulated with transported difference quotients, as in the Hirsch–Pugh–Shub proof. The formal differentiated equations below then describe the limiting difference-quotient equations.

First consider \(k=1\). In local bundle coordinates, differentiating

\[
\zeta(f(m))-B_m\zeta(m)=q(m)
\]

gives

\[
D\zeta(f(m))Df(m)-B_mD\zeta(m)
=
Dq(m)+D_mB(m)\zeta(m).
\]

Writing

\[
J(m):=D\zeta(m),
\]

we obtain

\[
J(f(m))
-
B_mJ(m)Df(m)^{-1}
=
\bigl[Dq(m)+D_mB(m)\zeta(m)\bigr]Df(m)^{-1}.
\]

Thus \(J\) satisfies a cohomological equation over the induced first-jet cocycle

\[
J\mapsto B_mJ\,Df(m)^{-1}.
\]

In a nontrivial bundle, the chosen connection and transported derivatives produce the same principal cocycle; the connection terms are lower-order terms controlled by \(\|\zeta\|_{C^0}\) and the fixed bundle geometry.

Along an orbit \(m_n=f^n(m)\), the homogeneous first-jet equation gives

\[
J_n=\Phi(n,0)J_0Df^{-n}(m).
\]

On the stable component,

\[
\|J_n^s\|
\le
\|\Phi^s(n,0)\|\,\|Df^{-n}(m)\|\,\|J_0^s\|,
\]

and the \(1\)-bunching condition gives exponential contraction. On the unstable component, backward iteration gives

\[
\|J_{-n}^u\|
\le
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|\,\|J_0^u\|,
\]

which also contracts by \(1\)-bunching. Hence the induced first-jet cocycle has an exponential dichotomy. Applying the \(C^0\) Green construction to the first-jet equation gives

\[
\|J\|_{C^0}\le C\|Q_1\|_{C^0},
\]

where \(Q_1\) denotes the right-hand side above. Since \(Q_1\) depends linearly on \(Dq\) and on \(\zeta\), and since

\[
\|\zeta\|_{C^0}\le C\|q\|_{C^0},
\]

we obtain

\[
\|\zeta\|_{C^1}\le C_1\|q\|_{C^1}.
\]

For higher \(k\), proceed by induction. The \(k\)-th derivative of

\[
\zeta\circ f-B\zeta=q
\]

has principal part

\[
D^k\zeta(f(m))\circ Df(m)^{\otimes k}
-
B_mD^k\zeta(m).
\]

All other terms involve derivatives of \(f\) and \(B\) up to order \(k\), derivatives of \(q\) up to order \(k\), and derivatives of \(\zeta\) of order at most \(k-1\). The induction hypothesis controls these lower-order terms. The principal homogeneous \(k\)-jet equation is governed by

\[
J\mapsto B_mJ\circ(Df(m)^{-1})^{\otimes k},
\]

where

\[
J(m)\in\operatorname{Sym}^k(T_m^*M;E_m).
\]

Its stable part is controlled by

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m)\|^k,
\]

and its backward unstable part by

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|^k.
\]

The \(k\)-bunching condition gives an exponential dichotomy for this induced \(k\)-jet cocycle. Applying the \(C^0\) Green construction to the induced equation gives

\[
\|D^k\zeta\|_{C^0}\le C_k\|q\|_{C^k}.
\]

Induction yields

\[
\|\mathcal Gq\|_{C^k}\le C_k\|q\|_{C^k}.
\]

When the projections are not differentiable, the argument is interpreted in the transported difference-quotient sense rather than by differentiating the splitting. This is the linear version of the HPS topological-jet argument; alternatively, one may assume \(C^r\) regularity of the splitting and work with ordinary jet bundles. If \(V\) is a smooth vector field on \(M\) with local flow \(\varphi_t\), define

\[
\zeta_t(m)
=
\frac{
P_{m\leftarrow\varphi_t(m)}\zeta(\varphi_t(m))-\zeta(m)
}{t}.
\]

Applying the cohomological operator to \(\zeta_t\) gives a difference-quotient equation whose commutator terms come from the variation of \(f\), \(B\), and the fibre identifications. These terms converge to the lower-order terms in the formal jet equations above. The uniform Green bounds for the induced difference-quotient cocycles imply convergence of the difference quotients and hence genuine \(C^k\) regularity.

Parameter dependence follows from the same estimates. If the data and dichotomy projections depend continuously on a parameter and the dichotomy constants are uniform, then the Green sums converge uniformly in both the base point and the parameter. Higher parameter regularity follows by differentiating the parameter-dependent cohomological equation, or by using parameter difference quotients, provided the corresponding parameter-bunching estimates hold. ∎

Appendix A gives a self-contained proof of the \(C^k\) cohomological inverse theorem under the clean hypothesis that the splitting and projections have the required \(C^r\) regularity. The continuous-projection version used in the HPS setting should be read in the transported difference-quotient sense described above. Appendix K sharpens the linear theory in the \(C^{k,\alpha}\) scale by replacing integer bunching with a fractional jet-spectrum condition and by recording periodic jet-resonance obstructions.

---

## 4. The invariant-section theorem

The persistence theorem uses the invariant-section theorem of Hirsch, Pugh, and Shub, adapted to Banach bundles. We state it as a theorem on invariant sections of a Banach bundle over a compact finite-dimensional base.

---

Let

\[
\mathcal B_{\rho,L}
=
\left\{
h\in C^0(M,E):
\|h\|_{C^0}\le \rho,
\ \operatorname{Lip}(h)\le L
\right\}.
\]

Equip \(\mathcal B_{\rho,L}\) with the \(C^0\) metric. Since \(M\) is compact and the Lipschitz bound is uniform, \(\mathcal B_{\rho,L}\) is complete.

The constants are chosen in the following order. First choose an iterate or a uniformly equivalent adapted norm, if needed, so that the bunching margins are strict. Then choose the tube radius \(\rho>0\), then the cone or Lipschitz aperture \(L>0\), and finally choose the perturbation size \(\delta_\varepsilon\) small enough. The \(C^0\) radius and the Lipschitz or cone aperture play different roles and are controlled separately.

Let \(\kappa>0\). In local coordinates adapted to

\[
TE|_M \simeq TM\oplus E^s\oplus E^u,
\]

define center cones by

\[
\mathcal C^c_{(m,\eta)}
=
\left\{
(v^c,v^s,v^u):
\|(v^s,v^u)\|\le \kappa\|v^c\|
\right\}.
\]

Similarly define stable and unstable cones by

\[
\mathcal C^s_{(m,\eta)}
=
\left\{
(v^c,v^s,v^u):
\|v^u\|\le \kappa(\|v^c\|+\|v^s\|)
\right\},
\]

and

\[
\mathcal C^u_{(m,\eta)}
=
\left\{
(v^c,v^s,v^u):
\|v^s\|\le \kappa(\|v^c\|+\|v^u\|)
\right\}.
\]

A \(C^1\) section with \(\operatorname{Lip}(h)\le\kappa\) has a graph tangent to the center cones; a merely Lipschitz section satisfies the corresponding secant-cone condition. The center cones describe admissible graphs, while the stable and unstable cones enter the two-sided Hadamard matching construction.

In the two-sided normally hyperbolic case, we do not assert that \(DF_\varepsilon\) maps center cones forward into center cones; unstable expansion can destroy such a statement. Instead, the graph transform is a two-sided Hadamard transform. It preserves the admissible class of Lipschitz graphs by stable and unstable matching estimates and is a contraction in the transported \(C^0\) graph metric. The estimates use the stable and unstable bounds for \(B\), the boundedness of the tangent dynamics \(Df\), the smallness of the base-normal coupling, and the strengthened remainder estimates below.

---

### Theorem 4.1. Hirsch–Pugh–Shub invariant-section theorem

Let \(E\to M\) be a \(C^{r+1}\) Banach bundle over a compact finite-dimensional \(C^{r+1}\) manifold without boundary. Let \(f:M\to M\) be a \(C^{r+1}\) diffeomorphism. Let \(B\in\Gamma^r(\operatorname{Aut}(E))\) have an exponential dichotomy over \(f\), and assume the \(j\)-bunching inequalities for every \(0\le j\le r\).

Let \(F_\varepsilon\) be a family of \(C^{r+1}\) fibre maps defined near the zero section, written in bundle coordinates as

\[
F_\varepsilon(m,\eta)
=
\bigl(b_\varepsilon(m,\eta),g_\varepsilon(m,\eta)\bigr).
\]

Assume the following.

1. For \(\varepsilon=0\),

   \[
   b_0(m,0)=f(m),
   \qquad
   g_0(m,0)=0,
   \]

   and

   \[
   D_\eta b_0(m,0)=0.
   \]

2. The normal linear part satisfies

   \[
   D_\eta g_0(m,0)=B_m.
   \]

3. For \(\varepsilon\neq0\), the maps \(F_\varepsilon\) are sufficiently \(C^1\)-close to \(F_0\) on a small tube. In particular, \(b_\varepsilon(m,0)\) is \(C^1\)-close to \(f(m)\), \(g_\varepsilon(m,0)=O(\delta_\varepsilon)\), and the normal linear part \(D_\eta g_\varepsilon(m,0)\), transported to the fibre over \(f(m)\), is \(O(\delta_\varepsilon)\)-close to \(B_m\).

4. Let

   \[
   r_\varepsilon(m,\eta)
   :=
   g_\varepsilon(m,\eta)
   -
   \tau_{b_\varepsilon(m,\eta)\leftarrow f(m)}
   B_m\eta.
   \]

   Then on a tube \(\|\eta\|\le\rho\),

   \[
   \|r_\varepsilon(m,0)\|
   \le
   C\delta_\varepsilon,
   \]

   and

   \[
   \|D_\eta r_\varepsilon(m,\eta)\|
   \le
   C\delta_\varepsilon+\omega(\rho),
   \]

   where

   \[
   \delta_\varepsilon:=\|F_\varepsilon-F_0\|_{C^1},
   \]

   and \(\omega(\rho)\to0\) as \(\rho\to0\).

   In adapted bundle charts, assume also the base derivative estimate

   \[
   \|D_m r_\varepsilon(m,\eta)\|
   \le
   C\delta_\varepsilon+\omega(\rho).
   \]

   In the present NHIM setting this follows from \(g_0(m,0)=0\), \(D_\eta g_0(m,0)=B_m\), and \(C^{r+1}\) regularity after subtracting the transported linear part. This estimate prevents a non-small base-variation term in the Lipschitz preservation argument.

   Equivalently, after reducing the tube if necessary, these estimates imply

   \[
   \|r_\varepsilon(m,\eta)\|
   \le
   C\delta_\varepsilon+\omega(\rho)\|\eta\|.
   \]

   Assume also that the base nonlinear part satisfies

   \[
   \|D_\eta b_\varepsilon(m,\eta)\|
   \le
   C\delta_\varepsilon+\omega(\rho)
   \]

   on the same tube. This follows from \(D_\eta b_0(m,0)=0\) when \(F_\varepsilon\) is \(C^1\)-close to \(F_0\).

Then there exist constants \(\rho>0\), \(L>0\), and \(\delta_0>0\) such that if \(\delta_\varepsilon<\delta_0\), there exists a locally unique section

\[
h_\varepsilon\in\Gamma^r(E)
\]

satisfying

\[
\|h_\varepsilon\|_{C^0}\le\rho,
\qquad
\operatorname{Lip}(h_\varepsilon)\le L,
\]

Define

\[
f_\varepsilon(m):=b_\varepsilon(m,h_\varepsilon(m)).
\]

Then \(h_\varepsilon\) satisfies the graph equation

\[
h_\varepsilon(f_\varepsilon(m))
=
g_\varepsilon(m,h_\varepsilon(m)),
\]

or equivalently

\[
F_\varepsilon(m,h_\varepsilon(m))
=
\bigl(f_\varepsilon(m),h_\varepsilon(f_\varepsilon(m))\bigr).
\]

Moreover, \(f_\varepsilon\) is a \(C^r\) local diffeomorphism \(C^1\)-close to \(f\). Setwise equality

\[
F_\varepsilon(\operatorname{graph}(h_\varepsilon))
=
\operatorname{graph}(h_\varepsilon)
\]

follows once \(f_\varepsilon\) is known to be onto; in Theorem 5.1 this is proved by the compact local-diffeomorphism argument.

If, in addition,

\[
\|F_\varepsilon-F_0\|_{C^k}
\le
C|\varepsilon|,
\qquad
0\le k\le r,
\]

with uniform \(C^k\) bounds on the tube, then

\[
\|h_\varepsilon\|_{C^k}
\le
C_k|\varepsilon|.
\]

If \(F_\varepsilon\) depends \(C^\ell\) on \(\varepsilon\) in the appropriate \(C^{r+1}\) topology, and if the required mixed base/parameter bunching inequalities hold up to the relevant total order, then \(h_\varepsilon\) depends \(C^\ell\) on \(\varepsilon\), with regularity determined by those mixed bunching conditions. Without such mixed estimates one should only claim the parameter regularity supplied by the available uniform contraction estimates.

Uniqueness holds among invariant sections lying in the same tube and satisfying the same Lipschitz and cone admissibility bounds.

---

Hirsch, Pugh, and Shub prove the finite-dimensional version of this theorem [2]. In the present manuscript, Theorem 4.1 is the structural HPS input in the Banach-bundle category. The graph transform used in Theorem 4.1 is the full two-sided HPS Hadamard graph transform, not the separate stable-forward/unstable-backward component transform. The component equations alone do not imply invariance; the full HPS admissible matching construction is required. In finite-dimensional fibres, compatibility of the forward and backward base correspondences is part of the HPS graph-transform theorem. For Banach-space invariant-manifold results using the same graph-transform/Perron architecture, see Bates--Lu [4] and Bates--Lu--Zeng [9]. Appendix J records the precise external structural input and verifies the reduction from the tubular Banach-bundle formulation used here. Appendix D proves the one-sided normally attracting Banach-fibre case completely; the two-sided case is supplied by the imported HPS/Banach-space theorem described in Appendix J.

The invariant graph equation has the following transported form. For a section \(h:M\to E\), set

\[
b_{\varepsilon,h}(m):=b_\varepsilon(m,h(m)).
\]

The graph of \(h\) is invariant if and only if

\[
h(b_{\varepsilon,h}(m))
=
g_\varepsilon(m,h(m)).
\]

Transporting both sides to the fibre over \(f(m)\), define

\[
\Psi_\varepsilon(h)(m)
:=
P_{f(m)\leftarrow b_{\varepsilon,h}(m)}
\left[
h(b_{\varepsilon,h}(m))
-
g_\varepsilon(m,h(m))
\right].
\]

Then \(\Psi_\varepsilon(h)\in\Gamma(f^*E)\), and the invariant graph equation is

\[
\Psi_\varepsilon(h)=0.
\]

Using the remainder \(r_\varepsilon\), one obtains

\[
\Psi_\varepsilon(h)
=
\mathcal Ah+\mathcal N_\varepsilon(h),
\]

where

\[
\mathcal Ah=h\circ f-Bh
\]

and

\[
\mathcal N_\varepsilon(h)(m)
=
\Delta_{b_{\varepsilon,h}(m)}^{f(m)}h
-
P_{f(m)\leftarrow b_{\varepsilon,h}(m)}
r_\varepsilon(m,h(m)).
\]

Thus the fixed-point problem is

\[
h=-\mathcal G\mathcal N_\varepsilon(h).
\]

The graph transform acts as a contraction in the \(C^0\) graph metric, not in the Lipschitz norm. The \(C^0\) graph distance is measured by the maximal transported vertical separation after the center coordinates have been matched. This is the metric in which the normal hyperbolicity gap gives contraction. Schematically, after passing to an iterate if necessary, the contraction factor has the form

\[
q
\le
C\left(
e^{-\mathrm{gap}\,N}
+\delta_\varepsilon
+\omega(\rho)
+L
\right),
\]

where the first term comes from the strict normal-hyperbolicity gap and the remaining terms come from perturbation size, tube radius, and cone aperture. Choosing the constants in the order described above gives \(q<1\). The \(C^0\) radius is preserved by an estimate of the form

\[
\|\mathcal H_\varepsilon h\|_{C^0}
\le
C\delta_\varepsilon+q\rho.
\]

After choosing \(q<1\), one chooses \(\delta_\varepsilon\) small enough so that the right-hand side is at most \(\rho\). The Lipschitz bound is preserved separately by the stable/unstable matching estimates, using the strengthened base and fibre derivative bounds on the remainders. Thus the fixed point is obtained in the complete metric space \(\mathcal B_{\rho,L}\) with the \(C^0\) metric, while the admissible-graph estimates ensure that the transform maps \(\mathcal B_{\rho,L}\) into itself.

The Hadamard graph transform should be understood in the two-sided normally hyperbolic sense. In the normally attracting case, the transform is the forward image of a graph, reparametrized over the base. With both stable and unstable directions present, stable components are matched in one time direction and unstable components in the opposite time direction; the center coordinate labels the transformed graph. The admissible-graph preservation estimate comes from the full simultaneous HPS matching construction, not from forward invariance of center cones.

A naive transform that separately matches only the stable component forward and the unstable component backward is insufficient. Affine examples can satisfy those two separate component equations while failing the full graph equation, because the forward and backward base correspondences need not be inverse to one another. The HPS transform avoids this defect by imposing the simultaneous admissible matching whose fixed points are precisely locally invariant graphs.

A contraction in the Lipschitz norm is not available in general. For instance, on \(M=\mathbb T^1\), let \(h\) be a triangular wave of period \(p\). Then \(\operatorname{Lip}(h)=4/p\), while for the shift \(\beta=p/2\), the difference \(h(\cdot+\beta)-h\) has Lipschitz constant \(8/p\). Thus composition by a small base shift need not be small in Lipschitz norm on a Lipschitz ball. This is why the fixed point is taken in the transported \(C^0\) graph metric and the Lipschitz bound is preserved separately by admissible-graph estimates.

Higher regularity follows by lifting the graph transform to jet bundles. For first jets, the principal fibre part is controlled by

\[
\|B_m^s\|\,\|Df(m)^{-1}\|,
\qquad
\|(B_m^u)^{-1}\|\,\|Df(m)\|.
\]

The \(1\)-bunching assumption makes the corresponding fibre transform contractive. Inductively, the \(k\)-jet transform has principal part controlled by

\[
\|B_m^s\|\,\|Df(m)^{-1}\|^k,
\qquad
\|(B_m^u)^{-1}\|\,\|Df(m)\|^k.
\]

The \(k\)-bunching assumption gives contraction on the \(k\)-jet fibres, while lower-order terms depend only on previously constructed jets and on derivatives of \(F_\varepsilon\) up to order \(k\). The \(C^0\) contraction gives the zeroth-order estimate; derivative estimates require these lifted jet contractions.

Thus Theorem 4.1 is the imported HPS mechanism. A fully self-contained proof would require carrying out the Hadamard graph transform and its jet extensions in the stated Banach-bundle category; otherwise one should cite a source that proves this version with the required uniformity.

---

## 5. Fenichel persistence theorem

We now derive the persistence theorem for Banach-space diffeomorphisms.

---

### Theorem 5.1. Persistence of a compact normally hyperbolic invariant manifold

Let \(X\) be a Banach space. Let \(M\subset X\) be a compact finite-dimensional \(C^{r+1}\) embedded submanifold without boundary with a split \(C^{r+1}\) tubular neighbourhood. Let \(F_\varepsilon\) be a family of \(C^{r+1}\) local diffeomorphisms defined on a common neighbourhood of \(M\). Assume that

\[
F_0(M)=M,
\]

and that the invariant splitting

\[
T_mX=T_mM\oplus E_m^s\oplus E_m^u
\]

is normally hyperbolic in the sense of Section 2. Assume also that the normal cocycle satisfies the \(r\)-bunching inequalities.

Then, for all sufficiently small \(\varepsilon\), there exists a locally unique \(C^r\) embedded manifold

\[
M_\varepsilon
\]

near \(M\) such that

\[
F_\varepsilon(M_\varepsilon)=M_\varepsilon.
\]

Moreover:

1. There exists a \(C^r\) embedding

   \[
   K_\varepsilon:M\to X
   \]

   such that

   \[
   M_\varepsilon=K_\varepsilon(M).
   \]

2. There exists a \(C^r\) diffeomorphism

   \[
   f_\varepsilon:M\to M
   \]

   such that

   \[
   F_\varepsilon\circ K_\varepsilon
   =
   K_\varepsilon\circ f_\varepsilon.
   \]

3. If

   \[
   \|F_\varepsilon-F_0\|_{C^r}
   \le
   C|\varepsilon|,
   \]

   then

   \[
   \|K_\varepsilon-i_M\|_{C^r}
   +
   \|f_\varepsilon-f\|_{C^r}
   \le
   C_r|\varepsilon|.
   \]

4. The normal hyperbolicity persists: for every weakened rate compatible with the original strict gap, there exists a persisted invariant splitting

   \[
   T_{M_\varepsilon}X
   =
   TM_\varepsilon\oplus E_\varepsilon^s\oplus E_\varepsilon^u
   \]

   satisfying the corresponding exponential estimates.

5. Uniqueness holds among invariant graphs lying in the prescribed tube and satisfying the prescribed Lipschitz and cone bounds.

---

### Proof

Work in tubular coordinates. By compactness of \(M\), invariance of \(M\) under \(F_0\), and \(C^1\)-closeness of \(F_\varepsilon\) to \(F_0\), we choose the tube so that, for all sufficiently small \(\varepsilon\),

\[
F_\varepsilon(U_E^\rho)\subset U_E^{2\rho},
\]

where \(U_E^\rho\) denotes the tube of radius \(\rho\). This ensures that the graph transform is defined on the chosen class of graphs and that all transported fibre comparisons remain inside the fixed tubular coordinate neighbourhood.

In tubular coordinates,

\[
\widehat F_\varepsilon(m,\eta)
=
\bigl(b_\varepsilon(m,\eta),g_\varepsilon(m,\eta)\bigr).
\]

For \(\varepsilon=0\),

\[
b_0(m,0)=f(m),
\qquad
g_0(m,0)=0,
\]

and the invariant splitting implies

\[
D_\eta b_0(m,0)=0.
\]

Indeed, \(b_0\) is the base component of \(F_0\) in tubular coordinates. The derivative \(D_\eta b_0(m,0)\) is the base component of \(DF_0(m)\) applied to a vertical vector in \(E_m\). Since the invariant splitting gives \(DF_0(m)E_m=E_{f(m)}\), this derivative has no \(TM\)-component.

The normal linear cocycle is

\[
B_m=D_\eta g_0(m,0).
\]

By hypothesis, \(B\) has an exponential dichotomy and satisfies the \(r\)-bunching inequalities. The nonlinear remainder

\[
r_\varepsilon(m,\eta)
=
g_\varepsilon(m,\eta)
-
\tau_{b_\varepsilon(m,\eta)\leftarrow f(m)}
B_m\eta
\]

satisfies the smallness estimates required in Theorem 4.1, because \(F_\varepsilon\) is \(C^1\)-close to \(F_0\) and because

\[
D_\eta b_0(m,0)=0.
\]

The same argument gives

\[
\|D_\eta b_\varepsilon(m,\eta)\|
\le
C\delta_\varepsilon+\omega(\rho)
\]

on the tube. Therefore Theorem 4.1 applies and yields a section

\[
h_\varepsilon\in\Gamma^r(E)
\]

satisfying the graph equation. Define

\[
K_\varepsilon(m):=\Theta(m,h_\varepsilon(m)),
\]

and

\[
M_\varepsilon:=K_\varepsilon(M).
\]

Define

\[
f_\varepsilon(m):=b_\varepsilon(m,h_\varepsilon(m)).
\]

The graph equation gives

\[
F_\varepsilon(K_\varepsilon(m))
=
K_\varepsilon(f_\varepsilon(m)).
\]

Hence

\[
F_\varepsilon(M_\varepsilon)\subset M_\varepsilon.
\]

We next prove equality by proving invariance under the original map, when an iterate was used, and then proving that \(f_\varepsilon\) is onto.

If the bunching assumptions were obtained by replacing \(F_0\) with an iterate \(F_0^N\), Theorem 4.1 gives invariance under \(F_\varepsilon^N\). To obtain invariance under \(F_\varepsilon\), observe that

\[
F_\varepsilon^N(M_\varepsilon)=M_\varepsilon.
\]

Consider \(F_\varepsilon(M_\varepsilon)\). Since \(F_\varepsilon\) commutes with \(F_\varepsilon^N\),

\[
F_\varepsilon^N(F_\varepsilon(M_\varepsilon))
=
F_\varepsilon(F_\varepsilon^N(M_\varepsilon))
=
F_\varepsilon(M_\varepsilon).
\]

For small \(\varepsilon\), \(F_\varepsilon(M_\varepsilon)\) remains in the same admissible tube and satisfies the same Lipschitz and cone bounds. By local uniqueness for \(F_\varepsilon^N\),

\[
F_\varepsilon(M_\varepsilon)=M_\varepsilon.
\]

We prove that \(f_\varepsilon\) is a diffeomorphism. Since \(h_\varepsilon\) is \(C^1\)-small and \(F_\varepsilon\) is \(C^1\)-close to \(F_0\), the map \(f_\varepsilon\) is \(C^1\)-close to \(f\). Therefore

\[
g_\varepsilon:=f^{-1}\circ f_\varepsilon:M\to M
\]

is a \(C^1\) local diffeomorphism sufficiently close to the identity.

We use the following elementary lemma.

---

### Lemma 5.2. Local diffeomorphism close to the identity

Let \(M\) be a compact manifold without boundary. If \(g:M\to M\) is a \(C^1\) local diffeomorphism sufficiently \(C^1\)-close to the identity, then \(g\) is a global \(C^1\) diffeomorphism.

#### Proof

Because \(g\) is a local diffeomorphism, \(g(M)\) is open. Because \(M\) is compact, \(g(M)\) is compact, hence closed. If \(M\) is connected, \(g(M)=M\). If \(M\) is disconnected, the same argument applies componentwise, since \(g\) close to the identity preserves each component. Thus \(g\) is a covering map. Since \(g\) is homotopic to the identity, its covering degree is one componentwise. A degree-one covering is a diffeomorphism. ∎

Applying Lemma 5.2 to \(g_\varepsilon=f^{-1}\circ f_\varepsilon\) shows that \(f_\varepsilon\) is a \(C^r\) diffeomorphism. Hence

\[
F_\varepsilon(M_\varepsilon)
=
K_\varepsilon(f_\varepsilon(M))
=
K_\varepsilon(M)
=
M_\varepsilon.
\]

The quantitative estimate follows from the parameterized version of Theorem 4.1. If

\[
\|F_\varepsilon-F_0\|_{C^r}
\le
C|\varepsilon|,
\]

then

\[
\|h_\varepsilon\|_{C^r}
\le
C_r|\varepsilon|.
\]

Since

\[
K_\varepsilon(m)=\Theta(m,h_\varepsilon(m)),
\]

and \(\Theta\) is \(C^{r+1}\) with uniformly bounded derivatives on the tube,

\[
\|K_\varepsilon-i_M\|_{C^r}
\le
C_r'|\varepsilon|.
\]

Also,

\[
f_\varepsilon(m)=b_\varepsilon(m,h_\varepsilon(m)),
\]

so the chain rule gives

\[
\|f_\varepsilon-f\|_{C^r}
\le
C_r''|\varepsilon|.
\]

These \(C^r\) estimates require uniform contraction estimates for the lifted jet graph transforms. They do not follow from the \(C^0\) graph-transform contraction alone.

If the perturbation admits an expansion

\[
F_\varepsilon
=
F_0+\varepsilon F_1+\cdots+\varepsilon^k F_k
+O(\varepsilon^{k+1})
\]

in the appropriate topology, and if the required parameter-bunching conditions hold, then, in the chosen tubular coordinates,

\[
h_\varepsilon
=
h_0+\varepsilon h_1+\cdots+\varepsilon^k h_k
+O(\varepsilon^{k+1}),
\qquad h_0=0.
\]

Differentiating the invariance equation gives the coefficients \(h_j\) recursively. At each order one solves a linear cohomological equation of the form treated in Theorem 3.1. Appendix F records the abstract expansion argument and the recursive coefficient equations.

We next describe the persistence of the invariant splitting. Straighten \(M_\varepsilon\) by the tubular change of variables

\[
(m,\eta)\mapsto (m,\eta-h_\varepsilon(m)).
\]

In these coordinates, \(M_\varepsilon\) is the zero section. The derivative of \(F_\varepsilon\) along \(M_\varepsilon\) has triangular form

\[
DF_\varepsilon|_{M_\varepsilon}
=
\begin{pmatrix}
Df_\varepsilon & *\\
0 & B_\varepsilon
\end{pmatrix},
\]

where \(B_\varepsilon\) is the perturbed normal cocycle. The cocycle \(B_\varepsilon\) is \(C^0\)-close to \(B\), and \(f_\varepsilon\) is \(C^1\)-close to \(f\). Roughness of exponential dichotomies gives an exponential dichotomy for \(B_\varepsilon\), possibly with weakened rates. Appendix C proves the fixed-base Banach-bundle roughness estimate by a linear half-line Perron argument, and Appendix E gives a direct close-base linear graph-transform proof under the transported block estimates used here; this is the standard roughness theorem of Palmer [6] in the present bundle notation. Equivalently, we obtain the perturbed stable and unstable bundles as invariant graphs of linear maps between the original stable and unstable summands.

More explicitly, if the original estimates involve a strict gap between normal rates and tangent rates, then any slightly weakened rates inside that gap persist. For example, if \(\alpha\) denotes the relevant normal contraction or expansion rate and \(\beta\) denotes the relevant tangent rate, one may choose

\[
\alpha'<\alpha,
\qquad
\beta'>\beta,
\qquad
\alpha'>\beta',
\]

with the required bunching margins. For sufficiently small \(\varepsilon\), the perturbed splitting satisfies the corresponding estimates with \(\alpha'\) and \(\beta'\).

The bundles \(E_\varepsilon^s\) and \(E_\varepsilon^u\) are generally continuous under the basic hypotheses. Higher regularity of these bundles requires additional bunching assumptions and should not be inferred solely from the \(C^r\) regularity of \(M_\varepsilon\).

Theorem 4.1 gives local uniqueness among admissible graphs. If one wants uniqueness among all sufficiently \(C^1\)-close invariant manifolds, one must first show that every such manifold lies in the admissible class. This is usually true for manifolds whose tangent spaces remain inside the prescribed center cones in tubular coordinates, but the theorem’s intrinsic uniqueness statement is the qualified admissible-graph uniqueness above. ∎

**Remark.** Another common proof strategy constructs local center-stable and center-unstable manifolds and obtains the normally hyperbolic manifold as their transverse intersection,

\[
M_\varepsilon
=
W^{cs}_{\mathrm{loc}}\cap W^{cu}_{\mathrm{loc}}.
\]

That approach is equivalent in spirit but requires separate hypotheses and constructions for the two larger invariant manifolds. We do not use it in the proof above.


---

### Corollary 5.3. Conditional nonlinear regularity spectrum

Let \(s_*\) be the linear regularity spectrum defined in Appendix K. Suppose that the imported HPS invariant-section theorem is available in the Hölder class \(C^{k,\alpha}\), and that the nonlinear maps \(F_\varepsilon\) have the regularity and tame estimates required by that Hölder invariant-section theorem. Then the invariant section \(h_\varepsilon\) has regularity \(C^{k,\alpha}\) whenever

\[
k+\alpha<s_*
\]

and the coefficients have the required regularity.

If an integer order \(k\) is obstructed by a periodic jet resonance in the sense of Appendix K, then the linearized cohomological operator is not onto on \(C^k\). In that case one cannot expect a uniform \(C^k\) implicit-function-theorem proof of the invariance equation, although special nonlinear perturbations may still admit special solutions.

---

## 6. Stable and unstable fibres

We now construct strong stable and strong unstable fibres. These constructions require rate-gap assumptions that are stronger than those required for persistence of the manifold alone.

Let \(p\in M_\varepsilon\), and write

\[
p_n=F_\varepsilon^n(p).
\]

The linearized dynamics along the orbit is

\[
A_n:=DF_\varepsilon(p_n).
\]

The splitting along \(M_\varepsilon\) gives

\[
T_{p_n}X
=
T_{p_n}M_\varepsilon
\oplus
E^s_{\varepsilon,p_n}
\oplus
E^u_{\varepsilon,p_n}.
\]

To construct the strong stable fibre, group the directions as

\[
T_{p_n}X
=
E^s_{\varepsilon,p_n}
\oplus
E^{cu}_{\varepsilon,p_n},
\]

where

\[
E^{cu}_{\varepsilon,p_n}
:=
T_{p_n}M_\varepsilon
\oplus
E^u_{\varepsilon,p_n}.
\]

Assume that there exist constants \(C>0\), \(\alpha_s>0\), and \(\beta_{cu}\ge0\) such that

\[
\|\Phi_\varepsilon^s(n,k)\|
\le
C e^{-\alpha_s(n-k)},
\qquad
n\ge k,
\]

and

\[
\|\Phi_\varepsilon^{cu}(n,k)\|
\le
C e^{\beta_{cu}(k-n)},
\qquad
n\le k.
\]

Assume the strong stable gap condition

\[
\beta_{cu}<\alpha_s.
\]

---

### Theorem 6.1. Strong stable fibres

Under the above assumptions, there exists a local strong stable fibre

\[
W^s_{\mathrm{loc}}(p)
\]

through \(p\), tangent to \(E^s_{\varepsilon,p}\) at \(p\). The fibre is parametrized by a neighbourhood of the origin in \(E^s_{\varepsilon,p}\). Points in \(W^s_{\mathrm{loc}}(p)\) remain near the orbit of \(p\) for forward time and converge to it exponentially.

---

### Proof

Work in coordinates straightened along \(M_\varepsilon\). A nearby orbit is written as

\[
p_n+\xi_n,
\]

with

\[
\xi_n=\xi_n^s+\xi_n^{cu},
\]

where

\[
\xi_n^s\in E^s_{\varepsilon,p_n},
\qquad
\xi_n^{cu}\in E^{cu}_{\varepsilon,p_n}.
\]

The nonlinear variational equation has the form

\[
\xi_{n+1}
=
A_n\xi_n+R_n(\xi_n),
\]

where

\[
R_n(0)=0,
\qquad
DR_n(0)=0.
\]

Shrinking the coordinate neighbourhood if necessary, the \(C^{r+1}\) regularity of \(F_\varepsilon\) gives uniform estimates

\[
\|R_n(\xi)\|\le C\|\xi\|^2,
\qquad
\|DR_n(\xi)\|\le C\|\xi\|
\]

for small \(\xi\), uniformly in \(n\) and \(p\in M_\varepsilon\).

Choose \(\gamma\) such that

\[
\beta_{cu}<\gamma<\alpha_s.
\]

Define the weighted Banach space

\[
\ell_\gamma^+
:=
\left\{
(\xi_n)_{n\ge0}:
\|\xi\|_\gamma
:=
\sup_{n\ge0}e^{\gamma n}\|\xi_n\|
<\infty
\right\}.
\]

For \(a\in E^s_{\varepsilon,p_0}\), define the Perron operator \(\mathcal P_a\) by

\[
(\mathcal P_a\xi)_n
=
(\mathcal P_a\xi)_n^s
+
(\mathcal P_a\xi)_n^{cu},
\]

where

\[
(\mathcal P_a\xi)_n^s
=
\Phi_\varepsilon^s(n,0)a
+
\sum_{k=0}^{n-1}
\Phi_\varepsilon^s(n,k+1)
P^s_{k+1}R_k(\xi_k),
\]

and

\[
(\mathcal P_a\xi)_n^{cu}
=
-
\sum_{k=n}^{\infty}
\Phi_\varepsilon^{cu}(n,k+1)
P^{cu}_{k+1}R_k(\xi_k).
\]

The center component is not frozen in this construction. It belongs to \(\xi_n^{cu}\), and the future boundary condition determines it together with the unstable component. Thus the Perron operator solves simultaneously for the stable displacement, the center displacement, and the unstable displacement relative to the reference orbit.

Let

\[
B_r:=\{\xi\in\ell_\gamma^+:\|\xi\|_\gamma\le r\}.
\]

For the stable homogeneous term,

\[
e^{\gamma n}\|\Phi_\varepsilon^s(n,0)a\|
\le
C e^{-(\alpha_s-\gamma)n}\|a\|
\le
C\|a\|.
\]

If \(\|\xi\|_\gamma\le r\), then

\[
\|\xi_k\|\le r e^{-\gamma k}.
\]

Since \(R_k(\xi_k)=O(\|\xi_k\|^2)\),

\[
\|R_k(\xi_k)\|
\le
C r^2 e^{-2\gamma k}.
\]

The stable convolution satisfies

\[
e^{\gamma n}
\left\|
\sum_{k=0}^{n-1}
\Phi_\varepsilon^s(n,k+1)
P^s_{k+1}R_k(\xi_k)
\right\|
\le
C r^2,
\]

because \(\gamma<\alpha_s\).

For the center-unstable part,

\[
e^{\gamma n}
\left\|
\sum_{k=n}^{\infty}
\Phi_\varepsilon^{cu}(n,k+1)
P^{cu}_{k+1}R_k(\xi_k)
\right\|
\]

is bounded by

\[
C r^2 e^{\gamma n}
\sum_{k=n}^{\infty}
e^{\beta_{cu}(k+1-n)}e^{-2\gamma k}.
\]

Writing \(k=n+j\), this becomes

\[
C r^2 e^{-\gamma n}
\sum_{j=0}^{\infty}
e^{(\beta_{cu}-2\gamma)j}.
\]

Since \(\beta_{cu}<\gamma\), the series converges uniformly. Thus

\[
\|\mathcal P_a\xi\|_\gamma
\le
C\|a\|+C r^2.
\]

Choosing \(r\) small and \(\|a\|\le c r\) with \(c\) sufficiently small yields

\[
\mathcal P_a(B_r)\subset B_r.
\]

For \(\xi,\eta\in B_r\),

\[
R_k(\xi_k)-R_k(\eta_k)
=
O(r)\|\xi_k-\eta_k\|.
\]

The same convolution estimates give

\[
\|\mathcal P_a\xi-\mathcal P_a\eta\|_\gamma
\le
C r\|\xi-\eta\|_\gamma.
\]

Choosing \(r\) small gives \(Cr<1\). Therefore \(\mathcal P_a\) is a contraction on \(B_r\). By the Banach fixed point theorem, there exists a unique fixed point \(\xi(a)\in B_r\).

Define

\[
W^s_{\mathrm{loc}}(p)
:=
\left\{
p+\xi_0(a):
a\in E^s_{\varepsilon,p},
\ \|a\|\text{ sufficiently small}
\right\}.
\]

This gives the desired local strong stable fibre. ∎

Appendix B records the same half-line Perron construction as a standalone theorem, including the self-map estimate, contraction estimate, tracking estimate, tangency, and unstable analogue.

**Remark on non-reflexive ambient spaces.** The half-line Perron construction uses only completeness of the weighted sequence space and uniform contraction estimates. It does not require reflexivity of the ambient Banach space or weak compactness of bounded sets. This observation concerns the construction and internal regularity of individual leaves. Transverse regularity of the family of leaves and regularity of the phase projection remain separate questions requiring additional bunching assumptions.

---

### 6.1. Stable manifold, phase projection, and tracking

Iteration extends the local stable fibres globally, provided the orbits remain in the tube in which the construction is valid. Define

\[
W^s(M_\varepsilon)
=
\left\{
y:
F_\varepsilon^n(y)\text{ remains near }M_\varepsilon
\text{ for all }n\ge0
\text{ and approaches }M_\varepsilon
\right\}.
\]

Locally,

\[
W^s(M_\varepsilon)
=
\bigcup_{p\in M_\varepsilon}
W^s_{\mathrm{loc}}(p).
\]

The invariance property is

\[
F_\varepsilon(W^s(M_\varepsilon))
\subset
W^s(M_\varepsilon).
\]

If \(F_\varepsilon\) is a diffeomorphism and the relevant inverse iterates remain in the domain where the stable manifold is defined, this inclusion becomes equality on the corresponding global stable set. The unstable manifold \(W^u(M_\varepsilon)\) is defined analogously using backward iteration.

The stable fibres define an asymptotic phase projection

\[
\pi^s:W^s_{\mathrm{loc}}(M_\varepsilon)\to M_\varepsilon.
\]

If \(y\in W^s_{\mathrm{loc}}(M_\varepsilon)\), then \(\pi^s(y)\) is the unique point in \(M_\varepsilon\) whose orbit is asymptotic to the orbit of \(y\). For \(n\ge0\),

\[
\operatorname{dist}
\left(
F_\varepsilon^n(y),
F_\varepsilon^n(\pi^s(y))
\right)
\le
C e^{-\gamma n}
\operatorname{dist}(y,M_\varepsilon).
\]

The regularity of \(\pi^s\) is a separate question and requires its own bunching assumptions. Appendix H gives the precise globalization by iteration, including the domain assumptions, invariance, phase projection, and tracking after entry into the local stable tube.

---

### 6.2. Regularity of stable leaves

We distinguish four regularity questions:

1. regularity of each stable leaf in its internal coordinate;
2. regularity of the leaf as a function of the base point \(p\in M_\varepsilon\);
3. regularity of the asymptotic phase projection

   \[
   \pi^s:W^s_{\mathrm{loc}}(M_\varepsilon)\to M_\varepsilon;
   \]

4. regularity of the total lamination.

We obtain internal regularity of the stable leaves by differentiating the Perron operator with respect to the fibre coordinate \(a\). For \(C^\ell\) internal regularity, one requires the strong stable bunching condition

\[
\alpha_s>\ell\,\beta_{cu},
\]

or, more invariantly, contractivity of the induced \(\ell\)-jet Perron operator. The nonlinear Faà di Bruno terms are controlled by lower-order derivatives in the induction.

The dependence on \(p\) is generally weaker because the reference orbit \(p_n=F_\varepsilon^n(p)\) enters the Perron operator. Under basic normal hyperbolicity the stable foliation is typically continuous, and often Hölder, transversely. Higher transverse regularity and regularity of \(\pi^s\) require separate bunching assumptions. In particular, the full stable foliation is not automatically \(C^r\) transversely.

---

### 6.3. Strong unstable fibres

We obtain the strong unstable fibres by applying the preceding construction to \(F_\varepsilon^{-1}\). One groups the tangent directions as

\[
T_{p_n}X
=
E^u_{\varepsilon,p_n}
\oplus
E^{cs}_{\varepsilon,p_n},
\]

where

\[
E^{cs}_{\varepsilon,p_n}
:=
T_{p_n}M_\varepsilon
\oplus
E^s_{\varepsilon,p_n}.
\]

Assume that the backward unstable evolution contracts with rate \(\alpha_u>0\), while the backward growth of the center-stable complement is bounded by \(\beta_{cs}\), with

\[
\beta_{cs}<\alpha_u.
\]

The Perron construction on negative time then gives local strong unstable fibres

\[
W^u_{\mathrm{loc}}(p),
\]

tangent to \(E^u_{\varepsilon,p}\) at \(p\). Equivalently, for \(b\in E^u_{\varepsilon,p}\), one solves a negative-time Perron equation of the form

\[
\xi_{n-1}
=
A_{n-1}^{-1}\xi_n
+
\widetilde R_n(\xi_n),
\qquad n\le0,
\]

in a weighted space as \(n\to-\infty\). Internal and transverse regularity require the unstable analogues of the stable bunching assumptions.

---

## 7. Flows

Let \(\Phi_t^\varepsilon\) be a genuine \(C^{r+1}\) local flow defined for positive and negative time on a neighbourhood of \(M\). Assume that the unperturbed flow leaves \(M\) invariant for all time:

\[
\Phi_t^0(M)=M,
\qquad
t\in\mathbb R.
\]

Choose \(T>0\) large enough that the time-\(T\) map

\[
F_\varepsilon:=\Phi_T^\varepsilon
\]

satisfies the hypotheses of Theorem 5.1. Applying Theorem 5.1 gives a manifold \(M_\varepsilon\) invariant under \(F_\varepsilon\).

For \(0\le t\le T\), define

\[
N_t:=\Phi_t^\varepsilon(M_\varepsilon).
\]

Because the flow maps commute,

\[
F_\varepsilon(N_t)
=
\Phi_T^\varepsilon\Phi_t^\varepsilon(M_\varepsilon)
=
\Phi_t^\varepsilon\Phi_T^\varepsilon(M_\varepsilon)
=
N_t.
\]

Thus \(N_t\) is invariant under the time-\(T\) map. For sufficiently small \(\varepsilon\), and uniformly for \(t\in[0,T]\), the manifold \(N_t\) remains in the same admissible tube and satisfies the same Lipschitz and cone bounds. This follows from the continuity of the flow in \(t\) and the \(C^1\)-closeness of \(\Phi_t^\varepsilon\) to \(\Phi_t^0\) on compact time intervals. By local uniqueness,

\[
N_t=M_\varepsilon.
\]

Therefore,

\[
\Phi_t^\varepsilon(M_\varepsilon)=M_\varepsilon,
\qquad
0\le t\le T.
\]

By the flow property, invariance extends to all \(t\in\mathbb R\). Appendix G records this time-\(T\) reduction as a standalone lemma.

In continuous time, the strong stable Perron operator for the deviation equation

\[
\dot\xi(t)=A(t)\xi(t)+R(t,\xi(t))
\]

is

\[
\xi^s(t)
=
\Phi^s(t,0)a
+
\int_0^t
\Phi^s(t,s)P^s(s)R(s,\xi(s))\,ds,
\]

and

\[
\xi^{cu}(t)
=
-
\int_t^\infty
\Phi^{cu}(t,s)P^{cu}(s)R(s,\xi(s))\,ds.
\]

The same rate-gap condition is required: the stable decay rate must dominate the backward growth rate of the center-unstable complement.

If one only knows that \(\Phi_T^0(M)=M\), but not that \(\Phi_t^0(M)=M\) for all \(t\), then \(\Phi_t^0(M)\) for \(0<t<T\) need not remain close to \(M\). In that case \(N_t=\Phi_t^\varepsilon(M_\varepsilon)\) may fail to lie in the admissible tube around \(M\), so the uniqueness argument for the time-\(T\) graph transform cannot be applied. Thus the time-map reduction requires full-flow invariance, unless one constructs the invariant manifold directly by a continuous-time Lyapunov--Perron method.

---

## 8. Extensions

The compact invertible theorem serves as the model case. The same architecture extends to several broader classes of systems. In each case we replace the discrete Green operator by the appropriate linear inverse and adapt the function spaces to the dynamics. The subsections below state the required modifications and proof architecture; each extension requires its own theorem-level hypotheses.

Without additional hypotheses, the compact invertible theorem does not cover:

1. noninvertible parabolic semiflows;
2. unbounded linear generators;
3. noncompact invariant manifolds;
4. Banach-dimensional invariant manifolds;
5. delay equations;
6. random or nonautonomous cocycles;
7. quasilinear equations with derivative loss;
8. manifolds with boundary;
9. transverse \(C^r\) regularity of stable or unstable foliations without additional bunching.

The following table summarizes the replacements used in the extension settings.

| Setting | Linear inverse | Function space | Additional hypothesis |
|---|---|---|---|
| Compact invertible map | discrete Green operator | \(C^k(M,E)\) | bunching |
| Noncompact finite-dimensional manifold | discrete Green operator with uniform constants | \(C_b^k(M,E)\) | bounded geometry |
| Banach-dimensional manifold | discrete Green operator on Banach bundles | \(C_b^k(M,E)\) | split tubular neighbourhood, adapted metric |
| Parabolic semiflow | analytic semigroup Perron integral | weighted mild-solution spaces | sectorial dichotomy, smoothing |
| Random cocycle | random Green operator | tempered weighted spaces | random or tempered dichotomy |
| Quasilinear PDE | tame or maximal-regularity inverse | scales \(X_s\) | derivative recovery or Nash–Moser |

---

### 8.1. Finite-dimensional singular perturbations

In finite-dimensional singular perturbation problems one often considers

\[
\begin{aligned}
\dot x &= f(x,y,\varepsilon),\\
\dot y &= \varepsilon g(x,y,\varepsilon).
\end{aligned}
\]

The critical manifold is

\[
M_0=\{(x,y):f(x,y,0)=0\}.
\]

Normal hyperbolicity of \(M_0\) means that the fast linearization \(D_xf(x,y,0)\) has spectrum bounded away from the imaginary axis. If \(M_\varepsilon\) is written as a graph

\[
x=h_\varepsilon(y),
\]

then the reduced equation on \(M_\varepsilon\) is exactly

\[
\dot y=\varepsilon g(h_\varepsilon(y),y,\varepsilon).
\]

Approximate reduced equations arise only after expanding \(h_\varepsilon\) in powers of \(\varepsilon\). For example, if \(h_\varepsilon=h_0+O(\varepsilon)\), then

\[
\dot y
=
\varepsilon g(h_0(y),y,0)+O(\varepsilon^2).
\]

---

### 8.2. Parabolic semiflows

Let \(A\) be a sectorial operator on a Banach space \(X_0\), and let

\[
X_1\hookrightarrow X_\theta\hookrightarrow X_0
\]

be an interpolation scale, with \(X_1=D(A)\). Since \(A\) is sectorial on \(X_0\), it generates an analytic semigroup. In an interpolation scale one has estimates of the form

\[
\|e^{At}\|_{\mathcal L(X_0,X_\theta)}
\le
C t^{-\theta}e^{at},
\qquad t>0.
\]

These smoothing estimates are part of the functional framework and replace the bounded-map estimates used in the compact invertible theorem. Unlike the compact invertible map setting, the vector field is typically not a bounded \(C^r\) vector field on the base phase space, and the time-\(t\) maps are not local Banach-space diffeomorphisms. Unstable directions must therefore be handled through backward solvability of the unstable linear cocycle, not by inverting the full semiflow. Consider a semilinear parabolic fast-slow system of the form

\[
\begin{aligned}
u_t &= Au+f(u,v,\varepsilon),\\
v_t &= \varepsilon g(u,v,\varepsilon),
\end{aligned}
\]

where \(u\in X_0\) is the fast variable and \(v\in Y\) is the slow variable.

Assume that the critical manifold is a graph

\[
M_0=\{(h_0(v),v):v\in Y_0\},
\]

and that the fast linearization

\[
L_v=A+D_u f(h_0(v),v,0)
\]

generates a uniformly exponentially dichotomous analytic semigroup. In particular, spectral separation alone is not sufficient. One requires uniform semigroup estimates, uniformly bounded dichotomy projections, and uniform resolvent bounds. A typical sufficient hypothesis is a uniform resolvent estimate: for some \(\eta>0\),

\[
\sup_{v\in Y_0}
\sup_{\operatorname{Re}\lambda\ge -\eta}
\|(\lambda-L_v)^{-1}\|_{\mathcal L(X_0)}
<\infty,
\]

together with uniform bounds on the associated spectral or dichotomy projections.

The Perron operator is formulated in weighted mild-solution spaces such as

\[
C_\gamma([0,\infty),X_\theta)
:=
\left\{
\eta:
\|\eta\|_\gamma
=
\sup_{t\ge0}e^{\gamma t}\|\eta(t)\|_{X_\theta}
<\infty
\right\}.
\]

For a stable coordinate \(a\), the stable and unstable components are given by

\[
\eta^s(t)
=
e^{L^s t}a
+
\int_0^t
e^{L^s(t-s)}P^sR(s,\eta(s))\,ds,
\]

and

\[
\eta^u(t)
=
-
\int_t^\infty
e^{L^u(t-s)}P^uR(s,\eta(s))\,ds.
\]

The unstable integral is meaningful only on a backward well-posed unstable subspace. In many parabolic applications the unstable space is finite-dimensional, so backward evolution on that subspace is well-defined. In purely normally attracting problems, the unstable term is absent and the construction simplifies.

The analytic smoothing estimates give convolution bounds of the form

\[
\sup_{t\ge0}
e^{\gamma t}
\int_0^t
(t-s)^{-\rho}
e^{-\alpha(t-s)}
e^{-\gamma s}\,ds
<\infty,
\]

provided

\[
\gamma<\alpha,
\qquad
\rho<1.
\]

Under the corresponding bunching assumptions, the fixed point gives a slow manifold

\[
M_\varepsilon=\{(h_\varepsilon(v),v):v\in Y_0\},
\]

and the reduced equation on \(M_\varepsilon\) is exactly

\[
v_t=\varepsilon g(h_\varepsilon(v),v,\varepsilon).
\]

For detailed treatments in this direction, see Henry [5] and Chow, Lin, and Lu [3].

---

### 8.3. Noncompact finite-dimensional manifolds

Let \(M\) be a complete finite-dimensional \(C^{r+1}\) manifold with bounded geometry. Bounded geometry may be taken to include a positive injectivity radius, uniformly bounded curvature and covariant derivatives up to the required order, a uniformly controlled bundle atlas, a uniform tubular radius, uniformly bounded bundle projections, and uniformly bounded derivatives of \(f\), \(f^{-1}\), \(B\), and the nonlinear terms. Assume uniform exponential dichotomy estimates and uniform bunching constants. Appendix I proves the corresponding noncompact uniform cohomological inverse theorem in \(C_b^k\) spaces.

Replace \(C^k(M,E)\) by bounded uniformly continuous section spaces \(C_b^k(M,E)\). The admissible class

\[
\mathcal B_{\rho,L}
=
\left\{
h\in C_b^0(M,E):
\|h\|_{C^0}\le\rho,
\ \operatorname{Lip}(h)\le L
\right\}
\]

is complete in the \(C^0\) metric. The graph transform is defined globally using the uniform cone fields, and the contraction estimates are uniform in the base point.

For global invariance one must ensure that orbits remain in the region where the tube and estimates are valid. Common hypotheses are: global definition and uniform closeness on the relevant region; a cutoff outside a controlled neighbourhood; a local theorem combined with continuation while the orbit remains in the tube; or inflowing/overflowing invariance when a boundary is present.

If \(M\) has boundary, one must impose inflowing or overflowing invariance conditions, or introduce a localized cutoff.

---

### 8.4. Manifolds with boundary

If \(M\) has boundary, ordinary invariance may fail at the boundary. In that case we distinguish several notions:

1. local invariance away from the boundary;
2. inflowing invariance, where trajectories enter the manifold through part of the boundary;
3. overflowing invariance, where trajectories leave the manifold through part of the boundary;
4. invariance after cutting off the vector field outside a prescribed region.

Persistence theorems for manifolds with boundary require boundary-compatible hyperbolicity conditions and a precise choice of one of these invariance notions.

---

### 8.5. Banach-dimensional invariant manifolds

Let \(M\) itself be a Banach manifold, and assume that the tangent bundle is split:

\[
T_mX=T_mM\oplus N_m,
\]

with \(N_m\) complemented. Unlike the finite-dimensional case, a tubular neighbourhood theorem is not automatic for arbitrary Banach submanifolds. One should assume explicitly that \(M\) is a split submanifold, the normal bundle is complemented, and the tubular chart and its inverse have uniformly bounded derivatives up to the required order. In Hilbert spaces this is natural, since orthogonal complements are available.

The proof then proceeds in bounded section spaces \(C_b^k(M,N)\). Bunching is formulated in an adapted Finsler metric. The adapted metric must be uniformly equivalent to the original Banach norm, or the equivalence constants must be tracked explicitly. For \(C^r\) regularity on Banach bases, one must control the jet or difference-quotient theory in uniformly bounded charts. The main complications are lack of local compactness, possible absence of smooth partitions of unity, derivative loss in composition operators, and the need for uniform transition-map estimates. The Hirsch–Pugh–Shub section theorem applies with uniform constants.

---

### 8.6. Random and nonautonomous cocycles

Let \((\Omega,\mathcal F,\mathbb P,\theta)\) be a metric or measurable dynamical system, and let

\[
F_\varepsilon(\omega,\cdot):X\to X
\]

be a random cocycle. Assume that the normal linear cocycle \(B(\omega)\) admits a random exponential dichotomy, either uniform or tempered. In the tempered case the dichotomy estimates take the form

\[
\|\Phi^s(\omega,n)\|
\le
C(\omega)e^{-\alpha n},
\qquad
\|\Phi^u(\omega,-n)\|
\le
C(\omega)e^{-\alpha n},
\]

where \(C(\omega)\) is tempered. The Perron map is then defined on tempered weighted spaces whose norms depend on \(\omega\). The Perron operator is defined pathwise, and the fixed point yields a random invariant section

\[
h_\varepsilon(\omega,\cdot).
\]

Cocycle invariance takes the form

\[
F_\varepsilon
\left(
\omega,
\operatorname{graph}(h_\varepsilon(\omega))
\right)
=
\operatorname{graph}
\left(
h_\varepsilon(\theta\omega)
\right).
\]

Measurability follows from measurable selection or from convergence of measurable iterates. In infinite-dimensional random settings, the multiplicative ergodic theorem may be used to verify the dichotomy under compactness or quasi-compactness assumptions; see Ruelle [7]. In Banach spaces this typically also requires measurability of projections and integrability of logarithmic growth. In many applications one assumes the random dichotomy directly and uses the multiplicative ergodic theorem only as a verification tool. Pathwise regularity follows from the same jet-extension argument, provided the bunching inequalities hold pathwise or in a tempered sense. Measurable or \(L^p\) dependence on \(\omega\) requires additional estimates.

---

### 8.7. Quasilinear equations and derivative loss

For quasilinear equations of the form

\[
u_t=A(u)u+f(u),
\]

the linearized operator depends on the solution and may lose derivatives. One works in a scale of Banach spaces \(\{X_s\}_{s\ge0}\), with

\[
X_{s+\sigma}\hookrightarrow X_s.
\]

The invariant graph is sought in a stronger space \(X_{s+\sigma}\), while residuals are estimated in \(X_s\). A typical tame estimate has the form

\[
\|F(h)\|_s
\le
C_s(1+\|h\|_{s+\sigma}),
\]

while the linear inverse may satisfy a loss estimate

\[
\|\mathcal Gq\|_s
\le
C_s\|q\|_{s+\sigma}.
\]

If parabolic smoothing or maximal regularity recovers the lost derivatives, the Perron method applies directly. For quasilinear parabolic equations, maximal regularity often replaces the elementary semigroup estimate. One may work in spaces such as

\[
L^p(0,T;X_1)\cap W^{1,p}(0,T;X_0),
\]

or in Hölder spaces adapted to the interpolation scale. If smoothing is unavailable, a Nash–Moser scheme may be required; see Hamilton [8]. In such a scheme, the linearized operator has a tame inverse with derivative loss, the nonlinear remainder is tame, smoothing operators are inserted at each Newton step, tame estimates control the loss, and convergence is obtained in a lower regularity category.

An alternative formulation uses topological jets or difference quotients. The principal jet cocycle is

\[
J\mapsto B_mJ\circ(Df_m^{-1})^{\otimes k},
\]

and the bunching assumptions control its growth.

---

### 8.8. Delay equations

Delay equations may be formulated as semiflows or cocycles on history spaces, for example

\[
X=C([-\tau,0],\mathbb R^d),
\]

or the corresponding Banach-valued history space. The linearized delay equation induces a linear cocycle on the history space. If that cocycle admits an exponential dichotomy satisfying the appropriate bunching assumptions, the same Perron and invariant-section machinery applies.


---

## 9. Open problems and spectral directions

The preceding sections separate proved modules, structural inputs, and conditional extensions. Several natural problems remain open or are deliberately left as future directions.

1. **A self-contained two-sided Banach-bundle HPS theorem.** The full two-sided Hadamard matching theorem is used here as an external HPS/Banach structural input. A self-contained proof in the precise Banach-bundle category of this manuscript would require a complete admissible matching lemma, transported \(C^0\) graph contraction, Lipschitz preservation, and jet or difference-quotient extension. Appendix D proves the one-sided attracting case, but the two-sided case remains a separate nonlinear problem.

2. **Converse fractional spectrum theorem.** Appendix K proves that

   \[
   \widehat\rho_{k,\alpha}<1
   \]

   implies boundedness of the Green inverse on \(C^{k,\alpha}\), and it gives periodic resonance obstructions to \(C^k\)-surjectivity. A natural converse problem is to characterize when bounded invertibility of the Green operator forces a subunit fractional Green-summand radius, or to identify cancellations that permit bounded inversion at borderline radii.

3. **Transverse lamination and phase regularity.** The Perron construction gives internal regularity of individual strong leaves under strong stable or unstable bunching. The transverse regularity of the family of leaves, and the regularity of the asymptotic phase map, require separate estimates. A central problem is to characterize those transverse regularity thresholds in terms of integer bunching or fractional jet spectra.

4. **Spectral interpretation of the Green-summand radii.** The fractional radii in Appendix K are defined by exact Green summand operator norms on Hölder jet sections. It would be useful to relate these radii to Mather, Sacker--Sell, or evolution-semigroup spectra of the induced weighted-shift operators under precise hypotheses. Such a relation should be treated as an additional spectral theorem, not as a replacement for the estimates proved here.

5. **Nonlinear Hölder persistence at fractional thresholds.** Corollary 5.3 is conditional on the availability of an HPS invariant-section theorem in the relevant Hölder category. A full nonlinear theorem combining the fractional cohomological inverse with a Hölder HPS graph transform would identify when the linear regularity spectrum controls the regularity of the persisted NHIM itself.

6. **Extension theorems beyond the compact invertible model.** Section 8 records extension architectures for parabolic semiflows, random cocycles, delay equations, quasilinear problems, Banach-dimensional bases, and noncompact manifolds. Each setting requires its own theorem-level hypotheses: semigroup smoothing, tempered dichotomies, bounded geometry, history-space dichotomies, or tame/Nash--Moser estimates.

---

## 10. Summary

The proof of the compact invertible persistence theorem follows the chain

\[
\text{exponential dichotomy}
\Longrightarrow
\text{linear cohomological inverse}
\Longrightarrow
\text{invariant-section theorem}
\Longrightarrow
\text{persisted normally hyperbolic manifold}
\Longrightarrow
\text{stable and unstable fibres}.
\]

The ambient phase space may be infinite-dimensional. The base manifold is finite-dimensional and compact in the main theorem. Appendix A supplies a self-contained proof of the smooth-splitting version of the \(C^k\) cohomological inverse theorem, Appendix B supplies a self-contained half-line Perron proof of the local strong-fibre theorem, Appendix C proves the fixed-base roughness of exponential dichotomies in Banach bundles, Appendix D proves the one-sided normally attracting Banach-bundle graph transform, Appendix E proves close-base roughness under transported block estimates, Appendix F proves the parameter-expansion recursion, Appendix G proves the time-map reduction for flows, Appendix H proves the globalization of local stable fibres under explicit domain assumptions, Appendix I proves the uniform noncompact cohomological inverse theorem, Appendix J records the external two-sided HPS input and the reduction to the tubular formulation, and Appendix K gives the fractional jet-spectrum regularity theorem and periodic resonance obstruction. We obtain extensions to parabolic semiflows, noncompact manifolds, Banach-dimensional manifolds, random cocycles, delay equations, and quasilinear problems by replacing the discrete Green operator with the appropriate Perron or tame inverse and by adapting the function spaces to the dynamics.


---

## Appendix A. The \(C^k\) Banach-bundle cohomological inverse theorem

This appendix gives a self-contained proof of the linear \(C^k\) inverse theorem under a clean regularity hypothesis on the splitting. The continuous-projection version used in the HPS difference-quotient setting is obtained by replacing the covariant derivative computations below with transported difference quotients.

### A.1. Statement

Let \(M\) be a compact finite-dimensional \(C^{r+1}\) manifold, let \(E\to M\) be a \(C^{r+1}\) Banach bundle, and let \(f\in\operatorname{Diff}^{r+1}(M)\). Let

\[
B_m:E_m\to E_{f(m)}
\]

be a \(C^r\) bundle automorphism preserving a \(C^r\) splitting

\[
E=E^s\oplus E^u.
\]

Assume that the projections onto \(E^s\) and \(E^u\) are \(C^r\) and uniformly bounded. Assume that \(B\) has an exponential dichotomy and that, for every \(0\le k\le r\), there are constants \(C_k>0\) and \(\theta_k\in(0,1)\) such that

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m_n)\|^k
\le
C_k\theta_k^n,
\qquad n\ge0,
\]

and

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|^k
\le
C_k\theta_k^n,
\qquad n\ge0.
\]

Then, for every \(0\le k\le r\), the operator

\[
\mathcal A:\Gamma^k(E)\to\Gamma^k(f^*E),
\qquad
(\mathcal A\zeta)(m)=\zeta(f(m))-B_m\zeta(m),
\]

is an isomorphism and

\[
\|\mathcal A^{-1}q\|_{C^k}
\le
C_k'\|q\|_{C^k}.
\]

The \(C^k\) norms may be defined using a fixed \(C^r\) connection or a finite bundle atlas. Compactness of \(M\) and boundedness of the transition maps make the resulting norms equivalent.

### A.2. The \(C^0\) inverse

The \(C^0\) inverse is the Green operator constructed in Section 3. Along an orbit \(m_n=f^n(m)\), the equation becomes

\[
\zeta_{n+1}-B_{m_n}\zeta_n=q_n,
\qquad q_n\in E_{m_{n+1}}.
\]

Decompose the forcing in the target fibre:

\[
q_n^\sigma=P_{m_{n+1}}^\sigma q_n.
\]

Then

\[
\zeta_n^s
=
\sum_{j=-\infty}^{n-1}
\Phi^s(n,j+1)q_j^s,
\]

and

\[
\zeta_n^u
=
-
\sum_{j=n}^{\infty}
\Phi^u(n,j+1)q_j^u.
\]

The exponential dichotomy gives absolute and uniform convergence and

\[
\|\zeta\|_{C^0}\le C\|q\|_{C^0}.
\]

The same formulas show \(\mathcal A\zeta=q\). A bounded homogeneous solution has zero stable part by letting the initial time tend to \(-\infty\), and zero unstable part by letting the terminal time tend to \(+\infty\). Hence the bounded solution is unique.

### A.3. First derivatives

Use the fixed connection to write covariant derivatives. Differentiating

\[
\zeta(f(m))-B_m\zeta(m)=q(m)
\]

gives, in local bundle coordinates,

\[
D\zeta(f(m))Df(m)-B_mD\zeta(m)=Dq(m)+D_mB(m)\zeta(m)+L_1(m)\zeta(m),
\]

where \(L_1\) denotes connection terms with uniformly bounded coefficients. These terms are lower order. With

\[
J(m)=D\zeta(m),
\]

the equation becomes

\[
J(f(m))-B_mJ(m)Df(m)^{-1}=Q_1(m).
\]

The homogeneous first-jet cocycle is

\[
J\mapsto B_mJDf(m)^{-1}.
\]

Along the stable subbundle it is bounded by

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m_n)\|,
\]

and along the unstable subbundle, backward in time, by

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|.
\]

The \(1\)-bunching estimate therefore gives an exponential dichotomy for the first-jet cocycle. Applying the \(C^0\) Green inverse to the first-jet equation yields

\[
\|J\|_{C^0}
\le
C\|Q_1\|_{C^0}.
\]

Since \(Q_1\) depends linearly on \(Dq\) and on \(\zeta\), and since \(\|\zeta\|_{C^0}\le C\|q\|_{C^0}\), we obtain

\[
\|\zeta\|_{C^1}\le C\|q\|_{C^1}.
\]

### A.4. Higher derivatives

Assume inductively that, for some \(1\le k\le r\),

\[
\|\zeta\|_{C^{k-1}}\le C\|q\|_{C^{k-1}}.
\]

The \(k\)-th covariant derivative of the equation has principal part

\[
D^k\zeta(f(m))\circ Df(m)^{\otimes k}-B_mD^k\zeta(m).
\]

All remaining terms contain derivatives of \(f\), \(B\), the connection coefficients, \(q\), and \(\zeta\), but derivatives of \(\zeta\) occur only up to order \(k-1\). Thus the lower-order terms are controlled by the induction hypothesis.

The principal homogeneous \(k\)-jet cocycle is

\[
J\mapsto B_mJ\circ(Df(m)^{-1})^{\otimes k},
\]

where

\[
J(m)\in \operatorname{Sym}^k(T_m^*M;E_m).
\]

The stable part is controlled by

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m_n)\|^k,
\]

and the backward unstable part by

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|^k.
\]

The \(k\)-bunching condition gives an exponential dichotomy for the induced \(k\)-jet cocycle. The \(C^0\) Green inverse applied to this induced equation gives

\[
\|D^k\zeta\|_{C^0}\le C_k\|q\|_{C^k}.
\]

Induction proves

\[
\|\mathcal A^{-1}q\|_{C^k}\le C_k\|q\|_{C^k}
\]

for every \(0\le k\le r\).

### A.5. Parameter dependence

If \(f\), \(B\), and \(q\) depend on a parameter and the dichotomy and bunching constants are uniform, the \(C^0\) Green sums converge uniformly in the parameter. Differentiating the parameter-dependent cohomological equation gives linear equations of the same type, with inhomogeneous terms controlled by lower parameter derivatives. Under the corresponding mixed base/parameter bunching conditions, the same induction gives the claimed parameter regularity.

### A.6. Continuous projections

If the dichotomy projections are merely continuous, the derivative computation above should not be read as differentiating the projections. Instead, one works with transported difference quotients. The principal difference-quotient cocycles are the same jet cocycles displayed above, and the lower-order commutator terms converge uniformly. This is precisely the HPS difference-quotient mechanism. The self-contained proof above therefore closes the smooth-splitting case, while the continuous-splitting case is obtained by the standard transported difference-quotient interpretation.

---

## Appendix B. Strong fibres from a half-line Perron method

This appendix records a standalone proof of the local strong stable fibre theorem. The unstable theorem follows by applying the same argument to the inverse map.

### B.1. Statement

Let \(F\) be a \(C^{r+1}\) local diffeomorphism of a Banach space or Banach manifold, and let \(M\) be an invariant \(C^r\) manifold. Fix \(p\in M\) and write

\[
p_n=F^n(p),
\qquad A_n=DF(p_n).
\]

Assume that along the orbit there is an invariant splitting

\[
T_{p_n}X=E^s_{p_n}\oplus E^{cu}_{p_n},
\qquad
E^{cu}_{p_n}=T_{p_n}M\oplus E^u_{p_n},
\]

with uniformly bounded projections. Assume that

\[
\|\Phi^s(n,k)\|\le C e^{-\alpha_s(n-k)},
\qquad n\ge k,
\]

and

\[
\|\Phi^{cu}(n,k)\|\le C e^{\beta_{cu}(k-n)},
\qquad n\le k.
\]

Assume

\[
\beta_{cu}<\alpha_s.
\]

Then for every \(\gamma\in(\beta_{cu},\alpha_s)\), there exists a local strong stable fibre \(W^s_{\mathrm{loc}}(p)\) through \(p\), tangent to \(E^s_p\), such that points on the fibre track the orbit of \(p\) at rate \(e^{-\gamma n}\).

### B.2. Moving coordinates and remainders

Work in uniformly controlled moving coordinates along \(p_n\), so that a nearby orbit is written

\[
p_n+\xi_n,
\qquad
\xi_n=\xi_n^s+
\xi_n^{cu}.
\]

The equation is

\[
\xi_{n+1}=A_n\xi_n+R_n(\xi_n),
\]

where

\[
R_n(0)=0,
\qquad DR_n(0)=0.
\]

After shrinking the coordinate neighbourhood, uniformly in \(n\),

\[
\|R_n(\xi)\|\le C\|\xi\|^2,
\qquad
\|DR_n(\xi)\|\le C\|\xi\|.
\]

### B.3. The weighted space and Perron operator

Choose \(\gamma\) with

\[
\beta_{cu}<\gamma<\alpha_s.
\]

Let

\[
\ell_\gamma^+=
\left\{
\xi=(\xi_n)_{n\ge0}:
\|\xi\|_\gamma=
\sup_{n\ge0}e^{\gamma n}\|\xi_n\|<\infty
\right\}.
\]

For \(a\in E^s_p\), define

\[
(\mathcal P_a\xi)_n^s
=
\Phi^s(n,0)a+
\sum_{k=0}^{n-1}
\Phi^s(n,k+1)P^s_{k+1}R_k(\xi_k),
\]

and

\[
(\mathcal P_a\xi)_n^{cu}
=
-
\sum_{k=n}^{\infty}
\Phi^{cu}(n,k+1)P^{cu}_{k+1}R_k(\xi_k).
\]

Set

\[
\mathcal P_a\xi=(\mathcal P_a\xi)^s+(\mathcal P_a\xi)^{cu}.
\]

The center component belongs to \(\xi^{cu}\); it is not frozen.

### B.4. Self-map estimate

Let

\[
B_r=\{\xi\in\ell_\gamma^+:\|\xi\|_\gamma\le r\}.
\]

If \(\xi\in B_r\), then

\[
\|\xi_k\|\le r e^{-\gamma k},
\]

and therefore

\[
\|R_k(\xi_k)\|\le Cr^2e^{-2\gamma k}.
\]

The stable homogeneous term satisfies

\[
e^{\gamma n}\|\Phi^s(n,0)a\|
\le
C e^{-(\alpha_s-\gamma)n}\|a\|
\le C\|a\|.
\]

The stable nonlinear convolution is bounded by

\[
C r^2 e^{\gamma n}
\sum_{k=0}^{n-1}e^{-\alpha_s(n-k-1)}e^{-2\gamma k}
\le C r^2,
\]

because \(\gamma<\alpha_s\). The center-unstable convolution is bounded by

\[
C r^2 e^{\gamma n}
\sum_{k=n}^{\infty}e^{\beta_{cu}(k+1-n)}e^{-2\gamma k}.
\]

Writing \(k=n+j\), this becomes

\[
C r^2 e^{-\gamma n}
\sum_{j=0}^{\infty}e^{(\beta_{cu}-2\gamma)j},
\]

which is uniformly bounded since \(\beta_{cu}<\gamma\). Hence

\[
\|\mathcal P_a\xi\|_\gamma
\le
C\|a\|+Cr^2.
\]

Choose \(r>0\) small and \(\|a\|\le c r\). Then \(\mathcal P_a(B_r)\subset B_r\).

### B.5. Contraction estimate

For \(\xi,\eta\in B_r\), the mean-value theorem and the bound on \(DR_n\) give

\[
\|R_k(\xi_k)-R_k(\eta_k)\|
\le
C r e^{-\gamma k}\|\xi_k-\eta_k\|
\le
C r e^{-2\gamma k}\|\xi-\eta\|_\gamma.
\]

The same convolution estimates as above yield

\[
\|\mathcal P_a\xi-\mathcal P_a\eta\|_\gamma
\le
C r\|\xi-\eta\|_\gamma.
\]

Taking \(r\) smaller if necessary gives \(Cr<1\). Thus \(\mathcal P_a\) is a contraction on \(B_r\).

### B.6. The stable fibre, tracking, and tangency

By the Banach fixed-point theorem, there is a unique \(\xi(a)\in B_r\) satisfying

\[
\mathcal P_a\xi(a)=\xi(a).
\]

Define

\[
W^s_{\mathrm{loc}}(p)=
\{p+\xi_0(a):a\in E^s_p,
\|a\|\text{ sufficiently small}\}.
\]

The fixed-point equation is exactly the variation-of-constants formula for the nonlinear orbit equation, so the point \(p+\xi_0(a)\) has a forward orbit staying in the coordinate neighbourhood and satisfying

\[
\|F^n(p+\xi_0(a))-F^n(p)\|
\le
C e^{-\gamma n}\|a\|.
\]

Tangency follows by differentiating the fixed-point equation at \(a=0\). Since \(R_n(0)=0\) and \(DR_n(0)=0\), the derivative satisfies

\[
(D_a\xi(a)|_{a=0})_n^s=
\Phi^s(n,0),
\qquad
(D_a\xi(a)|_{a=0})_n^{cu}=0.
\]

At \(n=0\), this gives

\[
D_a\xi_0(0)=\operatorname{id}_{E^s_p}.
\]

Therefore

\[
T_pW^s_{\mathrm{loc}}(p)=E^s_p.
\]

Local uniqueness holds among trajectories in the weighted class because the Perron operator has a unique fixed point.

### B.7. The unstable fibre

Apply the preceding theorem to \(F^{-1}\), grouping

\[
T_{p_n}X=E^u_{p_n}\oplus E^{cs}_{p_n},
\qquad
E^{cs}_{p_n}=T_{p_n}M\oplus E^s_{p_n}.
\]

If the backward unstable contraction rate dominates the backward growth rate of \(E^{cs}\), the same half-line argument on negative time gives \(W^u_{\mathrm{loc}}(p)\), tangent to \(E^u_p\). Internal regularity of these fibres and transverse regularity of the family require additional bunching and are not consequences of the basic contraction alone.


---

## Appendix C. Roughness of exponential dichotomies in Banach bundles

This appendix records the linear robustness estimate used for persistence of the normal splitting. We state and prove the fixed-base version. The close-base version, where the base diffeomorphism is also perturbed, follows by the same estimates after transporting fibres to a common reference bundle; this is the standard roughness theorem for exponential dichotomies.

### C.1. Statement

Let \(E\to M\) be a Banach bundle over a compact base, and let

\[
B_m:E_m\to E_{f(m)}
\]

be a bundle automorphism over a homeomorphism \(f:M\to M\). Assume that \(B\) has an exponential dichotomy

\[
E_m=E_m^s\oplus E_m^u
\]

with projections uniformly bounded by \(K_P\), and with constants \(C>0\) and \(0<\lambda<1\):

\[
\|\Phi^s(n,k)\|\le C\lambda^{n-k},
\qquad n\ge k,
\]

and

\[
\|\Phi^u(k,n)\|\le C\lambda^{n-k},
\qquad n\ge k.
\]

Let

\[
\widetilde B_m=B_m+R_m:E_m\to E_{f(m)}
\]

be another bundle automorphism over the same base map, with

\[
\sup_m\|R_m\|\le\delta.
\]

Then, for every \(\gamma\) with

\[
\lambda<\gamma<1,
\]

there exists \(\delta_0>0\) such that if \(0<\delta<\delta_0\), the cocycle \(\widetilde B\) has an exponential dichotomy with rate \(\gamma\). Its stable and unstable bundles are graphs over the original bundles:

\[
\widetilde E_m^s=\{a+L_m^s a:a\in E_m^s\},
\qquad
L_m^s:E_m^s\to E_m^u,
\]

and

\[
\widetilde E_m^u=\{b+L_m^u b:b\in E_m^u\},
\qquad
L_m^u:E_m^u\to E_m^s,
\]

with

\[
\sup_m\|L_m^s\|+\\sup_m\|L_m^u\|
\le C_\gamma\delta.
\]

The perturbed projections are uniformly bounded and converge to the original projections as \(\delta\to0\).

### C.2. Stable graph by a half-line Perron equation

Fix \(m\in M\) and write \(m_n=f^n(m)\). Along this orbit, the perturbed linear equation is

\[
x_{n+1}=B_{m_n}x_n+R_{m_n}x_n.
\]

Choose \(\gamma\in(\lambda,1)\) and define the weighted sequence space

\[
\ell_\gamma^+
=
\left\{
x=(x_n)_{n\ge0}:
\|x\|_\gamma=
\sup_{n\ge0}\gamma^{-n}\|x_n\|<\infty
\right\}.
\]

For a prescribed stable coordinate \(a\in E_m^s\), define a linear Perron operator on \(\ell_\gamma^+\) by

\[
(\mathcal T_a x)_n^s
=
\Phi^s(n,0)a
+
\sum_{k=0}^{n-1}
\Phi^s(n,k+1)P^s_{m_{k+1}}R_{m_k}x_k,
\]

and

\[
(\mathcal T_a x)_n^u
=
-
\sum_{k=n}^{\infty}
\Phi^u(n,k+1)P^u_{m_{k+1}}R_{m_k}x_k.
\]

Set \(\mathcal T_a x=(\mathcal T_a x)^s+(\mathcal T_a x)^u\). The first sum is finite and the second converges absolutely in the weighted norm.

Indeed, using \(\|x_k\|\le\gamma^k\|x\|_\gamma\),

\[
\gamma^{-n}
\left\|
\sum_{k=0}^{n-1}
\Phi^s(n,k+1)P^sR_kx_k
\right\|
\le
C K_P\delta\|x\|_\gamma
\sum_{k=0}^{n-1}
\gamma^{-n}\lambda^{n-k-1}
\gamma^k.
\]

Writing \(j=n-k-1\), this is bounded by

\[
C K_P\delta\gamma^{-1}
\sum_{j=0}^{\infty}(\lambda/\gamma)^j
\|x\|_\gamma
\le
C_1(\gamma)\delta\|x\|_\gamma.
\]

Similarly,

\[
\gamma^{-n}
\left\|
\sum_{k=n}^{\infty}
\Phi^u(n,k+1)P^uR_kx_k
\right\|
\le
C K_P\delta\|x\|_\gamma
\sum_{k=n}^{\infty}
\gamma^{-n}\lambda^{k+1-n}
\gamma^k.
\]

Writing \(j=k-n\), this becomes

\[
C K_P\delta\lambda
\sum_{j=0}^{\infty}(\lambda\gamma)^j
\|x\|_\gamma
\le
C_2(\gamma)\delta\|x\|_\gamma.
\]

Thus

\[
\|\mathcal T_a x-\mathcal T_a y\|_\gamma
\le
C_3(\gamma)\delta\|x-y\|_\gamma.
\]

For \(\delta\) small enough, \(C_3(\gamma)\delta<1\), so \(\mathcal T_a\) is a contraction. It has a unique fixed point \(x(a)\in\ell_\gamma^+\). The dependence on \(a\) is linear and bounded, since \(\mathcal T_a\) is affine in \(a\).

Define

\[
L_m^s a:=P_m^u x_0(a).
\]

Then

\[
\widetilde E_m^s:=\{a+L_m^s a:a\in E_m^s\}
\]

is the set of initial data whose forward perturbed orbit lies in \(\ell_\gamma^+\). Since the fixed point satisfies the variation-of-constants formula, \(\widetilde E^s\) is invariant under \(\widetilde B\). Moreover,

\[
\|L_m^s a\|
\le C_\gamma\delta\|a\|.
\]

The fixed point estimate also gives, for \(x_0\in\widetilde E_m^s\),

\[
\|\widetilde\Phi(n,0)x_0\|
\le
C_\gamma\gamma^n\|x_0\|.
\]

### C.3. Unstable graph

Apply the same construction to the inverse cocycle over negative time. Equivalently, fix \(b\in E_m^u\) and solve the backward weighted equation in

\[
\ell_\gamma^-=
\left\{
x=(x_n)_{n\le0}:
\sup_{n\le0}\gamma^{n}\|x_n\|<\infty
\right\}.
\]

The backward dichotomy estimate gives a contraction for \(\delta\) small. This produces a graph

\[
\widetilde E_m^u=
\{b+L_m^u b:b\in E_m^u\},
\]

with

\[
\|L_m^u\|
\le C_\gamma\delta,
\]

and, for \(x_0\in\widetilde E_m^u\),

\[
\|\widetilde\Phi(-n,0)x_0\|
\le
C_\gamma\gamma^n\|x_0\|,
\qquad n\ge0.
\]

### C.4. Splitting and projections

For \(\delta\) small, both graph maps have norm less than one. Hence

\[
E_m=\widetilde E_m^s\oplus\widetilde E_m^u
\]

for every \(m\), and the associated projections are uniformly bounded. The graph norms are \(O(\delta)\), so the perturbed projections converge uniformly to the original projections.

Continuity of \(m\mapsto \widetilde E_m^s\) and \(m\mapsto \widetilde E_m^u\) follows from continuous dependence of the contraction fixed point on parameters. If the cocycle depends with higher regularity and the corresponding graph transforms act on higher regularity section spaces with bunching, the same argument gives higher regularity of the splitting.

This proves the fixed-base roughness theorem.


---

## Appendix D. A normally attracting Banach-bundle graph transform

This appendix proves a self-contained one-sided version of the invariant-section theorem. It does not replace the two-sided HPS theorem used in the main normally hyperbolic case, but it closes the important normally attracting case and records the estimates that underlie the admissible graph transform.

### D.1. Statement

Let \(E\to M\) be a \(C^{r+1}\) Banach bundle over a compact finite-dimensional \(C^{r+1}\) manifold, and let

\[
F_\varepsilon(m,\eta)=(b_\varepsilon(m,\eta),g_\varepsilon(m,\eta))
\]

be a \(C^{r+1}\) fibre map defined near the zero section. Assume

\[
b_0(m,0)=f(m),
\qquad
g_0(m,0)=0,
\]

where \(f\in\operatorname{Diff}^{r+1}(M)\). Assume

\[
D_\eta b_0(m,0)=0,
\qquad
B_m:=D_\eta g_0(m,0):E_m\to E_{f(m)}
\]

is a bundle automorphism satisfying the normally attracting estimates

\[
\nu_0:=\sup_m\|B_m\|<1,
\]

and, for \(1\le j\le r\),

\[
\nu_j:=\sup_m\|B_m\|\,\|Df(m)^{-1}\|^j<1.
\]

Assume the transported remainder

\[
r_\varepsilon(m,\eta)
=
g_\varepsilon(m,\eta)-\tau_{b_\varepsilon(m,\eta)\leftarrow f(m)}B_m\eta
\]

satisfies, on \(\|\eta\|\le\rho\),

\[
\|r_\varepsilon(m,0)\|\le C\delta_\varepsilon,
\]

\[
\|D_\eta r_\varepsilon(m,\eta)\|+
\|D_m r_\varepsilon(m,\eta)\|
\le C\delta_\varepsilon+
\omega(\rho),
\]

and

\[
\|D_\eta b_\varepsilon(m,\eta)\|
\le C\delta_\varepsilon+
\omega(\rho),
\]

where \(\omega(\rho)\to0\) as \(\rho\to0\). Then for \(\rho>0\), \(L>0\), and \(\delta_\varepsilon\) sufficiently small, there exists a unique section

\[
h_\varepsilon\in\Gamma^r(E),
\qquad
\|h_\varepsilon\|_{C^0}\le\rho,
\qquad
\operatorname{Lip}(h_\varepsilon)\le L,
\]

such that, with

\[
f_\varepsilon(m)=b_\varepsilon(m,h_\varepsilon(m)),
\]

one has the graph equation

\[
h_\varepsilon(f_\varepsilon(m))
=
g_\varepsilon(m,h_\varepsilon(m)).
\]

Moreover, if \(\|F_\varepsilon-F_0\|_{C^k}\le C|\varepsilon|\) for \(0\le k\le r\), then

\[
\|h_\varepsilon\|_{C^k}
\le C_k|\varepsilon|.
\]

### D.2. The forward graph transform

For \(h\in\mathcal B_{\rho,L}\), define

\[
b_h(m)=b_\varepsilon(m,h(m)).
\]

Because \(h\) is initially only Lipschitz, \(b_h\) should not be called a \(C^1\) local diffeomorphism at this stage. Instead, in local charts write \(b_h=f+e_h\). The estimates on \(D_\eta b_\varepsilon\), together with the small Lipschitz aperture of \(h\) and the \(C^1\)-closeness of \(b_\varepsilon(\cdot,0)\) to \(f\), give

\[
\operatorname{Lip}(f^{-1}\circ b_h-\operatorname{id})
\le \mu(\rho,L,\delta_\varepsilon)<1.
\]

Thus \(f^{-1}\circ b_h\) is a bi-Lipschitz homeomorphism by the contraction mapping theorem applied to the equation \(x+(f^{-1}\circ b_h-\operatorname{id})(x)=y\). Hence \(b_h\) is a bi-Lipschitz homeomorphism close to \(f\), with a uniformly Lipschitz inverse. Once the fixed point has been upgraded to \(C^r\), the corresponding map \(b_{h_\varepsilon}\) is a \(C^r\) diffeomorphism. Define the graph transform by

\[
(\mathcal H_\varepsilon h)(y)
=
g_\varepsilon(b_h^{-1}(y),h(b_h^{-1}(y))).
\]

All fibre comparisons are made using the fixed local transports. This is the ordinary forward graph transform; no unstable matching is needed in the attracting case.

### D.3. The \(C^0\) contraction

Let \(h_1,h_2\in\mathcal B_{\rho,L}\), set \(b_i=b_{h_i}\), and let

\[
x_i=b_i^{-1}(y).
\]

Since \(b_1(x_1)=b_2(x_2)=y\), write

\[
b_1(x_1)-b_1(x_2)=b_2(x_2)-b_1(x_2)
\]

in a local chart on \(M\). The right-hand side is controlled by the fibre derivative of \(b_\varepsilon\):

\[
d_M(b_1(x_2),b_2(x_2))
\le
\|D_\eta b_\varepsilon\|_{C^0}
\|h_1-h_2\|_{C^0}.
\]

Since \(b_1^{-1}\) has uniformly bounded Lipschitz constant, with bound \(\|Df^{-1}\|+O(\delta_\varepsilon)+O(L)+O(\omega(\rho))\), we get the base preimage estimate

\[
d_M(x_1,x_2)
\le
\mu_{\mathrm{base}}
\|h_1-h_2\|_{C^0},
\]

where

\[
\mu_{\mathrm{base}}
\le
C\|D_\eta b_\varepsilon\|_{C^0}
\le
C(\delta_\varepsilon+\omega(\rho)).
\]

All values below are transported to the common target fibre \(E_y\). Using

\[
g_\varepsilon(m,\eta)=
\tau_{b_\varepsilon(m,\eta)\leftarrow f(m)}B_m\eta+r_\varepsilon(m,\eta),
\]

split the difference into a pure fibre shift at \(x_1\) and a base-induced shift from \(x_1\) to \(x_2\). The pure fibre term is bounded by

\[
\left(\nu_0+C\delta_\varepsilon+\omega(\rho)\right)
\|h_1-h_2\|_{C^0},
\]

where \(\nu_0=\sup_m\|B_m\|<1\). The base-induced term is bounded by

\[
\mu_{\mathrm{base}}
\left[
C\delta_\varepsilon+\omega(\rho)
+L(\nu_0+C\delta_\varepsilon+\omega(\rho))
\right]
\|h_1-h_2\|_{C^0}.
\]

The terms coming from the variation of the fibre transports are included in the same \(C\delta_\varepsilon+\omega(\rho)\) bound, since the target bases differ by \(O(\|D_\eta b_\varepsilon\|\|h_1-h_2\|)\). Hence

\[
\|\mathcal H_\varepsilon h_1-
\mathcal H_\varepsilon h_2\|_{C^0}
\le
(\nu_0+
\mu)
\|h_1-h_2\|_{C^0},
\]

where one may take

\[
\mu
=
C\delta_\varepsilon+\omega(\rho)
+
\mu_{\mathrm{base}}
\left[
C\delta_\varepsilon+\omega(\rho)
+L(\nu_0+C\delta_\varepsilon+\omega(\rho))
\right].
\]

Thus \(\mu\to0\) as \(\rho,L,\delta_\varepsilon\to0\). Choosing the constants in the order described above gives a contraction factor \(q=\nu_0+\mu<1\). The radius estimate is

\[
\|\mathcal H_\varepsilon h\|_{C^0}
\le
C\delta_\varepsilon+(\nu_0+\mu)\rho.
\]

After fixing \(\rho\) and then choosing \(\delta_\varepsilon\) small, \(\mathcal H_\varepsilon\) maps the \(C^0\)-ball of radius \(\rho\) into itself.

### D.4. Lipschitz preservation

Let \(y_1,y_2\in M\), and set \(x_i=b_h^{-1}(y_i)\). Since \(b_h^{-1}\) is close to \(f^{-1}\),

\[
d_M(x_1,x_2)
\le
(\|Df^{-1}\|+
\mu)d_M(y_1,y_2).
\]

Using transported difference estimates for the linear part and the base and fibre derivative estimates for the remainder,

\[
\begin{aligned}
&\|(\mathcal H_\varepsilon h)(y_1)-(\mathcal H_\varepsilon h)(y_2)\| \\
&\qquad\le
(\|B\|\,\|Df^{-1}\|+
\mu)
\operatorname{Lip}(h)
\,d_M(y_1,y_2)
+
\mu d_M(y_1,y_2).
\end{aligned}
\]

Thus

\[
\operatorname{Lip}(\mathcal H_\varepsilon h)
\le
(\nu_1+
\mu)L+
\mu.
\]

Choose \(L>0\) and then choose \(\rho\) and \(\delta_\varepsilon\) so small that

\[
(\nu_1+
\mu)L+
\mu
\le L.
\]

Then \(\mathcal H_\varepsilon\mathcal B_{\rho,L}\subset\mathcal B_{\rho,L}\).

### D.5. Existence, uniqueness, and the graph equation

The space \(\mathcal B_{\rho,L}\) is complete in the \(C^0\) metric. The graph transform is a contraction and maps \(\mathcal B_{\rho,L}\) into itself. Therefore it has a unique fixed point \(h_\varepsilon\). By definition of \(\mathcal H_\varepsilon\), the fixed-point equation says

\[
h_\varepsilon(y)
=
g_\varepsilon(b_{h_\varepsilon}^{-1}(y),
h_\varepsilon(b_{h_\varepsilon}^{-1}(y))).
\]

Putting \(y=f_\varepsilon(m)=b_{h_\varepsilon}(m)\) gives

\[
h_\varepsilon(f_\varepsilon(m))
=
g_\varepsilon(m,h_\varepsilon(m)).
\]

This is the graph equation. Since \(f_\varepsilon=b_{h_\varepsilon}\) is a diffeomorphism close to \(f\), it also gives setwise equality of the graph with its image.

### D.6. \(C^r\) regularity and estimates

The derivative of the graph transform on first jets has principal fibre part

\[
J\mapsto B_mJ Df(m)^{-1}.
\]

Its norm is bounded by \(\nu_1<1\), up to the small error \(\mu\). Therefore the induced first-jet transform is a contraction. Inductively, the induced \(j\)-jet transform has principal part

\[
J\mapsto B_mJ\circ(Df(m)^{-1})^{\otimes j},
\]

with norm bounded by \(\nu_j<1\), again up to a small error. Lower-order Faà di Bruno terms depend only on previously constructed lower jets. The fibre-contraction argument on jet bundles gives \(h_\varepsilon\in C^r\).

If \(F_\varepsilon-F_0=O(\varepsilon)\) in \(C^k\), then the graph transform sends the zero section to an \(O(\varepsilon)\) section in \(C^k\), and each induced jet transform has a uniform contraction constant. Hence

\[
\|h_\varepsilon\|_{C^k}
\le C_k|\varepsilon|,
\qquad
0\le k\le r.
\]

This completes the normally attracting Banach-bundle graph-transform theorem.


---

## Appendix E. Close-base roughness by a linear graph transform

Appendix C proves fixed-base roughness. This appendix records a direct close-base graph-transform version sufficient for the normal-splitting argument in Theorem 5.1. The statement is deliberately formulated in transported block coordinates; those are the coordinates obtained by identifying the fibre over \(\widetilde f(m)\) with the nearby fibre over \(f(m)\), or conversely, using the connection.

### E.1. Statement

Let \(E=E^s\oplus E^u\) be a Banach bundle over compact \(M\), with uniformly bounded projections. Let \(\widetilde f:M\to M\) be a homeomorphism. Let

\[
A_m:E_m\to E_{\widetilde f(m)}
\]

be a bundle automorphism. Write its block form with respect to the original splitting at \(m\) and at \(\widetilde f(m)\):

\[
A_m=
\begin{pmatrix}
A_m^{ss} & A_m^{su}\\
A_m^{us} & A_m^{uu}
\end{pmatrix}.
\]

Assume that \(A_m^{uu}:E_m^u\to E_{\widetilde f(m)}^u\) is invertible and that, in an adapted norm, there are constants

\[
0<\alpha<1,
\qquad
0<\beta<1,
\qquad
\delta>0
\]

such that, uniformly in \(m\),

\[
\|A_m^{ss}\|\le\alpha,
\qquad
\|(A_m^{uu})^{-1}\|\le\beta,
\]

and

\[
\|A_m^{su}\|+
\|A_m^{us}\|\le\delta.
\]

If \(\delta\) is sufficiently small, then there is a unique invariant stable bundle of the form

\[
\widetilde E_m^s=
\{a+L_m^s a:a\in E_m^s\},
\qquad
L_m^s:E_m^s\to E_m^u,
\]

with

\[
\sup_m\|L_m^s\|\le C\delta.
\]

It satisfies

\[
A_m\widetilde E_m^s=
\widetilde E_{\widetilde f(m)}^s.
\]

Similarly, applying the same argument to the inverse cocycle gives an invariant unstable bundle, provided the corresponding inverse-time block estimates hold. For perturbations of an invertible dichotomous cocycle these estimates follow from the original unstable contraction backward in time. Thus

\[
\widetilde E_m^u=
\{b+L_m^u b:b\in E_m^u\},
\qquad
\sup_m\|L_m^u\|\le C\delta.
\]

The resulting splitting is a small perturbation of \(E^s\oplus E^u\), and the corresponding projections are uniformly bounded.

### E.2. Stable graph transform

Let \(\mathcal X_R\) be the complete metric space of continuous sections

\[
L_m:E_m^s\to E_m^u,
\qquad
\sup_m\|L_m\|\le R,
\]

with the \(C^0\) operator norm. We define a transform \(\mathfrak T\) on \(\mathcal X_R\).

Given \(L\in\mathcal X_R\), for each \(m\) define \((\mathfrak T L)_m=X_m\) as the unique solution of

\[
X_m
=
(A_m^{uu})^{-1}
\left[
L_{\widetilde f(m)}(A_m^{ss}+A_m^{su}X_m)-A_m^{us}
\right].
\]

For fixed \(L\), the right-hand side is a contraction in \(X_m\), since

\[
\|(A_m^{uu})^{-1}\|\,
\|L_{\widetilde f(m)}\|\,
\|A_m^{su}\|
\le
\beta R\delta.
\]

Choose \(R\) and \(\delta\) so that \(\beta R\delta<1/2\). Then \(X_m\) exists uniquely and depends continuously on \(m\).

The bound

\[
\|X_m\|
\le
\frac{\beta(R\alpha+
\delta)}{1-
\beta R\delta}
\]

shows that, for \(R=C\delta\) and \(\delta\) small, \(\mathfrak T\) maps \(\mathcal X_R\) into itself.

### E.3. Contraction of the graph transform

Let \(L,L'\in\mathcal X_R\), and write

\[
X_m=(\mathfrak T L)_m,
\qquad
X_m'=(\mathfrak T L')_m.
\]

Subtracting the defining equations gives

\[
\begin{aligned}
X_m-X_m'
&=(A_m^{uu})^{-1}
\Bigl[
(L_{\widetilde f(m)}-L'_{\widetilde f(m)})(A_m^{ss}+A_m^{su}X_m)\\
&\qquad
+L'_{\widetilde f(m)}A_m^{su}(X_m-X_m')
\Bigr].
\end{aligned}
\]

Therefore

\[
\|X_m-X_m'\|
\le
\frac{\beta(\alpha+\delta R)}{1-\beta R\delta}
\|L-L'\|_{C^0}.
\]

Since \(\alpha<1\) and \(\beta<1\), the constant is strictly less than one for \(\delta\) small. Hence \(\mathfrak T\) is a contraction. It has a unique fixed point \(L^s\in\mathcal X_R\).

### E.4. Invariance and estimates

Let

\[
\widetilde E_m^s=
\operatorname{graph}L_m^s.
\]

If \(v=a+L_m^s a\), then

\[
A_m v
=
(A_m^{ss}+A_m^{su}L_m^s)a
+
(A_m^{us}+A_m^{uu}L_m^s)a.
\]

The fixed-point equation is exactly

\[
A_m^{us}+A_m^{uu}L_m^s
=
L_{\widetilde f(m)}^s(A_m^{ss}+A_m^{su}L_m^s).
\]

Thus

\[
A_m\operatorname{graph}L_m^s
\subset
\operatorname{graph}L_{\widetilde f(m)}^s.
\]

Since \(A_m\) is invertible and the graph map is close to the original stable space, the inclusion is equality. The graph bound gives

\[
\sup_m\|L_m^s\|\le C\delta.
\]

For \(v\in\widetilde E_m^s\), its stable coordinate evolves by

\[
a_{n+1}=(A_{m_n}^{ss}+A_{m_n}^{su}L_{m_n}^s)a_n.
\]

Hence

\[
\|a_{n+1}\|
\le
(\alpha+
\delta C\delta)
\|a_n\|.
\]

For \(\delta\) small, this gives any weakened stable rate larger than \(\alpha\). Norm equivalence between the graph norm and the ambient norm yields the corresponding exponential estimate on \(\widetilde E^s\).

### E.5. Unstable graph and splitting

The unstable bundle follows by applying the same argument to \(A^{-1}\) over \(\widetilde f^{-1}\), or equivalently by solving the symmetric graph equation for maps \(L_m^u:E_m^u\to E_m^s\). This gives

\[
\widetilde E_m^u=
\operatorname{graph}L_m^u,
\qquad
\sup_m\|L_m^u\|\le C\delta,
\]

and backward exponential estimates with weakened rates.

If \(\delta\) is small, both graph maps have norm less than one. Therefore

\[
E_m=
\widetilde E_m^s\oplus\widetilde E_m^u
\]

and the associated projections are uniformly bounded. The perturbed projections differ from the original projections by \(O(\delta)\). This proves close-base roughness under the transported block estimates.


---

## Appendix F. Parameter expansions of invariant sections

This appendix justifies the expansion statement used in Theorem 5.1. It is an abstract consequence of the graph equation, the cohomological inverse, and the parameter differentiability supplied by the invariant-section theorem. It does not add new dynamical hypotheses; it records exactly what the expansion coefficients solve once parameter regularity is available.

### F.1. Abstract formulation

Let \(X_r\) and \(Y_r\) be Banach spaces of sections, for example

\[
X_r=\Gamma^r(E),
\qquad
Y_r=\Gamma^r(f^*E),
\]

or the corresponding transported difference-quotient spaces. Let

\[
\Psi:(-\varepsilon_0,
\varepsilon_0)\times U	o Y_r,
\qquad
(\varepsilon,h)
\mapsto
\Psi_\varepsilon(h),
\]

be the transported graph residual, with \(U\subset X_r\) a neighbourhood of the zero section. Assume

\[
\Psi_0(0)=0,
\]

and

\[
D_h\Psi_0(0)=\mathcal A,
\]

where

\[
\mathcal A h=h\circ f-Bh
\]

is the cohomological operator. Assume that \(\mathcal A:X_r\to Y_r\) is an isomorphism and that \(\Psi\) is \(C^{N+1}\) in \((\varepsilon,h)\) in the section topologies under consideration. Then the Banach implicit function theorem gives a unique \(C^{N+1}\) curve

\[
\varepsilon\mapsto h_\varepsilon\in X_r
\]

with

\[
\Psi_\varepsilon(h_\varepsilon)=0,
\qquad
h_0=0.
\]

The HPS graph transform supplies this curve in the manuscript. The point here is that, once it is known to be sufficiently differentiable in \(\varepsilon\), the coefficient equations follow by differentiating \(\Psi_\varepsilon(h_\varepsilon)=0\).

### F.2. First coefficient

Let

\[\eta_j:=\partial_\varepsilon^j h_\varepsilon|_{\varepsilon=0}.
\]

Differentiating once gives

\[
D_\varepsilon\Psi_0(0)+D_h\Psi_0(0)\eta_1=0.
\]

Thus

\[
\mathcal A\eta_1
=
-\partial_\varepsilon\Psi_0(0),
\]

and therefore

\[\eta_1
=
-\mathcal G\,
\partial_\varepsilon\Psi_0(0).
\]

This is the first-order cohomological equation for the displacement of the invariant graph.

### F.3. Higher coefficients

For \(n\ge2\), differentiating \(n\) times gives

\[
\mathcal A\eta_n+R_n(\eta_1,
\ldots,
\eta_{n-1})=0,
\]

where \(R_n\) is a universal finite sum of derivatives of \(\Psi\) at \((0,0)\) applied to the previously computed coefficients. Explicitly,

\[
R_n
=
\sum_{
\substack{a+b\ge1,\ a\le n,\ b\le n\\
(a,b)\ne(0,1)}}
C_{a,b,n}
D_\varepsilon^aD_h^b\Psi_0(0)
[\eta_{j_1},
\ldots,
\eta_{j_b}
],
\]

where the sum is over indices satisfying

\[
a+j_1+\cdots+j_b=n,
\qquad
1\le j_i<n.
\]

The term \((a,b)=(0,1)\) with \(j_1=n\) is precisely \(\mathcal A\eta_n\) and is excluded from \(R_n\). Hence

\[\eta_n
=
-
\mathcal G R_n(\eta_1,
\ldots,
\eta_{n-1}).
\]

Thus every coefficient is obtained by solving one linear cohomological equation with the same inverse \(\mathcal G\).

### F.4. Expansion with or without factorials

Taylor's theorem gives

\[
h_\varepsilon
=
\sum_{j=1}^{N}
\frac{\varepsilon^j}{j!}
\eta_j
+O(\varepsilon^{N+1})
\]

in \(X_r\). If one writes the expansion in the form

\[
h_\varepsilon
=
\varepsilon h_1+
\varepsilon^2 h_2+\cdots+
\varepsilon^N h_N
+O(\varepsilon^{N+1}),
\]

then

\[
h_j=\frac{1}{j!}\eta_j.
\]

In the tubular coordinates used in the manuscript, the unperturbed invariant manifold is the zero section, so the constant coefficient is

\[
h_0=0.
\]

### F.5. Bounds and remainder

If \(\Psi\) is \(C^{N+1}\) with bounded derivatives on a neighbourhood of \((0,0)\), Taylor's theorem in Banach spaces gives

\[
\left\|h_\varepsilon-
\sum_{j=1}^{N}
\frac{\varepsilon^j}{j!}
\eta_j
\right\|_{X_r}
\le
C_N|
\varepsilon|^{N+1}.
\]

The constants depend on bounds for the derivatives of \(\Psi\), on the inverse bound for \(\mathcal G\), and on the parameter-bunching constants that give differentiability of \(\varepsilon\mapsto h_\varepsilon\). This proves the expansion statement used in the main text.


---

## Appendix G. Reduction of flows to time maps

This appendix isolates the time-\(T\) reduction used in Section 7. The point is to state exactly where full-flow invariance of the unperturbed manifold enters.

### G.1. Setting

Let \(\Phi_t^\varepsilon\) be a \(C^{r+1}\) local flow defined for \(|t|\le T\) on a fixed neighbourhood of a compact manifold \(M\). Assume

\[
\Phi_t^0(M)=M,
\qquad |t|\le T.
\]

Let

\[
F_\varepsilon:=\Phi_T^\varepsilon.
\]

Suppose the time-\(T\) map theorem gives an admissible invariant graph \(M_\varepsilon\) for \(F_\varepsilon\), locally unique among graphs in a prescribed tube with prescribed Lipschitz and cone bounds:

\[
F_\varepsilon(M_\varepsilon)=M_\varepsilon.
\]

Assume also that \(\Phi_t^\varepsilon\to\Phi_t^0\) in \(C^1\), uniformly for \(t\in[0,T]\), on the relevant tube. Then

\[
\Phi_t^\varepsilon(M_\varepsilon)=M_\varepsilon,
\qquad 0\le t\le T.
\]

Consequently, by the flow property,

\[
\Phi_t^\varepsilon(M_\varepsilon)=M_\varepsilon
\]

for all times for which the local flow is defined along the orbit.

### G.2. Proof

For \(0\le t\le T\), define

\[
N_t:=\Phi_t^\varepsilon(M_\varepsilon).
\]

Because the maps of a flow commute,

\[
F_\varepsilon(N_t)
=
\Phi_T^\varepsilon\Phi_t^\varepsilon(M_\varepsilon)
=
\Phi_t^\varepsilon\Phi_T^\varepsilon(M_\varepsilon)
=
\Phi_t^\varepsilon(M_\varepsilon)
=N_t.
\]

Thus \(N_t\) is invariant under the same time-\(T\) map.

We must check that \(N_t\) lies in the uniqueness class. Since \(M_\varepsilon\) is an admissible graph close to \(M\), and since \(\Phi_t^\varepsilon\) is uniformly \(C^1\)-close to \(\Phi_t^0\) for \(t\in[0,T]\), while \(\Phi_t^0(M)=M\), the image \(N_t\) remains in the same tubular neighbourhood for all \(t\in[0,T]\) when \(\varepsilon\) is small. The derivative of \(\Phi_t^\varepsilon\) maps the tangent spaces of \(M_\varepsilon\) to tangent spaces of \(N_t\); uniform \(C^1\)-closeness and compactness preserve the prescribed Lipschitz and cone bounds after, if necessary, choosing the admissible constants with a small margin. Hence \(N_t\) is an admissible invariant graph for \(F_\varepsilon\).

By local uniqueness for the time-\(T\) map,

\[
N_t=M_\varepsilon.
\]

Therefore

\[
\Phi_t^\varepsilon(M_\varepsilon)=M_\varepsilon,
\qquad 0\le t\le T.
\]

For arbitrary positive time, write \(t=nT+s\) with \(n\in\mathbb N\) and \(0\le s<T\). Repeated use of the time-\(T\) invariance and the just-proved invariance for \(s\in[0,T]\) gives invariance for \(t\). Negative times follow similarly when the local flow is defined backward along the relevant orbit.

### G.3. Necessity of full-flow invariance of the unperturbed manifold

If one only knows

\[
\Phi_T^0(M)=M
\]

and not \(\Phi_t^0(M)=M\) for \(0<t<T\), then \(\Phi_t^0(M)\) may leave the tubular neighbourhood of \(M\). In that case

\[
N_t=\Phi_t^\varepsilon(M_\varepsilon)
\]

need not lie in the admissible class for the time-\(T\) graph transform, so the uniqueness argument cannot be applied. Therefore the time-map reduction requires full-flow invariance of \(M\), or else one must construct the invariant manifold directly by a continuous-time Perron method.


---

## Appendix H. Globalization of local stable fibres

This appendix makes precise the passage from local strong stable fibres to the global stable set. The result is conditional on the orbit remaining in the region where the local construction is valid; no global statement is asserted outside that domain.

### H.1. Local fibre data

Let \(F\) be a \(C^{r+1}\) local diffeomorphism, and let \(M\) be a compact invariant manifold. Assume that for each \(p\in M\) there is a local strong stable fibre

\[
W^s_{\mathrm{loc}}(p)
\]

with uniform size and with the local tracking estimate

\[
\operatorname{dist}(F^n y,F^n p)
\le
C e^{-\gamma n}\operatorname{dist}(y,p),
\qquad n\ge0,
\]

whenever \(y\in W^s_{\mathrm{loc}}(p)\). Assume also the local invariance property

\[
F(W^s_{\mathrm{loc}}(p))
\cap U
\subset
W^s_{\mathrm{loc}}(Fp),
\]

where \(U\) is the local tube in which the fibres are defined. This local invariance follows from the uniqueness of the half-line Perron fixed point applied to the shifted reference orbit.

Let

\[
W^s_{\mathrm{loc}}(M)=
\bigcup_{p\in M}W^s_{\mathrm{loc}}(p).
\]

The local phase projection is

\[
\pi^s_{\mathrm{loc}}:W^s_{\mathrm{loc}}(M)\to M,
\qquad
\pi^s_{\mathrm{loc}}(y)=p
\]

when \(y\in W^s_{\mathrm{loc}}(p)\).

### H.2. Global stable set

Assume first that \(F\) is a diffeomorphism on the region under consideration. Define

\[
W_N^s(M):=F^{-N}(W^s_{\mathrm{loc}}(M)),
\qquad N\ge0,
\]

where the inverse image is taken only along points whose intermediate iterates remain in the domain of the map. The global stable set generated by the local fibres is

\[
W^s(M):=
\bigcup_{N\ge0} W_N^s(M).
\]

Equivalently,

\[
y\in W^s(M)
\]

if and only if there exists \(N\ge0\) such that

\[
F^N(y)
\in
W^s_{\mathrm{loc}}(M).
\]

### H.3. Phase projection

For \(y\in W_N^s(M)\), define

\[
\pi^s(y):=F^{-N}\left(
\pi^s_{\mathrm{loc}}(F^N y)
\right).
\]

This definition is independent of the choice of sufficiently large \(N\). Indeed, if \(F^N y\in W^s_{\mathrm{loc}}(p_N)\), then by local invariance

\[
F^{N+1}y
\in
W^s_{\mathrm{loc}}(Fp_N)
\]

as long as the orbit remains in the local tube. Therefore

\[
\pi^s_{\mathrm{loc}}(F^{N+1}y)=F p_N,
\]

and hence

\[
F^{-(N+1)}
\pi^s_{\mathrm{loc}}(F^{N+1}y)
=
F^{-N}p_N.
\]

Thus \(\pi^s\) is well defined.

### H.4. Invariance

If \(y\in W^s(M)\), choose \(N\) such that \(F^N y\in W^s_{\mathrm{loc}}(M)\). Then

\[
F^{N-1}(Fy)=F^N y
\]

for \(N\ge1\), so \(Fy\in W^s(M)\). If \(N=0\), local invariance gives \(Fy\in W^s_{\mathrm{loc}}(M)\), provided the image remains in the local tube. Hence

\[
F(W^s(M))
\subset
W^s(M).
\]

If \(F\) is a diffeomorphism on the relevant region and the required inverse iterates remain in the domain, then equality holds on this generated global stable set:

\[
F(W^s(M))=W^s(M).
\]

### H.5. Tracking estimate

Let \(y\in W^s(M)\), and choose \(N\) such that

\[
F^N y
\in W^s_{\mathrm{loc}}(p_N),
\qquad
p_N=
\pi^s_{\mathrm{loc}}(F^N y).
\]

Then

\[
\pi^s(y)=F^{-N}p_N.
\]

For \(n\ge N\), the local estimate gives

\[
\operatorname{dist}
\left(
F^n y,
F^n\pi^s(y)
\right)
=
\operatorname{dist}
\left(
F^{n-N}(F^N y),
F^{n-N}p_N
\right)
\le
C e^{-\gamma(n-N)}
\operatorname{dist}(F^N y,p_N).
\]

Thus every point in the generated stable set tracks the orbit of its phase point exponentially after it enters the local stable tube.

### H.6. Lamination structure and limitations

Each set \(W_N^s(M)=F^{-N}(W^s_{\mathrm{loc}}(M))\) inherits a lamination structure from the local stable lamination by pullback under the diffeomorphism \(F^N\). The global stable set is the increasing union of these pulled-back laminations. It is therefore naturally an immersed lamination. It is embedded only under additional global no-self-intersection or properness assumptions.

The unstable set is obtained analogously by applying the same construction to \(F^{-1}\). Transverse regularity of the global laminations and regularity of the global phase maps are not automatic; they require the same additional bunching assumptions as in the local theory.


---

## Appendix I. Uniform cohomological inverses on noncompact bases

This appendix gives a theorem-level version of the linear part of the noncompact extension. It shows precisely how compactness in Theorem 3.1 may be replaced by bounded geometry and uniform estimates.

### I.1. Setting and statement

Let \(M\) be a complete finite-dimensional \(C^{r+1}\) manifold with bounded geometry, and let \(E\to M\) be a \(C^{r+1}\) Banach bundle with bounded geometry: uniformly controlled local trivializations, uniformly bounded transition maps and derivatives up to order \(r+1\), and a uniformly bounded connection. Let

\[
f:M\to M
\]

be a \(C^{r+1}\) diffeomorphism with uniformly bounded derivatives of \(f\) and \(f^{-1}\) up to order \(r+1\). Let

\[
B_m:E_m\to E_{f(m)}
\]

be a \(C^r\) bundle automorphism with uniformly bounded derivatives up to order \(r\), preserving a \(C^r\) splitting

\[
E=E^s\oplus E^u
\]

with uniformly bounded projections and uniformly bounded derivatives up to order \(r\).

Assume a uniform exponential dichotomy: for every orbit \(m_n=f^n(m)\),

\[
\|\Phi^s(n,k)\|\le C\lambda^{n-k},
\qquad n\ge k,
\]

and

\[
\|\Phi^u(k,n)\|\le C\lambda^{n-k},
\qquad n\ge k,
\]

with constants independent of \(m\). Assume also uniform \(j\)-bunching for \(0\le j\le r\): there are constants \(C_j>0\) and \(\theta_j\in(0,1)\), independent of \(m\), such that

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m_n)\|^j
\le C_j\theta_j^n,
\qquad n\ge0,
\]

and

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|^j
\le C_j\theta_j^n,
\qquad n\ge0.
\]

Let \(C_b^k(M,E)\) denote the space of bounded \(C^k\) sections whose covariant derivatives up to order \(k\) are bounded and uniformly continuous in the bounded-geometry atlas. Then, for every \(0\le k\le r\),

\[
\mathcal A:C_b^k(M,E)\to C_b^k(M,f^*E),
\qquad
(\mathcal A\zeta)(m)=\zeta(f(m))-B_m\zeta(m),
\]

is an isomorphism, and

\[
\|\mathcal A^{-1}q\|_{C_b^k}
\le C_k\|q\|_{C_b^k}.
\]

### I.2. The \(C_b^0\) Green inverse

For \(q\in C_b^0(M,f^*E)\), define along the orbit \(m_n=f^n(m)\)

\[
q_n=q(m_n)\in E_{m_{n+1}}.
\]

Decompose in the target fibre,

\[
q_n^\sigma=P_{m_{n+1}}^\sigma q_n.
\]

Set

\[
\zeta_n^s
=
\sum_{j=-\infty}^{n-1}\Phi^s(n,j+1)q_j^s,
\]

and

\[
\zeta_n^u
=
-
\sum_{j=n}^{\infty}\Phi^u(n,j+1)q_j^u.
\]

The uniform dichotomy gives

\[
\|\zeta_n^s\|
\le
\frac{C\sup_m\|P_m^s\|}{1-\lambda}
\|q\|_{C_b^0},
\]

and the same estimate for the unstable term. Hence

\[
\|\mathcal Gq\|_{C_b^0}
\le C\|q\|_{C_b^0}.
\]

The same telescoping calculation as in Section 3 gives

\[
\mathcal A\mathcal Gq=q.
\]

A bounded homogeneous solution has vanishing stable part by taking the initial time to \(-\infty\), and vanishing unstable part by taking the terminal time to \(+\infty\). Thus the bounded solution is unique.

Uniform continuity follows because the summands are uniformly continuous in the bounded-geometry atlas, with a common exponential majorant. Uniform convergence of uniformly continuous summands gives a uniformly continuous sum. Therefore

\[
\mathcal G:C_b^0(M,f^*E)
\to
C_b^0(M,E)
\]

is a bounded inverse.

### I.3. Higher derivatives

The higher-order proof is the uniform version of Appendix A. Differentiating the cohomological equation in uniformly controlled charts gives, at order \(k\), a principal equation for the \(k\)-jet

\[
J\mapsto B_mJ\circ(Df(m)^{-1})^{\otimes k}.
\]

The stable part of the induced \(k\)-jet cocycle is bounded by

\[
\|\Phi^s(n,0)\|\,\|Df^{-n}(m_n)\|^k,
\]

and the backward unstable part by

\[
\|\Phi^u(-n,0)\|\,\|Df^n(m)\|^k.
\]

The uniform \(k\)-bunching hypothesis gives a uniform exponential dichotomy for the induced jet cocycle. Applying the \(C_b^0\) inverse to the induced equation yields

\[
\|D^k\zeta\|_{C_b^0}
\le C_k\|q\|_{C_b^k}
\]

after lower-order terms have been controlled by induction. The bounded-geometry assumptions guarantee that all connection coefficients, transition functions, and Faà di Bruno terms have uniform constants. Induction gives

\[
\|\mathcal Gq\|_{C_b^k}
\le C_k\|q\|_{C_b^k}.
\]

### I.4. Role in the noncompact extension

This theorem supplies the linear inverse needed for a noncompact graph transform or invariant-section theorem. The nonlinear step still requires a uniform tube, uniform admissible cones or matching estimates, and a graph transform whose contraction constants are independent of the base point. Those are exactly the additional hypotheses stated in Section 8.3.


---

## Appendix J. External two-sided HPS input and reduction to the manuscript's setting

This appendix records the exact role of the external HPS theorem in the proof. It does not reprove the two-sided Hadamard matching lemma. Instead, it states the structural theorem imported from the HPS/Banach-space invariant-manifold literature and verifies that the hypotheses in the body of the manuscript reduce to that theorem in tubular coordinates.

### J.1. External structural theorem

We use the following structural input.

**External HPS--Banach invariant-section theorem.** Let \(X\) be a Banach space and let \(M\subset X\) be a compact finite-dimensional \(C^{r+1}\) embedded submanifold without boundary. Let \(T\) be a \(C^{r+1}\) local diffeomorphism defined on a neighbourhood of \(M\), with

\[
T(M)=M.
\]

Assume that along \(M\) there is a complemented invariant splitting

\[
T_MX=TM\oplus N^s\oplus N^u
\]

and that the normal cocycle has an exponential dichotomy satisfying the required \(j\)-bunching inequalities for \(0\le j\le r\). Then every sufficiently small \(C^{r+1}\) local diffeomorphism \(\widetilde T\) close to \(T\), with uniform bounds on the relevant neighbourhood, admits a locally unique admissible \(C^r\) invariant graph \(\widetilde M\) near \(M\). In a parametrization \(\widetilde K:M\to X\), there is an internal map \(\widetilde f:M\to M\) such that

\[
\widetilde T\circ \widetilde K
=
\widetilde K\circ \widetilde f.
\]

The fixed point is obtained by the full two-sided admissible Hadamard graph transform. In particular, the compatibility of the forward and backward base correspondences is part of the theorem; it is not derived from separate stable-forward and unstable-backward component equations.

For finite-dimensional fibres this is the graph-transform theorem of Hirsch, Pugh, and Shub [2]. Banach-space versions and the corresponding graph-transform/Perron constructions are developed in Bates--Lu [4] and Bates--Lu--Zeng [9].

### J.2. Reduction from the present tubular-bundle formulation

The setting of the manuscript is a direct tubular-coordinate form of the theorem above. The ambient Banach space is the same \(X\). The compact finite-dimensional invariant manifold is \(M\subset X\). The split tubular embedding

\[
\Theta:U_E\to U_X\subset X
\]

identifies a neighbourhood of \(M\) in \(X\) with a neighbourhood of the zero section of the Banach bundle \(E\to M\). Under this identification the normal bundle is

\[
E=E^s\oplus E^u,
\]

and the invariant splitting

\[
T_mX=T_mM\oplus E_m^s\oplus E_m^u
\]

is precisely the normally hyperbolic splitting in the external theorem.

In tubular coordinates,

\[
\widehat F_\varepsilon(m,\eta)
=
(b_\varepsilon(m,\eta),g_\varepsilon(m,\eta)).
\]

For \(\varepsilon=0\),

\[
b_0(m,0)=f(m),
\qquad
 g_0(m,0)=0,
\]

and

\[
B_m=D_\eta g_0(m,0):E_m\to E_{f(m)}
\]

is the normal cocycle. The exponential dichotomy and the invariant bunching inequalities in Section 2.2 are exactly the normal hyperbolicity and bunching hypotheses of the external theorem.

The hypotheses that \(F_\varepsilon\) is \(C^{r+1}\), locally diffeomorphic, defined on a common tube, and sufficiently close to \(F_0\) provide the perturbation neighbourhood required in the external theorem. The strengthened estimates on

\[
r_\varepsilon(m,\eta)
=
g_\varepsilon(m,\eta)
-
\tau_{b_\varepsilon(m,\eta)\leftarrow f(m)}B_m\eta
\]

are the transported-coordinate form of the usual small nonlinear remainder assumptions used in the graph-transform proof.

Thus the external theorem gives an admissible \(C^r\) graph in tubular coordinates:

\[
M_\varepsilon=
\{(m,h_\varepsilon(m)):m\in M\},
\qquad
h_\varepsilon\in\Gamma^r(E),
\]

with internal map

\[
f_\varepsilon(m)=b_\varepsilon(m,h_\varepsilon(m)),
\]

satisfying the local graph equation

\[
F_\varepsilon(m,h_\varepsilon(m))
=
(f_\varepsilon(m),h_\varepsilon(f_\varepsilon(m))).
\]

This is the conclusion of Theorem 4.1. The global equality

\[
F_\varepsilon(M_\varepsilon)=M_\varepsilon
\]

used in Theorem 5.1 follows afterward from the compact-manifold argument showing that \(f_\varepsilon\) is a global diffeomorphism.

### J.3. Why the componentwise substitute is excluded

A transform that separately enforces only

\[
g_+^s(m,h(m))=h^s(\beta_h^+(m))
\]

and

\[
g_-^u(m,h(m))=h^u(\beta_h^-(m))
\]

is not the HPS transform. Such component equations do not force

\[
\beta_h^-\circ\beta_h^+=\operatorname{id}_M.
\]

Affine examples can satisfy those separate component equations while failing the full graph equation. The external HPS theorem avoids this defect because the transformed graph is defined by simultaneous admissible stable/unstable matching, and the compatibility of the base correspondences is part of that theorem.

---

## Appendix K. Fractional jet spectra for Banach-bundle cohomological equations

This appendix sharpens the linear cohomological inverse theorem in the Hölder scale. The result is independent of the nonlinear HPS matching mechanism: it concerns only the Green inverse for \(\mathcal A\). The integer bunching assumptions in the main text are sufficient criteria; the intrinsic condition is the spectral radius of the exact Green summand operators acting on Hölder jet sections.

### K.1. Hölder Banach-bundle setting

Let \(M\) be a compact finite-dimensional \(C^{r+1,\beta}\) manifold without boundary, where \(0<\beta\le1\). Let \(E\to M\) be a \(C^{r+1,\beta}\) Banach bundle. Fix either a \(C^{r,\beta}\) connection or a finite \(C^{r+1,\beta}\) bundle atlas with uniformly controlled transition maps.

Let

\[
f\in\operatorname{Diff}^{r+1,\beta}(M),
\]

and let

\[
B_m:E_m\to E_{f(m)}
\]

be a \(C^{r,\beta}\) bundle automorphism. Assume a \(C^{r,\beta}\) invariant splitting

\[
E=E^s\oplus E^u
\]

with uniformly bounded \(C^{r,\beta}\) projections. Assume that \(B\) has a uniform exponential dichotomy over \(f\).

Let

\[
s=k+\alpha,
\qquad
0<\alpha<1,
\]

where \(k\) is a nonnegative integer and

\[
k+\alpha\le r+\beta.
\]

The space \(C^{k,\alpha}(M,E)\) is defined using the fixed connection or finite atlas. For \(k=0\), this is the usual Hölder section space \(C^\alpha(M,E)\).

---

### K.2. Hölder Green summand operators

Let

\[
\mathcal J_k(E):=
\operatorname{Sym}^k(T^*M;E)
\]

be the bundle of symmetric \(k\)-linear covariant tensors with values in \(E\). For \(k=0\), set \(\mathcal J_0(E)=E\).

The principal \(k\)-jet cocycle over \(f\) is

\[
\mathscr B_k(m)J
=
B_m\circ J\circ(Df(m)^{-1})^{\otimes k},
\]

mapping \(\mathcal J_k(E)_m\) to \(\mathcal J_k(E)_{f(m)}\).

The stable Green summand of length \(n\) is the operator

\[
\mathcal S_{k,n}^+:
C^\alpha(M,
\mathcal J_k(E)^s)
\to
C^\alpha(M,
\mathcal J_k(E)^s)
\]

which assigns to a jet-forcing section its stable contribution transported from time \(-n\) to time \(0\). In local notation,

\[
(\mathcal S_{k,n}^+Q)(m)
=
\Phi^s(0,-n;m)
\,Q(f^{-n}m)
\circ
(Df^{-n}(m))^{\otimes k},
\]

with the appropriate bundle transports and projections included. Similarly, the unstable Green summand of length \(n\) is

\[
\mathcal S_{k,n}^-:
C^\alpha(M,
\mathcal J_k(E)^u)
\to
C^\alpha(M,
\mathcal J_k(E)^u),
\]

with local form

\[
(\mathcal S_{k,n}^-Q)(m)
=
\Phi^u(0,n;m)
\,Q(f^n m)
\circ
(Df^{n}(m))^{\otimes k}.
\]

These definitions are invariantly interpreted using the fixed connection or atlas. Their operator norms on \(C^\alpha\) include all Hölder variation of cocycle products, projections, derivative iterates, and transports.

Define the fractional jet radii

\[
\widehat\rho_{k,\alpha}^+
=
\limsup_{n\to\infty}
\|\mathcal S_{k,n}^+\|_{C^\alpha\to C^\alpha}^{1/n},
\]

and

\[
\widehat\rho_{k,\alpha}^-
=
\limsup_{n\to\infty}
\|\mathcal S_{k,n}^-\|_{C^\alpha\to C^\alpha}^{1/n}.
\]

Set

\[
\widehat\rho_{k,\alpha}
=
\max\{
\widehat\rho_{k,\alpha}^+,
\widehat\rho_{k,\alpha}^-
\}.
\]

---

### K.3. Fractional cohomological inverse theorem

**Theorem K.1. Hölder jet-spectrum inverse.**

Assume the \(C^0\) exponential dichotomy. Let \(k+\alpha\le r+\beta\), with \(0<\alpha<1\). If

\[
\widehat\rho_{k,\alpha}<1,
\]

then

\[
\mathcal A:
C^{k,\alpha}(M,E)
\to
C^{k,\alpha}(M,f^*E),
\qquad
(\mathcal A\zeta)(m)=
\zeta(f(m))-B_m\zeta(m),
\]

is an isomorphism. Moreover,

\[
\|\mathcal A^{-1}q\|_{C^{k,\alpha}}
\le
C_{k,\alpha}
\|q\|_{C^{k,\alpha}}.
\]

The same statement holds on noncompact bounded-geometry bases in \(C_b^{k,\alpha}\) spaces if all geometric and operator-norm estimates are uniform.

---

### K.4. Proof of Theorem K.1

#### K.4.1. Zeroth-order inverse

The \(C^0\) inverse is the ordinary Green operator. Along an orbit \(m_n=f^n(m)\), write

\[
q_n=q(m_n)\in E_{m_{n+1}}.
\]

Decompose in the target fibre:

\[
q_n^\sigma=P_{m_{n+1}}^\sigma q_n.
\]

The unique bounded solution of

\[
\zeta_{n+1}-B_{m_n}\zeta_n=q_n
\]

is

\[
\zeta_n^s
=
\sum_{j=-\infty}^{n-1}
\Phi^s(n,j+1)q_j^s,
\]

and

\[
\zeta_n^u
=
-
\sum_{j=n}^{\infty}
\Phi^u(n,j+1)q_j^u.
\]

This gives a bounded inverse on \(C^0\), and uniqueness follows from the usual bounded homogeneous-solution argument.

#### K.4.2. Hölder Green lemma

We use the following abstract observation. Let \(F\to M\) be a \(C^\alpha\) Banach bundle and let \(C_m:F_m\to F_{f(m)}\) be a cocycle with a \(C^0\) exponential dichotomy. Suppose the exact stable and unstable Green summand operators on \(C^\alpha\) sections satisfy

\[
\limsup_{n\to\infty}
\|\mathcal S_n^+\|_{C^\alpha\to C^\alpha}^{1/n}<1,
\]

and

\[
\limsup_{n\to\infty}
\|\mathcal S_n^-\|_{C^\alpha\to C^\alpha}^{1/n}<1.
\]

Then the Green operator is bounded on \(C^\alpha\).

Indeed, choose \(\theta<1\) larger than both limsup values. Then, for all sufficiently large \(n\),

\[
\|\mathcal S_n^\pm\|_{C^\alpha\to C^\alpha}
\le
C\theta^n.
\]

The finitely many small \(n\) terms are harmless, and the Green series is a normally convergent series in the Banach space \(C^\alpha(M,F)\). This proves the bounded \(C^\alpha\) estimate.

#### K.4.3. Application to the \(k\)-jet equation

For the cohomological equation

\[
\zeta\circ f-B\zeta=q,
\]

the \(k\)-th covariant derivative has principal part

\[
D^k\zeta(f(m))
\circ Df(m)^{\otimes k}
-
B_mD^k\zeta(m).
\]

Equivalently, with \(J=D^k\zeta\),

\[
J(f(m))-\mathscr B_k(m)J(m)=Q_k(m),
\]

where \(Q_k\) contains \(D^kq\) and lower-order terms involving derivatives of \(f\), \(B\), the connection, and \(\zeta\) up to order \(k-1\).

The integer \(C^k\) cohomological inverse theorem gives

\[
\|\zeta\|_{C^k}
\le
C_k\|q\|_{C^k}.
\]

Because \(q\in C^{k,\alpha}\), and because the data have regularity at least \(C^{k,\alpha}\), the lower-order terms satisfy

\[
\|Q_k\|_{C^\alpha}
\le
C_{k,\alpha}\|q\|_{C^{k,\alpha}}.
\]

By definition, the stable and unstable Green summands for the \(k\)-jet equation have radii bounded by \(\widehat\rho_{k,\alpha}<1\). The Hölder Green lemma therefore gives

\[
\|D^k\zeta\|_{C^\alpha}
\le
C_{k,\alpha}\|Q_k\|_{C^\alpha}
\le
C_{k,\alpha}
\|q\|_{C^{k,\alpha}}.
\]

Together with the integer estimate, this yields

\[
\|\zeta\|_{C^{k,\alpha}}
\le
C_{k,\alpha}\|q\|_{C^{k,\alpha}}.
\]

#### K.4.4. Avoiding circular differentiability

Let \(G_Nq\) denote the Green series truncated at orbit lengths at most \(N\). Since the summands are \(C^{k,\alpha}\), each \(G_Nq\) is \(C^{k,\alpha}\). The argument above applies uniformly to the finite sums and shows that \(G_Nq\) is Cauchy in \(C^{k,\alpha}\). The uniform limit is the \(C^0\) Green solution \(Gq\). Hence \(Gq\in C^{k,\alpha}\), and the estimate follows. This avoids assuming differentiability of the \(C^0\) solution in advance.

Uniqueness in \(C^{k,\alpha}\) follows from uniqueness in \(C^0\). Thus \(\mathcal A\) is an isomorphism on \(C^{k,\alpha}\).

---

### K.5. Relation with one-step Hölder bunching

A stronger but more concrete sufficient condition is obtained by estimating the exact operator norms \(\|\mathcal S_{k,n}^\pm\|_{C^\alpha\to C^\alpha}\). If the cocycle products, projections, derivative iterates, and bundle transports have bounded distortion so that

\[
\|\mathcal S_{k,n}^+\|_{C^\alpha\to C^\alpha}
\le
C\theta^n
\]

and

\[
\|\mathcal S_{k,n}^-\|_{C^\alpha\to C^\alpha}
\le
C\theta^n
\]

for some \(\theta<1\), then \(\widehat\rho_{k,\alpha}<1\). In particular, the usual pointwise real-order bunching inequalities imply the theorem when supplemented by the corresponding bounded-distortion estimates for the iterated jet cocycles.

Thus the operator radius is the intrinsic formulation, while one-step norm-bunching is a convenient sufficient condition in adapted settings.

---

### K.6. Periodic jet-resonance obstruction

Let \(p\) be a periodic point of prime period \(N\). Let

\[
\mathfrak J_{\le k,p}
=
\bigoplus_{j=0}^{k}
\operatorname{Sym}^j(T_p^*M;E_p)
\]

be the full jet space up to order \(k\). The full triangular jet return map of the cohomological equation is the operator

\[
\mathfrak R_{\le k}(p):
\mathfrak J_{\le k,p}
\to
\mathfrak J_{\le k,p}.
\]

Its diagonal order-\(j\) block is the principal jet return map

\[
\mathscr R_j(p)J
=
\Phi(N,0;p)
\circ J\circ
(Df^N(p)^{-1})^{\otimes j}.
\]

Lower-order jet terms appear in the upper triangular blocks.

**Proposition K.2. Periodic jet-resonance obstruction.**

Assume the zeroth-order normal cocycle has an exponential dichotomy, so that \(\mathcal A\) is invertible on \(C^0\). If, for some periodic point \(p\),

\[
I-
\mathfrak R_{\le k}(p)
\]

is not surjective, then

\[
\mathcal A:C^k(M,E)	o C^k(M,f^*E)
\]

is not surjective.

If all lower-order blocks are nonresonant and

\[
I-
\mathscr R_k(p)
\]

is not surjective, the same conclusion follows.

#### Proof

Suppose \(\mathcal A:C^k(M,E)	o C^k(M,f^*E)\) were onto. Choose a finite jet datum for \(q\) along the periodic orbit such that the induced right-hand side in the periodic jet equation lies outside the range of

\[
I-
\mathfrak R_{\le k}(p).
\]

This is possible because the latter operator is not surjective. Since the periodic orbit is finite and \(M\) is finite-dimensional, a \(C^k\) section realizing these finite jets exists by a local bump-function construction in disjoint coordinate charts.

Let \(\zeta\in C^k(M,E)\) solve \(\mathcal A\zeta=q\). Taking jets of order \(\le k\) along the periodic orbit gives a linear periodic system. Iterating around the orbit yields

\[
(I-
\mathfrak R_{\le k}(p))Z=Q,
\]

where \(Z\) is the jet of \(\zeta\) at \(p\), and \(Q\) is the prescribed jet datum of \(q\). This contradicts the choice of \(Q\). Hence \(\mathcal A\) is not onto on \(C^k\).


---

### K.7. Compact return maps and Fredholm resonance

The obstruction in Proposition K.2 is stated as failure of surjectivity of

\[
I-\mathfrak R_{\le k}(p).
\]

In general Banach spaces this is the correct formulation: non-surjectivity need not be caused by an eigenvector. In compact or smoothing settings, however, the obstruction becomes an ordinary eigenvalue resonance.

**Theorem K.3. Compact jet-return Fredholm alternative.** Let \(Y\) be a Banach space and let \(K:Y\to Y\) be compact. If \(I-K\) is not surjective, then \(1\) is an eigenvalue of \(K\), with finite algebraic multiplicity.

Consequently, if the periodic jet-return operator

\[
\mathfrak R_{\le k}(p):\mathfrak J_{\le k,p}\to\mathfrak J_{\le k,p}
\]

is compact and if

\[
I-\mathfrak R_{\le k}(p)
\]

is not surjective, then there exists a nonzero jet

\[
J\in\mathfrak J_{\le k,p}
\]

such that

\[
\mathfrak R_{\le k}(p)J=J.
\]

Thus, in compact-return settings, the periodic obstruction is an eigenvalue-one resonance of finite algebraic multiplicity.

The proof is the Riesz--Schauder theorem: if \(I-K\) is not surjective, then \(I-K\) is not invertible, so \(1\in\sigma(K)\). Since \(1\ne0\) and \(K\) is compact, \(1\) is an eigenvalue of finite algebraic multiplicity.

**Corollary K.4. Parabolic compact-return case.** Assume a parabolic or smoothing setting in which the linear time-return map along a periodic orbit is compact on the chosen normal fibre space, for example because the sectorial generator has compact resolvent and the return time is positive. Since the tangent jet factors are finite-dimensional, the induced finite jet-return map \(\mathfrak R_{\le k}(p)\) is compact on the Banach jet fibre. Therefore any failure of surjectivity of \(I-\mathfrak R_{\le k}(p)\) is equivalent to the existence of an eigen-jet with eigenvalue \(1\).

Without compactness, Proposition K.2 should not be strengthened in this way: the obstruction may lie in point, continuous, or residual spectrum. The correct general statement remains non-surjectivity of \(I-\mathfrak R_{\le k}(p)\).

---

### K.8. Witness: first-jet resonance on a two-cycle

Let the base have a two-cycle and consider scalar fibres. Take normal multipliers

\[
B_0=B_1=\frac12
\]

and tangent derivatives

\[
Df_0=Df_1=\frac12.
\]

The \(C^0\) cohomological matrix is

\[
\begin{pmatrix}
-1/2&1\\
1&-1/2
\end{pmatrix},
\]

whose determinant is

\[
-\frac34\ne0.
\]

Thus the \(C^0\) equation is invertible. But the first-jet matrix is

\[
\begin{pmatrix}
-1&1\\
1&-1
\end{pmatrix},
\]

whose determinant is zero. The first-jet return map has eigenvalue one, so the \(C^1\) cohomological equation is not onto. This is the simplest periodic jet-resonance obstruction.

---

### K.9. Regularity spectrum

Define

\[
s_*=\sup\{k+\alpha:
\widehat\rho_{k,\alpha}<1\}.
\]

Then the Green inverse is bounded on every noninteger Hölder space \(C^{k,\alpha}\) with

\[
k+\alpha<s_*
\]

for which the data have the required regularity. Periodic jet resonances obstruct surjectivity at resonant integer orders. Thus the fractional jet spectrum describes the linear regularity threshold for the cohomological inverse.


### K.10. Model examples

#### K.10.1. Hyperbolic toral base with scalar attracting normal direction

Let

\[
A=
\begin{pmatrix}
2&1\\
1&1
\end{pmatrix}
\]

act on \(\mathbb T^2\). Its expanding eigenvalue is

\[
\Lambda=\frac{3+\sqrt5}{2}>1.
\]

Let \(E=\mathbb T^2\times\mathbb R\), and let the normal cocycle be scalar multiplication by

\[
0<\lambda<1.
\]

Then the cohomological equation is

\[
\zeta(Ax)-\lambda\zeta(x)=q(x).
\]

The stable Green summands at real order \(s=k+\alpha\) have growth rate

\[
\widehat\rho_s=
\lambda\Lambda^s.
\]

Consequently the Green inverse is bounded on every \(C^s\) space with

\[
s<\frac{\log(1/\lambda)}{
\log\Lambda}.
\]

Thus the regularity threshold is

\[
s_*=
\frac{\log(1/\lambda)}{
\log\Lambda}.
\]

If \(\lambda=\Lambda^{-N}\) for an integer \(N\), then the principal order-\(N\) jet return map at the fixed point \(0\in\mathbb T^2\) has eigenvalue one. Hence the periodic jet-resonance obstruction applies at order \(N\). This gives an explicit family where the fractional spectrum predicts the loss of integer-order surjectivity at the threshold.

#### K.10.2. Isometric base dynamics

If \(f\) is an isometry and the bundle transports, projections, and cocycle products have uniformly bounded Hölder constants, then

\[
\operatorname{Lip}(f^{\pm n})=1.
\]

For a scalar normally attracting cocycle \(B_m=\lambda\), \(0<\lambda<1\), the fractional radius is simply

\[
\widehat\rho_s=\lambda
\]

for all \(s\) allowed by the regularity of the data. Thus the cohomological inverse loses no regularity beyond the regularity already present in the coefficients. This contrasts with the hyperbolic toral example, where tangent distortion creates a finite regularity threshold.

---

---

## References

[1] N. Fenichel, *Geometric singular perturbation theory for ordinary differential equations*, Journal of Differential Equations 31 (1979), 53–98.

[2] M. Hirsch, C. Pugh, M. Shub, *Invariant Manifolds*, Lecture Notes in Mathematics 557, Springer, 1977.

[3] S.-N. Chow, X.-B. Lin, K. Lu, *Fenichel theory for infinite-dimensional semi-flows*, Journal of Differential Equations 162 (2000), 1–53.

[4] P. W. Bates, K. Lu, *Persistence of invariant manifolds for partial differential equations*, Journal of Differential Equations 117 (1995), 481–525.

[5] D. Henry, *Geometric Theory of Semilinear Parabolic Equations*, Lecture Notes in Mathematics 840, Springer, 1981.

[6] K. J. Palmer, *Exponential dichotomies and transversal homoclinic points*, Journal of Differential Equations 38 (1980), 225–256.

[7] D. Ruelle, *Characteristic exponents and invariant manifolds in Hilbert space*, Publications Mathématiques de l'IHÉS 51 (1980), 239–277.

[8] R. S. Hamilton, *The inverse function theorem of Nash and Moser*, Bulletin of the American Mathematical Society 7 (1982), 65–222.

[9] P. W. Bates, K. Lu, C. Zeng, *Existence and persistence of invariant manifolds for semiflows in Banach space*, Memoirs of the American Mathematical Society 135, no. 645, 1998.