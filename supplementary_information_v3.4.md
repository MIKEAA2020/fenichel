# Supplementary Information

## Cohomological Inverses and Fractional Jet Spectra in Banach-Space Normally Hyperbolic Persistence

**Author:** Amin Abaee — independent researcher, Tehran, Iran.  
**Date:** 2026-11-20  
**Primary manuscript:** main_manuscript_v3.4 (main text)  

---

## Declaration

**Funding.** None.  
**Competing interests.** None.  
**AI use.** Ernie (Baidu) and Deepseek AI assisted with computations, numerical checks and literature review. The author reviewed and edited the outputs and takes full responsibility for the work.

---

## Appendices

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
\sup_m\|L_m^s\|+\sup_m\|L_m^u\|
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
\varepsilon_0)\times U\to Y_r,
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

This appendix records the exact role of the external HPS theorem in the proof. It does not reprove the two-sided Hadamard matching lemma. Instead, it states the structural theorem imported from the HPS/Banach-space invariant-manifold literature and verifies that the hypotheses in the body of the manuscript reduce to that theorem in tubular coordinates. The imported structural input supplies the two-sided invariant sections whose existence and regularity is established by Theorems 5.3–5.6; these theorems guarantee the admissible invariant graphs that feed into the HPS reduction. The compatibility of forward and backward base correspondences is part of the imported theorem; it is not derived from separate stable-forward and unstable-backward component equations.

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

**Mapping to manuscript theorems.** The external structural theorem supplies the two-sided admissible invariant sections whose existence and uniqueness are established by **Theorem 5.3** (two-sided invariant section theorem), which guarantees the admissible invariant graph and its normal bundle splitting. **Theorem 5.4** extends this to the compact persistence theorem via the normal bundle construction of Appendix A/B. **Theorem 5.5** proves parameter regularity (Lipschitz and differentiability-with-loss) of the invariant section using the parameter expansions of Appendix F. **Theorem 5.6** addresses sharpness in skew-product and toral classes, using the fractional jet-spectrum results of Appendix K. The present tubular-bundle formulation of Sections 5.1–5.3 is a direct reduction of the external structural theorem to the Banach-bundle setting of the manuscript.

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
\mathcal A:C^k(M,E)\to C^k(M,f^*E)
\]

is not surjective.

If all lower-order blocks are nonresonant and

\[
I-
\mathscr R_k(p)
\]

is not surjective, the same conclusion follows.

#### Proof

Suppose \(\mathcal A:C^k(M,E)\to C^k(M,f^*E)\) were onto. Choose a finite jet datum for \(q\) along the periodic orbit such that the induced right-hand side in the periodic jet equation lies outside the range of

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
\tag{K.9.1}
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

