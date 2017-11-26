**Adventures in Recreational Mathematics: Volume II**

Salutations!

Welcome to the second instalment of AiRM, this time taking a look at **cellular automata**. 

We have some exciting articles lined up for the future, potentially including but not limited to Chaos Theory, Trans-finite Set Theory, Game Theory and more - so, watch this space!

To understand what a cellular automaton is, I think it is helpful to understand the motivation behind the concept’s creation in the 1940s, leading up to a book which essentially founded the field: *The Theory of Self-Reproducing Automata* by **John von Neumann**.

In this case, it is also necessary to have a word on John von Neumann, since he was an exceptional man and potentially merits the term genius in all the ways he contributed to mathematics. In fact, his remarkable intelligence was noticeable from a young age, when at just 6 years old, he was able to proficiently converse in Ancient Greek and became quickly famous in his school for being able to multiply and divide 8-digit numbers in his head in under 10 seconds. 



By the 1940s, von Neumann had become interested in self-replication. He wanted to comprehend on an abstract level how a dynamic system or mechanistic object like life on earth could go about creating copies of itself in an efficient way and one that could allow for variation (a property referred to as *evolvability*) – he came to the conclusion that it ultimately relied upon:

* The propagation of information in systems.

* The culmination of well-defined local rules into complex global behaviour.

* The information structure (or "tape" as he called it) being an active part of the construction process.

Consider that these observations were made prior to the discovery of the structure of DNA. von Neumann had, in a heuristic sense, understood what it had to look like.

To define a cellular automaton, consider an $n$-dimensional space (a plane, say) divided into discrete unit-squares, where each square is a *cell* which can be in one of a defined number of states. Then, we wish to propagate each cell to a new state with the use of a *ruleset*, where we look at a *neighbourhood* of defined nearby or local cells for a given cell and based on their states, we assign that cell its next state. The ruleset itself is an ordered list of sets-of-length 2 containing every possible configuration of the neighbourhood and a state assigned to that.

This sounds quite abstract, so to illustrate, we can take a look at one of the elementary automata, discovered in the 1980s by Stephen Wolfram.

![](image_0.gif)





![](image_1.png)





However, we must return to John von Neumann and his design for a self-replicating machine: while Rule 110 is only 1 dimensional with 2 states, von Neumann’s original automaton had a grand 29 states, was 2 dimensional & used a neighbourhood which looked at a cell and its four adjacent cells. As you can imagine, the ruleset would be massive and is too long to explain here (it required its own book, you see) but we can give an outline. There was the null or ground State 0 as per usual, a group of 8 *transmission* states which could act as wires to transmit binary signals,  a group of 4 *confluent* states which could act as junctions for these wires to give information to & finally 16 *transition* states which could be built by confluent cells given the right signals from transmission cells.



![](image_3.png)



* A State-1 (alive) cell with fewer than 2 State-1 cells in its neighbourhood becomes State-0 (dies).

* A State-1 cell with 2 or 3 State-1 cells in its neighbourhood stays at State-1.

* A State-1 cell with more than 3 State-1 *neighbours* becomes State-0.

* A State-0 cell with exactly 3 State-1 neighbours becomes State-1.

With just these four rules come the surprising results that the automaton is firstly also capable of universal construction, despite being so much simpler than von Neumann’s automaton, that it is capable of universal computation, like Rule 110 (or just a normal computer) and finally that for a given starting set of states, the problem of determining whether the system will eventually evolve to a "static" situation (where no further changes happen to the states of any cell in future iterations of the system) is *generally undecidable*, i.e. there is no algorithm that solve this problem for all situations. As Conway said himself “My life game wasn’t designed. I just sort of thought that if you couldn’t predict what it did, then probably that was because it was capable of doing anything.”



![](image_4.png)

 













* Finite-state Machines (part of understanding the more formal definition of C.A.)

* Von Neumann Universal Constructor

* Wireworld (another, extremely intuitive C.A. in which some individuals have made a fully programmable computer!)

* Langton’s Loops, Langton’s Ant & Turmites in general

* A New Kind of Science by Stephen Wolfram

* Garden of Eden Theorem

* Rule 30

**_Challenge II_**:

1. Calculate the lambda value for the Game of Life.

2. Design your own spaceship in your own cellular automaton. There are quite literally an uncountably infinite number of ways of answering this one, so we’ll be excited to see your answers.

Finally, we have some exciting news! Due to the fact that AiRM may be taking up permanent residence in The Librarian, there will soon be an *AiRM Challenge* page on **The Librarian’s website (www.librarian.cf/)** which will list all previous challenges and will have buttons to reveal student answers! So now, if (or, rather, when) you decide to attempt any of the challenges, you can go to the website to read them and if you are successful in cracking any of them, your answer will be up there permanently!


