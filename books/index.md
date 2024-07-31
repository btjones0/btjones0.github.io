# Books

<!-- Using Chicago Style Citations -->

These are some books that I've read and liked in various different mathematical/computer
science topics. I start with books that are applicable to some classes at Cal Poly and
then descend into deeper topics.

- [Introduction to Programming](#introduction-to-programming)
- [Introduction to Proofs](#introduction-to-proofs)
- [Programming Languages](#programming-languages)
- [Theory of Computation](#theory-of-computation)
- [Type Theory](#type-theory)
- [Lambda Calculus](#lambda-calculus)
- [Category Theory](#category-theory)
- [Mathematical Logic](#mathematical-logic)
- [Incompleteness/Undecidability](#incompletenessundecidability)
- [Set Theory](#set-theory)
- [Philosophy of Mathematics](#philosophy-of-mathematics)
- [History of Mathematics/Computer Science](#history-of-mathematicscomputer-science)

----------------------------------------------------------------------------------------

## Introduction to Programming

If you liked CSC 101/202 (or you're in it right now and you want some more books to
read), here are some books you might like. Most of these do not use the programming
language we use at Cal Poly for 101/202 (Python), so they're maybe not the best to
accompany a current student.

- Felleisen, Matthias, Robert Bruce Findler, Matthew Flatt, and Shriram Krishnamurthi.
  How to Design Programs: An Introduction to Programming and Computing. The MIT Press,
  2018.

  [Available as an online book](https://htdp.org/2024-11-6/Book/index.html), this is an
  introduction to programming using Racket (technically Racket-like languages designed
  for teaching).

- Sannella, Donald, Michael Fourman, Haoran Peng, and Philip Wadler. Introduction to
  Computation: Haskell, Logic and Automata. Springer, 2022.

  An introduction to programming using Haskell. It goes a bit deep into some theoretical
  topics (that we cover in 248, 430, 445, etc.) but assumes no prior knowledge in
  programming. It is used in a course for all first semester computer science students
  at the University of Edinburgh.

- Altenkirch, Thorsten, and Isaac Triguero. Conceptual Programming with Python.
  Lulu.com, 2019.

  An introduction to programming using Python. According to the book description, it's
  used in a course for Master's students with little or no background in programming
  coming from various different backgrounds.

----------------------------------------------------------------------------------------

## Introduction to Proofs

If you liked CSC 248 (or you're in it right now and you want some more books to read),
here are some books you might like.

- Cummings, Jay. Proofs: A long-Form Mathematics Textbook. Jay Cummings, 2021.

  This is an enormous book for learning mathematical proofs. It's largely intended for
  self study which means it has an extensive amount of detail.

----------------------------------------------------------------------------------------

## Programming Languages

If you liked CSC 430 (or perhaps haven't taken it yet, but you're excited for it), here
are some books you might like!

### Functional Programming

- Friedman, David P., and Matthias Felleisen. The Little Schemer. The MIT Press, 1996.

  An introduction to functional programming in Scheme. If you've taken CSC 430, most of
  this *should* be review. The last few chapters are possibly new (and there's a cool
  derivation of the Y combinator).

- Friedman, Daniel P., and Matthias Felleisen. The Seasoned Schemer. The MIT Press,
  1996.

  This is a companion to the above Little Schemer. It picks up where the Little Schemer
  left off and goes into other cool topics (e.g., continuations).

- Okasaki, Chris. Purely Functional Data Structures. Cambridge University Press, 1998.

  In CSC 202, you learn several data structures. Many of those probably involve
  mutations (e.g., every structure involving arrays). These structures don't work well
  if you want to do without mutation, but there are several data structures that can be
  implemented *purely* functionally.

### Implementing a Programming Language

- Siek, Jeremy. Essentials of Compilation: An Incremental Approach in Racket. The MIT
  Press, 2023.

  This is a book that *could* be used as a textbook for CSC 431. It's similar (at least
  at times) to CSC 430 material, except instead of parsing into an AST and then
  interpreting the AST into a value, we convert the AST into x86 assembly. The host (the
  language we're writing code in) is Racket and the target (the language for which we're
  writing a compiler) is a subset of Racket. Each chapter adds new features to the
  language.

- Siek, Jeremy. Essentials of Compilation: An Incremental Approach in Python. The MIT
  Press, 2023.

  This is the same idea as the above book *except* in Python. Because the target
  language is also Python, this means the book needs to talk about parsing (a topic we
  can mostly avoid when we implement a LISP-like language).

- Ball, Thorsten. Writing an Interpreter in Go. Thorsten Ball, 2016.

  Now if Go is more your preference, here's another book implementing an interpreter for
  a language hosted in Go. Because the target language (a new language created for the
  book called Monkey) isn't LISP-like syntax, we need to write a parser! Fully half the
  book is on lexing and parsing. This is a pretty good introduction to lexing/parsing
  and you write one entirely from scratch.

- Ball, Thorsten. Writing a Compiler in Go. Thorsten Ball, 2018.

  And a followup to the above book writing a compiler rather than an interpreter. I
  haven't finished reading this one yet, but it looks like you compile to byte code and
  then also write your own virtual machine.

----------------------------------------------------------------------------------------

## Theory of Computation

- Sipser, Michael. Introduction to the Theory of Computation. Cengage Learning, 2012.

----------------------------------------------------------------------------------------

## Type Theory

This is arguably still a part of the above [Programming
Languages](#programming-languages) section, but the books are (in my opinion) different
enough that I put them in their own section. They tend to be more theoretical
(definition/theorem/proof style).

- Friedman, Daniel P., and David Thrane Christiansen. The Little Typer. The MIT Press,
  2018.

  This is a fun introduction to dependent types in an incredibly small language called
  pie (the whole book is full of food puns). The book moves somewhat slowly but then
  some of the topics are quite strange at first.

- Pierce, Benjamin C. Types and Programming Languages. The MIT Press, 2002.

  This book is an introduction to type systems and to basic type theory. It's mostly
  grounded in implementation with theory when relevant.

- Stump, Aaron. Verified Functional Programming in Agda. Association for Computing
  Machinery and Morgan & Claypool, 2016.

  Agda is a dependently typed programming language/type theory playground. This book is
  aimed at writing algorithms and proving they're correct. And for some algorithms
  "internally" proving they're correct.

- Brady, Edwin. Type-Driven Development with Idris. Manning Publications Co, 2017.

  Idris is a dependently typed programming language intended as a general purpose
  language. This book given an introduction to the language along with details about
  dependent types.

- Nederpelt, Rob, and Herman Geuvers. Type Theory and Formal Proof: An Introduction.
  Cambridge University Press, 2014.

  This is dramatically more theoretical than the above books (and could arguably go in
  the next section on [Lambda Calculus](#lambda-calculus)). The first several chapters
  build up the syntax and semantics of dependant types. It then uses such a system to
  build definitions and mathematical proof.

- Hindley, J. Roger. Basic Simple Type Theory. Cambridge University Press, 2008.

  This is also very theoretical and could also arguable go in the Lambda Calculus
  section. It largely covers type assignment: given an expression determine all possible
  types that could be assigned to it.

----------------------------------------------------------------------------------------

## Lambda Calculus

Lambda calculus is part programming, part mathematical logic. It's arguably the first
programming language, predating computers by a few decades. In particular, it's the
backbone of functional programming languages.

- Michaelson, Greg. An Introduction to Functional Programming Through Lambda Calculus.
  Dover Publications, 2011.

  As the title would imply, this is an introduction to functional programming using
  lambda calculus. It builds several functional programming language features starting
  from a basis of just variables, function definitions, and function applications.

- Hindley, J. Roger, and Jonathan P. Seldin. Lambda-Calculus and Combinators, an
  Introduction. Cambridge University Press, 2010.

- Barendregt, Henk P. The Lambda Calculus, its Syntax and Semantics. College
  Publications, 2012.

  This is a rather dense, rather abstract book on lambda calculus. Not for the faint of
  heart.

----------------------------------------------------------------------------------------

## Category Theory

This starts to deviate quite a bit from practical computer science into very
mathematical topics. There is a large overlap/intertwining with certain parts of type
theory. A lot of category theory is quite abstract (sometimes called "abstract
nonsense") and heavily utilizes examples for intuition. A strong differentiator in
introductory books is what background is needed to understand the examples. Several of
the books I have in this section are specifically aimed at computer scientists.

### Introduction

- Lawvere, F. William, and Stephen H. Schanuel. Conceptual Mathematics: A first
  introduction to categories. Cambridge University Press, 2009.

  Possibly the gentlest introduction to category theory I've found. It assumes little
  prior mathematical knowledge.

- Walters, R. F. C. Categories and Computer Science. Cambridge University Press, 1992.

  This is another introduction to category theory, this one aimed at computer
  scientists. Many of the examples in the book are based around typed functions and
  computation.

- Milewski, Bartosz, and Igal Tabachnik. Category Theory for Programmers. Bartosz
  Milewski, 2019.

  This book started as a [series of blog
  posts](https://bartoszmilewski.com/2014/10/28/category-theory-for-programmers-the-preface/)
  that was typeset nicely into a book. There's also several [YouTube
  playlists](https://www.youtube.com/@DrBartosz/playlists) that you might enjoy. The
  examples use the Haskell programming language (but you don't need to know much to
  follow).

- Pierce, Benjamin C. Basic Category Theory for Computer Scientists. The MIT Press,
  1991.

  Another introduction to category theory aimed at computer scientists. Lots of type
  theory based examples.

- Goldblatt, Robert. Topoi: The Categorial Analysis of Logic. Dover Publications, 2006.

  The first few chapters of the book are a general introduction to category theory. This
  is not aimed at computer scientists and many of the examples in the book assume a
  broader pool of mathematical knowledge though you can get by skipping examples that
  you don't follow (not all of the examples are needed to build intuition). After the
  first few chapters, the book starts diving deep into the topic of topoi (plural of
  topos) hence the title of the book.

- Leinster, Tom. Basic Category Theory. Cambridge University Press, 2017.

  Another introduction to the subject aimed at mathematicians.

- Riehl, Emily. Category Theory in Context. Dover Publications, 2016.

  Another introduction to the subject aimed at mathematicians.

- Mac Lane, Saunders. Categories for the Working Mathematician. Springer, 1971.

  Saunders Mac Lane is the father of category theory. This is the original introduction
  to category theory. It is the classic reference.

  > All told, a monad in X is just a monoid in the category of endofunctors of X, with
  > product × replaced by composition of endofunctors and unit set by the identity
  > endofunctor. —Saunders Mac Lane

### Application

- Fong, Brendan, and David I. Spivak. An Invitation to Applied Category Theory: Seven
  Sketches in Compositionality. Cambridge University Press, 2019.

- Lawvere, F. William, and Robert Rosebrugh. Sets for Mathematics. Cambridge University
  Press, 2003.

  Mathematics is traditionally (by traditionally, I mean since the mid 1900s) been
  grounded in a theory of sets. But it doesn't have to be! This book describes how to
  axiomatically describe sets using category theory. It doesn't require much category
  theory background, but it doesn't hurt.

  It might be nice to read some [axiomatic set theory](#set-theory) first as a contrast.
  The Goldrei (Classic Set Theory) is my favorite.

- Lambek, J., and P. J. Scott. Introduction to higher order categorical logic. Cambridge
  University Press, 1988.

  Here we look at category theory as a logic foundation. This jumps right in and expects
  you to already be familiar with category theory.

- Mac Lane, Saunders, and Ieke Moerdijk. Sheaves in Geometry and Logic: A First
  Introduction to Topos Theory. Springer, 1992.

- Yanofsky, Noson S. Theoretical Computer Science for the Working Category Theorist.
  Cambridge University Press, 2022.

----------------------------------------------------------------------------------------

## Mathematical Logic

We don't really have a course at Cal Poly going into serious study of mathematical
logic. We have a brief introduction, but we don't see any deep results (e.g., soundness,
completeness, and compactness of first-order logic). We also don't really *need* any of
those result, but some of them (e.g., Gödel's incompleteness theorems) are relevant to
computer science. More on Gödel's incompleteness specifically in
[Incompleteness/Undecidability](#incompletenessundecidability).

- Chiswell, Ian, and Wilfrid Hodges. Mathematical Logic. Oxford University Press, 2007.
- Leary, Christopher C., and Lars Kristiansen. A Friendly Introduction to Mathematical
  Logic. Milne Library, SUNY Geneseo, 2015.
- Goldrei, Derek. Propositional and Predicate Calculus: A Model of Argument. Springer,
  2005.
- Plato, Jan von. Elements of Logical Reasoning. Cambridge University Press, 2013.
- Smullyan, Raymond M. First-Order Logic. Dover Publications, 1995.
- Bell, John L. Higher-Order Logic and Type Theory. Cambridge University Press, 2022.

----------------------------------------------------------------------------------------

## Incompleteness/Undecidability

Several books in this compilation relate to two major 1930's papers from Kurt Gödel and
Alan Turing. These are both *very* tough to read as they were aimed at experts in the
field.

- Kurt Gödel's "On formally undecidable propositions of Principia Mathematica and
  related systems I", and
- Alan Turing's "On Computable Numbers, with an Application to the Entscheidungsproblem"

The main results of incompleteness (Gödel) and undecidability (Turing) are then explored
in the following more recent books.

- Nagel, Ernest, and James R. Newman. Gödel’s Proof. New York University Press, 2001.

  This is an explanation of Gödel's incompleteness theorems proofs to make it more
  digestible than the original.

- Gödel, Kurt. On Formally Undecidable Propositions of Principia Mathematica and Related
  Systems. Dover Publications, 1992.

  This is a translation (the original was German) of Gödel's 1932 paper. I wouldn't
  necessarily read this, but it's very short and looks nice on a bookshelf.

- Petzold, Charles. The Annotated Turing: A Guided Tour Through Alan Turing’s Historic
  Paper on Computability and the Turing Machine. Wiley Publishing, 2008.

  Charles Petzold goes though the entirety of Turing's 1936 paper and explains it in
  order *very* thoroughly. The first couple chapters are mathematical and historical
  context.

- Heijenoort, Jean van. From Frege to Gödel: A Source Book in Mathematical Logic,
  1879–1931. Harvard University Press, 1967.

  This is a compilation of papers starting with Gottlob Frege's "Begriffsschrift" and
  leading up to (and including) Gödel's paper.

- Davis, Martin. The Undecidable: Basic Papers on Undecidable Propositions, Unsolvable
  Problems and Computable Functions. Dover Publications, 1965.

  This is a compilation of papers starting with Gödel (this is the third translation I
  own of this paper), goes through Alan Turing's thesis, and ending with Stephen Kleene
  and Emil Post.

----------------------------------------------------------------------------------------

## Set Theory

Set theory is the modern foundation for most of mathematics. Properly explaining a lot
of the nitty-gritty details is hard. Ernst Zermelo and later Abraham Fraenkel were two
people who worked on properly defining what is a set and what operations are allowed
when working with them.

- Goldrei, Derek. Classic Set Theory: For Guided Independent Study. Chapman & Hall,
  1996.

  This is a gentle introduction to axiomatic set theory.

----------------------------------------------------------------------------------------

## Philosophy of Mathematics

What is mathematics all about? Does it have a subject matter? What is this subject
matter? What are numbers, sets, points, lines, functions, and so on? What do
mathematical statements mean? What is the nature of mathematical truth? How is
mathematics known? What is its methodology? Is observation involved, or is it a purely
mental exercise? How are disputes among mathematicians adjudicated? What is a proof? Are
proofs absolutely certain, immune from rational doubt? What is the logic of mathematics?
Are there unknowable mathematical truths?

- Shapiro, Stewart. Thinking about mathematics: The philosophy of mathematics. Oxford
  University Press, 2000.

- Giaquinto, Marcus. The Search for Certainty: A Philosophical Account of Foundations of
  Mathematics. Oxford University Press, 2002.

- Lakatos, Imre. Proofs and Refutations. Cambridge University Press, 2015.

  This one is a bit of an oddball but shows a little of how the mathematical process
  works. Mathematical definitions are perhaps not as rigid as you'd think.

----------------------------------------------------------------------------------------

## History of Mathematics/Computer Science

Honestly there's a large overlap between books on the history of mathematics with books
on philosophy of mathematics. Several mathematicians through history have been motivated
by their philosophic outlook. These books are a bit less philosophical though.

- Swetz, Frank J. The Search for Certainty: A Journey Through the History of
  Mathematics, 1800–2000. Dover Publications, 2012.

- Doxiadis, Apostolos, and Christos H. Papadimitriou. Logicomix: An Epic Search for
  Truth. Bloomsbury, 2009.

  This is a graphic novel about foundations of mathematics. It largely follows Bertrand
  Russell in his quest to lay down the "axioms" of mathematics. It's (to my
  understanding) roughly historically accurate with some creative liberties to shorten
  the story at times.

- Mashaal, Maurice. Bourbaki: A Secret Society of Mathematicians. American Mathematical
  Society, 2006.

  There was (possibly still is) a secret society of French mathematicians that steered
  the direction of French mathematics (and to some extent global mathematics) for a few
  decades.

- Martin, Robert C. We, Programmers: A Chronicle of Coders from Ada to AI.
  Addison-Wesley, 2024.

- Petzold, Charles. Code: The Hidden Language of Computer Hardware and Software.
  Microsoft Press, 2022.

  I don't really know where to categorize this book. It's not quite history, but it's
  not quite not history. That said, I really like this book. It goes into detail about
  how a computer is built starting from very simple components and building up from
  there.

----------------------------------------------------------------------------------------

## Books I Plan to Read

In no particular order.

- Hofstadter, Douglas R. Gödel, Escher, Bach: an Eternal Golden Braid. Basic Books,
  1999.
- Aluffi, Paolo. Algebra: Notes from the Underground. Cambridge University Press, 2021.
- Moore, Gregory H. Zermelo’s Axiom of Choice: Its Origins, Development, & Influence.
  Dover Publications, 2013.
- Harper, Robert. Practical Foundations for Programming Languages. Cambridge University
  Press, 2016.
- Roberts, Siobhan. Genius at Play: The Curious Mind of John Horton Conway. Princeton
  University Press, 2024.
- Roberts, Siobhan. The Man Who Saved Geometry: The Multidimensional Mind of Donald
  Coxeter. Princeton University Press, 2024.
- Wilder, Raymond L. Introduction to the Foundations of Mathematics. Dover Publications,
  2012.
- Knuth, Donald E. Surreal Numbers. Addison-Wesley, 1974.
- Davis, Martin. Computability and Unsolvability. Dover Publications, 1985.
- Boolos, George S., John P. Burgess, and Richard C. Jeffrey. Computability and Logic.
  Cambridge University Press, 2007.
- Soare, Robert I. Turing Computability: Theory and Applications. Springer, 2018.
- Adams, Rod. An Early History of Recursive Functions and Computability: from Gödel to
  Turing. Decent Press, 2011.
- Aaronson, Scott. Quantum Computing Since Democritus. Cambridge University Press, 2013.
- Simmons, Harold. An Introduction to Category Theory. Cambridge University Press, 2011.
- Paulson, L. C. ML for the Working Programmer. Cambridge University Press, 1996.
- van Dalen, Dirk. Logic and Structure. Springer, 2012.
- van Dalen, Dirk. L.E.J. Brouwer - Topologist, Intuitionist, Philosopher: How
  Mathematics is Rooted in Life. Springer, 2013.
- Hinze, Ralf and Dan Marsden. Introducing String Diagrams: The Art of Category Theory.
  Cambridge University Press, 2023.
- Pavlovic, Dusko. Programs as Diagrams: From Categorical Computability to Computable
  Categories. Springer, 2024.
- Allison, Lloyd. A Practical Introduction to Denotational Semantics. Cambridge
  University Press, 1987.
- Bacon, Andrew. A Philosophical Introduction to Higher-order Logics. Routledge, 2023.
