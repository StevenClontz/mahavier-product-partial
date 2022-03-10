# Counting the Uncountable
### or, How I Learned to Stop Worrying and Love Elementary Submodels

**[STDC 2022 @ Baylor University](https://sites.baylor.edu/topology-conference)**

Steven Clontz | University of South Alabama

*Joint work with Will Brian* | *Slides at* [clontz.org](https://clontz.org)

---

## Abstract 1/2

Consider the following two-player game. Let \\(W\\) be some subset of the reals.
During the initial round, Alice chooses \\(-\infty\\) and Bob chooses
\\(+\infty\\). Then each subsequent move of either player is a real number
strictly between the two most recently chosen numbers.
After \\(\omega\\)-many rounds, Alice wins this game provided that some number
in \\(W\\) is both greater than all her choices and less than all Bob's choices.

---

## Abstract 2/2

Bob has a winning strategy in this game if and only if \\(W\\) is countable.
To see this, we will demonstrate two proofs accessible to a general mathematical 
audience, one utilizing countable elementary submodels, and the other involving
limited information strategies.

---

## Baker's Game

<div style="height:75vh"></div>

---

## History of Baker's Game 1/2

- Based upon a game defined in 1998 by Grossman, Turett
  for [Mathematics Magazine problem #1542][MathMagProb], which was
  solved by Newcomb in [1999][MathMagSol].

[MathMagProb]: https://www.jstor.org/stable/i326797
[MathMagSol]: https://www.jstor.org/stable/i326802

---

## History of Baker's Game 2/2

- Named for Matt Baker, who in [2007][MathMagBaker] showed several basic results:
    - If \\(W\subseteq\mathbb R\\) is countable, then Bob has a winning strategy.
      <!-- .element: class="fragment" -->
    - If \\(W\subseteq\mathbb R\\) is perfect (non-empty, closed, all points are
      limits), then Alice has a winning strategy.
      <!-- .element: class="fragment" -->
    - Therefore, we have a neat game-theoretic proof that the reals (which are
      perfect) are uncountable.
      <!-- .element: class="fragment" -->

[MathMagBaker]: https://www.jstor.org/stable/27643064

---

## Baker's Question

-   The proof that Bob wins for a countable set \\(W\\) is pretty quick:
    -   <!-- .element: class="fragment" -->
        Enumerate \\(W=\\{w_n:n&lt;\omega\\}\\), and on Bob's \\(n\\)th move
        he can play a number that prevents \\(w_n\\) from being between
        their moves at the end of the game.
-   <!-- .element: class="fragment" -->
    Does there exist an uncountable set \\(W\\) that allows Bob a winning
    strategy?
    - <!-- .element: class="fragment" -->
        Will Brian emailed me in January: Nope.

---
<!-- .slide: data-transition="slide-in fade-out" -->

## Sketch of a Proof

<div style="font-size:0.9em">

-   <!-- .element: class="fragment" -->
    Let \\(\\sigma\\) be a strategy for Bob that only uses rationals.
    Assume Alice only plays rationals. Say \\(x\\) is *legal* if
    it is between all prior moves of both players.
-   <!-- .element: class="fragment" -->
    For each partial playthrough \\(t\\), define
    \\[E_t = \\{x\\text{ legal}|a&lt;x\\Rightarrow\\sigma(t^\\frown\\langle{a}\\rangle)\\leq x\\}\\]
-   <!-- .element: class="fragment" -->
    \\(E_t\\) cannot contain bounded decreasing subsequences, as Alice picking infimum
    creates a contradiction.
-   <!-- .element: class="fragment" -->
    For \\(w\\) not in \\(\bigcup_t E_t\\) (countable), Alice can ensure \\(w\\) remains legal
    the whole game. If \\(w\\in W\\), Alice wins!

</div>

---
<!-- .slide: data-transition="fade" -->

## Sketchy Proof 🙃

<div style="font-size:0.9em">

-   <!-- .element: class="" -->
    Let \\(\\sigma\\) be a strategy for Bob that only uses rationals.
    Assume Alice only plays rationals. Say \\(x\\) is *legal* if
    it is between all prior moves of both players.
-   <!-- .element: class="" -->
    For each partial playthrough \\(t\\), define
    \\[E_t = \\{x\\text{ legal}|a&lt;x\\Rightarrow\\sigma(t^\\frown\\langle{a}\\rangle)\\leq x\\}\\]
-   <!-- .element: class="" -->
    \\(E_t\\) cannot contain bounded decreasing subsequences, as Alice picking infimum
    creates a contradiction.
-   <!-- .element: class="" -->
    For \\(w\\) not in \\(\bigcup_t E_t\\) (countable), Alice can ensure \\(w\\) remains legal
    the whole game. If \\(w\\in W\\), Alice wins!

</div>

---
<!-- .slide: data-transition="fade-in slide-out" -->

## Sketchy Proof 😲

<div style="font-size:0.9em">

-   <!-- .element: class="" -->
    Let \\(\\sigma\\) be a strategy for Bob that only uses rationals.
    **Assume Alice only plays rationals.**<!-- .element: style="color:cyan" -->
    Say \\(x\\) is *legal* if
    it is between all prior moves of both players.
-   <!-- .element: class="" -->
    For each partial playthrough \\(t\\), define
    \\[E_t = \\{x\\text{ legal}|a&lt;x\\Rightarrow\\sigma(t^\\frown\\langle{a}\\rangle)\\leq x\\}\\]
-   <!-- .element: class="" -->
    \\(E_t\\) cannot contain bounded decreasing subsequences, as 
    **Alice picking infimum**<!-- .element: style="color:cyan" -->
    creates a contradiction.
-   <!-- .element: class="" -->
    For \\(w\\) not in \\(\bigcup_t E_t\\) (countable), Alice can ensure \\(w\\) remains legal
    the whole game. If \\(w\\in W\\), Alice wins!

</div>

---

## Will's Response

"Ah, well, we can work around that."

<div class="fragment">
    <p>
"We can just use a countable elementary submodel."
    </p>
</div>
<div class="fragment"><iframe src="https://giphy.com/embed/vNrFmUK6KZMPK" width="480" height="339" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p style="font-size:0.5em"><a href="https://giphy.com/gifs/fonzie-the-fonz-gif-stories-vNrFmUK6KZMPK">via GIPHY</a></p>
</div>

---

## My initial reaction

<iframe src="https://giphy.com/embed/9Fticsj7froxbpd5Sg" width="480" height="400" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p style="font-size:0.5em"><a href="https://giphy.com/gifs/theoffice-9Fticsj7froxbpd5Sg">via GIPHY</a></p>

---

## But, after a few moments

<iframe src="https://giphy.com/embed/NENOgw8mgH0NW" width="480" height="470" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p style="font-size:0.5em"><a href="https://giphy.com/gifs/captain-america-NENOgw8mgH0NW">via GIPHY</a></p>

---

## So what do we need to know?

<div style="font-size:0.8em">

-   <!-- .element: class="fragment" -->
    While there are uncountable sets, any proof (whether written in English letters
    or formalized) is finite, and so there are only countably-many possible proofs.
-   <!-- .element: class="fragment" -->
    So perhaps this result, a consequence of Löwenheim-Skolem theorem, isn't too surprising:
    -   <!-- .element: class="" -->
        Given a countable set \\(S\\) in your universe of sets, there exists a
        countable set \\(M\\supseteq S\\) in your universe
        such that any statement* about things defined for \\(M\\)
        is true in your universe if and only if \\(M\\) witnesses its truth.
    -   <!-- .element: class="fragment" -->
        That is, \\(M\\) is a countable elementary submodel for your universe.
</div>

---

## Will's proof 1/5

<div style="font-size:0.9em">

-   <!-- .element: class="fragment" -->
    Fix a countable elementary submodel \\(M\\) of our universe that contains
    Bob's strategy \\(\sigma\\) and the rationals.
-   <!-- .element: class="fragment" -->
    Then consider
    \\[E_t = \\{x\\text{ legal}|a&lt;x\\Rightarrow\\sigma(t^\\frown\\langle{a}\\rangle)\\leq x\\}\\]
    enumerated over partial playthroughs \\(t\\) using reals from \\(M\cap\mathbb R\\) rather than
    just \\(\mathbb Q\\).
-   <!-- .element: class="fragment" -->
    Suppose \\(w\not\in \\bigcup_t E_t\\) (countable). We will describe how Alice ensures
    \\(w\\) remains legal throughout the game.

</div>

---

## Will's proof 2/5

-   <!-- .element: class="" -->
    Suppose Alice has successfully played the game up to a certain round,
    where the partial playthrough \\(t\\) only uses moves from \\(M\\), and \\(w\\)
    remains legal.
-   <!-- .element: class="fragment" -->
    Since
    \\[w\not\in E_t=\\{x\\text{ legal}|a&lt;x\\Rightarrow\\sigma(t^\\frown\\langle{a}\\rangle)\\leq x\\}\\]
    there exists \\(a'&lt;w\\) such that \\(\\sigma(t^\\frown\\langle{a'}\\rangle)&gt; w\\).
-   <!-- .element: class="fragment" -->
    Note \\(a'\\) is legal, but not necessarily in \\(M\\)...

---

## Will's proof 3/5

<div style="font-size:0.75em">

-   <!-- .element: class="" -->
    Let \\(\\alpha,\\beta\\in M\\) be the last moves of Alice and Bob, respectfully.
    We now have the following reals
    \\[\\alpha &lt;a'&lt;w&lt;\\sigma(t^\\frown\\langle{a'\\rangle})&lt;\\beta\\]
    where \\(a',w,\\sigma(t^\\frown\\langle{a'\\rangle})\\) may not belong to \\(M\\).
