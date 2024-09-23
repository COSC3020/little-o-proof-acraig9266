I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

# Little-o

In addition to the big-O, big-$\Omega$, and big-$\Theta$ notation that
we covered at the beginning of this class, a few other notations are sometimes
used in asymptotic analysis.  For example, "little-$o$" notation.

Prove (i.e.\ give a formal mathematical proof) that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.

Hint: The proof will be *very* short and *very* easy. You can start by
identifying the differences between the definitions of O and o.

I have started with the formal definition of $o$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$f(n)\in o(g(n)) \iff \forall c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

$f(n)\in O(g(n)) \iff \exists c>0, \exists n_0, \forall n\ge n_0: f(n) < c g(n)$

Examining the definitions of O and o it can be seen the only difference is that o requires \iff \forall c > 0 to be satisfied whereas O requires only \iff \exists c > 0 to be satisfied.
So, let c be a randomly selected constant that satisfies the definition of o for some function f(n). Since c satisfies the definition of o, it must be positive (c > 0). Since c is a positive constant it satisfies \iff \exists c>0 from the definition of O. Since all other requirements for o and O are the same, all requirements are now met proving that $f(n)\in o(g(n))$ implies
that $f(n)\in O(g(n))$.
