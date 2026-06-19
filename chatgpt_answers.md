# ChatGPT — Answers
**Score: 88/100** 4️⃣

---

## Q1. Prove there are infinitely many prime numbers

Assume finitely many primes p₁, p₂, …, pₙ.

Let N = p₁ · p₂ · … · pₙ + 1.

N is either prime or has a prime factor not in the list. Either way, our list is incomplete. Contradiction.

Therefore infinitely many primes exist. ∎

---

## Q2. Find all integer solutions of x² − y² = 2025

Factor: (x+y)(x−y) = 2025

Let a = x+y, b = x−y. Then x = (a+b)/2, y = (a−b)/2.

2025 = 3⁴ × 5² has 15 positive divisors. All odd → parity condition met.

**Some solutions:**

| a | b | x | y |
|------|---|-----|-----|
| 2025 | 1 | 1013 | 1012 |
| 675 | 3 | 339 | 336 |
| 405 | 5 | 205 | 200 |
| 225 | 9 | 117 | 108 |
| 135 | 15 | 75 | 60 |
| 81 | 25 | 53 | 28 |
| 45 | 45 | 45 | 0 |

With negatives: **28 integer solutions** (note: count may vary by methodology).

---

## Q3. Evaluate ∫₀^∞ x·e^(−x) dx

Integration by parts: u = x, dv = e^(−x)dx

= [−xe^(−x)]₀^∞ + [−e^(−x)]₀^∞ = 0 + 1 = **1** ✓

---

## Q4. Eigenvalues of a real symmetric matrix are real

Suppose Av = λv, v ≠ 0. Multiply by v*:

v*Av = λ‖v‖²

Since A = Aᵀ and real, v*Av is real. Hence λ is real. ∎

---

## Q5. Expected number of tosses until two consecutive heads

Let E = expected tosses from start, F = expected tosses given last was H.

E = 1 + ½F + ½E  →  E = 2 + F  
F = 1 + ½·0 + ½E

Solving: E = **6** ✓

---

## Q6. Circular arrangements of 8 people

Fix one seat to account for rotational symmetry. Remaining 7 people: 7! = **5040** ways. ∎

---

## Q7. Every finite group of prime order is cyclic

Take g ≠ e in G. |⟨g⟩| divides |G| = p. So |⟨g⟩| = p = |G|. Hence G = ⟨g⟩ is cyclic. ∎

---

## Q8. Limit of aₙ = n/(n+1)

|n/(n+1) − 1| = 1/(n+1) < ε when n > 1/ε − 1.

Choose N = ⌈1/ε⌉. Then for n > N: |aₙ − 1| < ε.

∴ limit = 1. ∎

---

## Q9. Tree with n vertices has n−1 edges

Induction: base case n=1: 0 edges ✓

Inductive step: tree with n+1 vertices has a leaf; remove it and its edge → tree with n vertices (n−1 edges by IH) → total = n edges = (n+1)−1. ∎

---

## Q10. Verification process for claimed RH proof

1. **Check the statement** — confirm proof targets Re(s) = ½ for nontrivial zeros.
2. **Line-by-line review** by number theorists.
3. **Check for common errors**: illegal limit swaps, divergent series treated as convergent, circular reasoning.
4. **Formalize** in proof assistant (Lean or Coq) if feasible.
5. **Numerical check** — verify consistency with known zeros.
6. **Publish** for open community review.
7. **Consensus** — accept only after sustained scrutiny with no open objections.