-   <!-- .element: class="fragment" -->
    Choose \\(r,s\\in \\mathbb Q\\subseteq M\\) with 
    \\[\\alpha &lt;a'&lt;r&lt;w&lt;s&lt;\\sigma(t^\\frown\\langle{a'\\rangle})&lt;\\beta\\]
-   <!-- .element: class="fragment" -->
    Consider the set
    \\[A=\\{a\\in(\\alpha,r)| \\sigma(t^\\frown\\langle{a\\rangle})\\in(s,\\beta)\\}\\]
    such that \\(a'\\in A\\).

</div>

---

## Will's proof 4/5

<div style="font-size:1em">

-   <!-- .element: class="" -->
    Then 
    \\[A=\\{a\\in(\\alpha,r)| \\sigma(t^\\frown\\langle{a\\rangle})\\in(s,\\beta)\\}\\]
    is a set \\(M\\) understands, since \\(A\\) is defined in terms of 
    \\(\\alpha,r,\\sigma,t,s,\\beta\\in M\\).
-   <!-- .element: class="fragment" -->
    Observe that
    \\(A\\not=\\emptyset\\)
    is true in our universe since \\(a'\\in A\\).
-   <!-- .element: class="fragment" -->
    Thus \\(M\\) witnesses \\(A\\not=\\emptyset\\), which means there exists
    \\(a\\in M\\) such that \\(a\\in A\\).

</div>

---

## Will's proof 5/5

<div style="font-size:0.9em">

-   <!-- .element: class="" -->
    Finally, from \\(a\\in A\\cap M\\) we have
    \\[\\alpha &lt;a&lt;r&lt;w&lt;s&lt;\\sigma(t^\\frown\\langle{a\\rangle})&lt;\\beta\\]
    where \\(a,\\sigma(t^\\frown\\langle{a\\rangle})\\in M\\), and \\(w\\) remains legal.
-   <!-- .element: class="fragment" -->
    This completes the induction: Alice is able to play reals known to our countable
    elementary submodel \\(M\\) such that \\(w\\) remains legal during the whole game.
-   <!-- .element: class="fragment" -->
    Thus Alice can defeat any strategy for Bob when \\(W\\) is uncountable.

</div>

---

## How can you do this kind of thing without submodels?

<div style="font-size:0.9em">

-   <!-- .element: class="fragment" -->
    We'll need this result from STDC 2021:
    Bob has a winning strategy
    if and only if he has a winning *coding* strategy:
    defined only in terms of the most recent move of
    each player.
    -   <!-- .element: class="fragment" -->
        ("Coding" comes from the fact that Bob can create
        such strategies from perfect-info strats by
        *encoding* all of Alice's previous moves into his
        own moves.)
-   <!-- .element: class="fragment" -->
    So now we need only show that Alice can defeat any
    coding strategy for Bob given an uncountable \\(W\\).

</div>

---

## Steven's Proof 1/2

<div style="font-size:0.9em">

-   <!-- .element: class="fragment" -->
    Let \\(\\sigma\\) be a coding strategy for Bob that only uses rationals.
-   <!-- .element: class="fragment" -->
    For each \\(q,\\beta\\in\\mathbb Q\\), define
    \\[E_{q,\\beta} = \\{x\\text{ legal}|a\\in(q,\\beta)\\Rightarrow\\sigma(\\beta,a)\\leq x\\}\\]
-   <!-- .element: class="fragment" -->
    \\(E_{q,\\beta}\\) cannot contain bounded decreasing subsequences, as \\(a=\\inf\\)
    creates a contradiction.
-   <!-- .element: class="fragment" -->
    Suppose \\(w\not\in \\bigcup_{q,\\beta} E_{q,\\beta}\\) (countable). We will describe how Alice ensures
    \\(w\\) remains legal throughout the game, defeating \\(\\sigma\\).

</div>

---

## Steven's Proof 2/2

<div style="font-size:0.9em">

-   <!-- .element: class="" -->
    Suppose Alice has successfully played the game up to a certain round,
    where \\(\\alpha,\\beta\\) were played most recently, and \\(w\\) remains legal,
    that is, \\(\\alpha&lt;w&lt;\\beta\\).
-   <!-- .element: class="fragment" -->
    Pick \\(q\\in\\mathbb Q\\) with \\(\\alpha&lt;q&lt;w&lt;\\beta\\).
-   <!-- .element: class="fragment" -->
    Since
    \\[w\\not\\in E_{q,\\beta} = \\{x\\text{ legal}|a\\in(q,x)\\Rightarrow\\sigma(\\beta,a)\\leq x\\}\\]
    there exists \\(a\\in(q,w)\\) such that \\(\\sigma(\\beta,a)&gt; w\\).
-   <!-- .element: class="fragment" -->
    Note \\(a\\) is legal, and results in \\(a&lt;w&lt;\\sigma(\\beta,a)\\),
    completing the induction.
    
</div>

---

## Thoughts and Observations

<div style="font-size:0.9em">

-   <!-- .element: class="fragment" -->
    My proof was shorter, but only because I factored out the complexity
    to the lemma "coding \\(\Leftrightarrow\\) perfect-info".
-   <!-- .element: class="fragment" -->
    The complexity was needed to exchange \\(a'\\) with \\(a\\)
    from a nice countable set in this inequality:
    \\[\\alpha &lt;a'&lt;w&lt;\\sigma(t^\\frown\\langle{a'\\rangle})&lt;\\beta\\]
    Perhaps this could have similarly been factored out to a lemma?
-   <!-- .element: class="fragment" -->
    Limited-info strategies can be used to clean up
    recursive arguments similar to using submodels.

</div>

---

## Your thoughts and observations

---

# THANK YOU!

Slides at [clontz.org](https://clontz.org)
