## Heuristics for the distribution of lambda invariants of elliptic curves

### 20151210 What is this file?

Much like [weber](https://github.com/daniel3735928559/wip-weber), this
file will be used to collect the existing notes and code around this
project, hopefully soon bringing this file up to the present.
Thereafter, I'll try to use it as a place to store sanitised versions
of my notes.

New entries will be added to the end of this file.

### 20151211 Recap of problem context and statement:

Lambda invariants of number fields are a kind of "stable" version of
the class number for p-adic families.  EJV describe a function field
analogue of this phenomenon and use this to set up heuristics for what
the lambda invariants of imaginary quadratic number fields should be,
and give some computations in support of these heuristics.

The question posed by Ellenberg is to do the same for elliptic curves,
where lambda invariants now describe the growth of Sha rather than of
class groups but are again the sort of "stable" version of this for
p-adic families.

### 20151212 Organising the possible directions and subproblems

#### mu-invariant:

See, for example, [This paper of
Sujatha](http://www.math.tifr.res.in/~sujatha/win.pdf):

E = X_0(11): y^2 + y = x^3 - x^2 - 10x - 20, p = 5, then mu = 2

Greenberg conjectures for any E/Q, p > 2, that E is isogenous to an E' with mu(E') = 0.

For example, see Greenberg-Vatsal: 

E, E_1, E_2 ell. curves, p a prime of good ordinary reduction (of all):

If E_1[p] isom E_2[p] as Galois modules, then mu_1 = = iff mu_2 = 0
If E has a cyclic isog. of deg p^t whose kernel is ramified (I_p acts non-trivially) and odd (complex conj acts as -1), then mu >= t
If E has cyclic isog. of deg. p, kernel unramified and odd or ramified and even, mu = 0.

Main conjecture: mu^alg = mu^an, lambda^alg = lambda^an

Can sometimes study non-primitive invariants and access information
about primitive invariants that way.  See also:
[Barman-Saikia](http://www.kurims.kyoto-u.ac.jp/EMIS/journals/em/docs/boletim/vol413/v41.3.a5.2010.pdf0

#### Numerical computation:

Analytic:
Using Pollack et al modular symbols code
Using interpolation of complex values
Mazur-Tate elements

Algebraic:
???

#### Heuristic from function fields:

[U0] Douglas Ulmer ECs over FFs

1.9.3:

E an EC of conductor n over K = K(C), C a curve of genus g, then:

L(E, s) = P(q^-s) polynomial of degree N = 4g - 4 + deg(n), and

L(E,s) = product i from 1 to N (1 - alpha_i q^-s)

where alpha_i has absolute value q in every complex embedding, and the set of alpha_i is invariant under (alpha mapsto q^2/alpha) (functional equation).

(How is this consistent with the previous computation for constant curves?)

#### Heuristic a la Poonen Rains: