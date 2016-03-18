# dismathportfolio-chen-christine
dismathportfolio-chen-christine created by Classroom for GitHub

## Week 1
###### January 11, 2016

- This week, we were introduced to a new subject called **Discrete Mathematics** (DISMATH).
- We are here to examine problems logically and carry out precise mathematical reasoning by utilizing formal logic and set notation.
- I've learned that DISMATH deals ONLY with *mathematical truth*.
- I learned that a **proposition** is a declarative statement which can be either *true* (1) or *false* (0).
- A **proposition** cannot be both true and false.
- I also learned how to use **logical connectives** as the table shown below:

| **Logical Symbol**  |  **Logical Operator** | **Shorthand** | **Formula** | **Logical Expression** |
| :-----: |:-------:|:-----:| :-------: | :-------: |
| ¬ |Negation | not | val(¬p) = 1 - val(p) | ¬p |
| ∧ | Conjunction | and | val(p ∧ q) = min(val(p), val(q)) | p ∧ q |
| v | Disjunction | or | val(p v q) = max(val(p), val(q)) | p v q |
| ⊕ | Exclusive disjunction | xor | if val(p)  not equal val(q) = 1 , otherwise  0|  p ⊕ q  ≡ (¬p ∧ q) v (p ∧ ¬q) |
| → | Conditional | if, then | if val(p)  ≤ val(q) = 1 , otherwise  0  | p → q ≡  ¬p v q |
| ↔ | Biconditional | iff | if val(p) equals val(q) = 1 , otherwise  0 |  p ↔ q ≡ (p → q) ∧ (q → p) |

- I learned how to verify a statement by using a **Truth Table**.
- A **truth table** is a list of all possible combination of inputs with corresponding outputs.
  - The number of rows for the truth table is 2<sup>n</sup>; n is the number of variables.


###### January 13, 2016

- From Monday's lesson, I've learned the different propositional logic such as:
  - Inverse of p → q: ¬p → ¬q
  - Converse of p → q: q → p
  - Contrapositive of p → q: ¬q → ¬p (which also happens to be the equivalent value of the original statement)
- Same as Algebra, Discrete Mathematics has its own set of laws and rules too.
- These laws and rules are call the **logical equivalences** as the table shown below:

|         Name        |                           Equivalence                          |
|:-------------------:|:--------------------------------------------------------------:|
|    Identity laws    |                      p ∧ T ≡ p<br>p v F ≡ p               |
|   Domination laws   |                       p v T ≡ T<br>p ∧ F ≡ F               |
|    Negation laws    |                     p v ¬p ≡ T<br>p ∧ ¬p ≡ F                   |
| Double negation law |                            ¬(¬p) ≡ p                           |
|   Idempotent laws   |                       p v p ≡ p<br>p ∧ p ≡ p               |
|   Commutative laws  |                   p v q ≡ q v p<br>p ∧ q ≡ q ∧ p               |
|   Associative laws  |       (p v q) v r ≡ p v (q v r)<br>(p ∧ q) ∧ r ≡ p ∧ (q ∧ r)   |
|  Distributive laws  | p v (q ∧ r) ≡ (p v q) ∧ (p v r)<br>p ∧(q v r) ≡ (p ∧ q) v (p ∧ r) |
|   De Morgan's laws  |              ¬(p ∧ q) ≡ ¬p v ¬q<br>¬(p v q) ≡ ¬p ∧ ¬q          |
|   Absorption laws   |                 p v (p ∧ q) ≡ p<br>p ∧ (p v q) ≡ p             |

- Using **logical equivalences** and **proof by truth table**, it has been proven that *p → q ≡ ¬p ∨ q*.
- By using the same techique in our homework, we were able to prove that superman does not exist.


## Week 2
###### January 18, 2016

- In this week's lesson, we were introduced to a new lesson: **Predicate Logic**
- **Predicate logic** concerned its internal structure in terms of *subject* and *predicate*.
- While **propositional logic** deals with proposition *as a whole*.
- **Quantifiers** indicate the generality of the open sentence in which a variable occurs.
  - **Universal Quantifier (∀x)** - "For all", it asserts that a predicate is true for *all values* of a variable in a particular domain.
  - **Existential Quantifier (∃x)** - "Then exist", it is true if and only if P(x) is true for *at least one value* of x in the domain.
- Lastly, I've learned the terminologies for **Rules of Inference**:
  - *Argument* - a sequence of statements that end with a conclusion.
    - Ex. (p1 ∧ p2 ∧ p3 ... ∧ pn) → q 
  - *Valid* - The conclusion of he argument must follow from the true of the preceding statements of the argument.
    - Ex. (p1 ∧ p2 ∧ p3 ... ∧ pn) → q  is *TAUTOLOGY*
    - *Tautology*- A statement is ALWAYS true
  - *Fallacy* - Invalid argument.


## Week 3
###### January 25, 2016

- From all the previous lesson, I learned that there are **tools** that can be used to prove statements and these are:
  - Truth Table (for less variables)
  - Logical equivalences
  - Quantifiers
  - Rules of Inference
- Since verifying the validity of an argument through a truth table is a tedious process.
- We can use **rules of inference** as an alternative, the table is shown below:

|   **Rule of Inference**  |            **Tautology**           |          **Name**          |
|:--------------------|:------------------------------:|:----------------------:|
|       p<br>p→q<br>∴ q      |        (p ∧ (p → q)) → q       |      Modus Ponens      |
|     ¬q<br>p→q<br>∴ ¬p     |       (¬q ∧ (p → q)) → ¬p      |      Modus Tollens     |
|     p→q<br>q→r<br>∴ p→r    |  ((p → q) ∧ (q → r)) → (p → r) | Hypothetical Syllogism |
|      p∨q<br>¬p<br>∴ q      |       ((p ∨ q) ∧ ¬p) → q       |  Disjunctive Syllogism |
|       p<br>∴p ∨ q       |           p → (p ∨ q)          |        Addition        |
|       p ∧ q<br>∴ p       |           (p ∧ q) → p          |      Simplication      |
|      p<br>q<br>∴ p ∧ q     |      ((p) ∧ (q)) → (p ∧ q)     |       Conjunction      |
| p ∨ q<br>¬p ∨ r<br>∴ q ∨ r | ((p ∨ q) ∧ (¬p ∨ r)) → (q ∨ r) |       Resolution       |

###### January 27, 2016

- From last Monday's lesson, we had some drills and exercises about the **rules if inference**.
- I've learned how to use the **rules of inference** in *premises*.
- I also learned how to use the **rules of inference** to build *arguments*.
- I learned the difference between *if and only if*, *if, then*, and *only if*.
  - NOTE: A *if* and *only if* B (A ↔ B)
    - A *if* B - A is the antecedent and B is the consequent. Therefore, *if* B *then* A (B → A).
    - A *only if* B - From (A ↔ B), we knew the *if, then* statement is (B → A). Therefore, (A ← B).
    - ((B → A) ∧ (A ← B)) → (A ↔ B)
- We were introduced to **methods of proofs**.
- **Direct proof** (p → q)
  - Steps:
    1. Assume *p* is true.
    2. Show that *q* is also true (based on 1).
  - Ex. "If n is an integer, then n<sup>2</sup> is odd."
    - Odd number: {2k+1 | k ∈ Z}
    - Even number: {2K | k ∈ Z}


## Week 4
###### February 1, 2016

- We continued our discussion in **methods of proofs**.
- **Proof by Contraposition**/Indirect (¬q → ¬p)
  - Steps:
    1. Assume *¬q* is true.
    2. Show that *¬p* is also true.
      - This is usually used when *p* is more complicated than *q*.
  - Ex 1. "If n is an integer and 3n+2 is odd, then n is odd."
  - Ex 2. "If n=ab, where a and b are positive intergers, then a≤√n or b≤√n."
- **Vacuous Proof** (¬p → (p → q))
  - Show that *p* is *false*, because *(p → q)* must be *true* when *p* is false.
  - Ex. "If 6 is a prime number, then 6<sup>2</sup>=30."
    - It is a **vacuous proof** because the first and second statement are both *false*.
- **Trivial Proof** (q → (p → q))
  - Show that *q* is *true*, it follows that *(p → q)* must also be *true*.
  - Ex. "If there are 30 students enrolled in this course this semester, then 6<sup>2</sup>=36."
    - It is a **trivial proof** because the first statement is *vague*, while the second statment is clearly *true*.
- **Proof by Contradiction**
  - Steps:
    1. Assume the WHOLE premise is false *¬(premise)*≡T.
    2. Show that (1) will end up in a *contradiction*.

###### February 3, 2016

- We had two examples in **proof by contradiction**.
  - Ex 1. Prove that √2 is irrational by giving a proof by contradiction.
    - Rational number: {a/b | a, b ∈ Z, b≠0, *a, b does not have common factor except ±1}
  - Ex 2. "If 3n+2 is odd, then n is odd."
- From example #2 of proof by contradiction it leads us to **negation of implication**.
- **Negation of Implication** (¬(p → q) → (p ∧ ¬q))
- **Contradiction and Implication**
  - “If *p* s true, then *q* is true” using a **proof by contradiction**:
    1. Assume that *p≡T* and that *q≡F*.
    2. Derive a contradiction.
    3. Conclude that if *p* is *true*, *q* must be *as well*.
- **Proof by Equivalence (Biconditionals)**
  - To prove a theorem that is a biconditional statement *(p ↔ q)*, we show that: *(p → q) → [(p → q) ∧ (q → p)]*
  - Ex 1. "If n is an integer, n is even iff n<sup>2</sup> is even." (r ↔ s)
    - For biconditional statement, we should prove (r → s) and (s → r) are both *true*.


## Week 5
###### February 10, 2016

- We continued our discussion in **methods of proofs**, and had more examples in **proof by equivalence**.
- **Proof by Equivalence (Biconditionals)**
  - Ex 2. "If n is a positive integer, then n is odd if and only if n<sup>2</sup> is odd."
  - Ex 3. For any natural number n, n is even if and only if n<sup>2</sup> is even.
  - Ex 4. Show that these statements about the integer _n_ are equivalent:
    - P1: n is even
    - P2: n-1 is odd
    - P2: n<sup>2</sup> is even
  - Ex 5. Prove or disprove the following theorem: 
    - Every positive integer is the sum os the squares of two integers.
      - The statement is *false* due to *counterexample*.
        - *Counterexample* - It is an example that disproves a universal ("for all") statement.
- **Mathematical Induction**
  - Treats the sequence of propositions as a domino:
    - P(1), P(2), P(3), P(k), P(k+1), ...
  - Steps:
    1. Basic step: Show *P(1)≡T*
    2. Inductive step: 
      - Assume *P(k)* is true.
      - Show that is also *P(k+1)* true.
  - *Q.E.D. (quod erat demonstrandum)* - "which is what had to be proven" or signals the completion of the proof.
  - Ex. Prove P(n) = 1 + 2 + 3 + … + n = n(n+1)/2

## Week 6
###### February 15, 2016
- **Summation**
  - The notation for sum of _a<sub>m</sub>, a<sub>m+1</sub>, ..., a<sub>n</sub>_ is _∑<sup>a</sup><sub>i=m </sub>a<sub>i</sub>_ where _i_ is the index of summation.
    - Example: ∑<sup>a</sup><sub>i=m </sub> = 1 + 2 + 3 + ... + n
    - We also proved the theorem: The sum of the first n powers of two is 2<sup>n</sup>-1.
- **Recursive/Inductive Definition**
  - Basic step: f(0)
  - Inductive step: Give a rule for finding its value.
  - Ex 1. Find f(1), f(2), f(3), f(4) of the following recursive function.
  - Ex 2. Give an induction definition of the factorial function f(n)=n!
  - Ex 3. Give a recursive definition of ∑<sup>n</sup><sub>k=0</sub> a<sub>k</sub>
  - Ex 4. Give a recursive definition of a<sup>n</sup>, where a is a non-zero ℝ and n is a nonnegative integer (N)
- **Recursive Algorithm**
  - It solves a problem by reducing it to an instance of the same problem with smaller input.
    - Recall: <u>Algorithm</u> - finite set of precise instructions for performing a computation/solving a problem.
  - Ex 1. What is the recursive algorithm n!?
  - Ex 2. Give a recursive algorithm for computing a<sup>n</sup>, where a is a nonzero real number and n is a nonnegative integer.

###### February 17, 2016
- **Program Correctness**
- We need a proof to show that the program always gives the correct output.
    - PROGRAM VERIFICATION
      - Proof of correctness of programs
      - Uses the rules of inference and various proof techniques including mathematical induction
      - It is said to be correct if it produces the correct output for every possible input:
         1. Show that the correct answer is obtained if the program terminates (Partial Correctness)
         2. Show that the program always terminates
    - PARTIAL CORRECTNESS
      - Two propositions are used to specify what it means for a program to produce the correct output:
         1. Initial Assertion - _p_ - gives the properties that the input values must have
         2. Final Assertion - _q_ - gives the properties that the output of the program should have, if the program did what it was told
- **Hoare Triple**
    - p{s}q
    - A program, _S_, is said to be partially correct with respect to the initial assertion _p_ and the final assertion _q_ if whenever _p_ is true for the input values of _S_ and _S_ terminates, then _q_ is true for the output values of _S_.
    - Example: Given the initial assertion _p: x=1_ and the final assertion _q: z=3_, show the partial correctness of the program segment: </br> y = 2 </br> z = x + y

- **Rules of Inference**
    - CONDITIONAL STATEMENTS </br>
        (p ∧ _condition_) {S} q </br>
        (p ∧ _¬condition_) → q </br>
        ∴ p {**if** _condition_ **then** _S_} q
        - Example: Verify that the following program segment is correct with respect to the initial assertion _T_ and the final assertion _y ≥ x_. </br>
            **if** _x>y_ **then** </br>
            _y=x_
    - IF-ELSE STATEMENT </br>
        (p ∧ _condition_) {S<sub>1</sub>} q </br>
        (p ∧ _¬condition_) {S<sub>2</sub>} q </br>
        ∴ p {*if* _condition_ *then* _S<sub>1</sub>_ *else* _S<sub>2</sub>_} q
        - Example: **if** _x<0_ **then** </br> _abs= -x_ </br> **else** </br> _abs = x_

- **Power Series**
    - ∑<sup>∞</sup><sub>n = 0</sub> a<sub>n</sub>x<sup>n</sup> </br>
        where _a<sub>0</sub>, a<sub>1</sub>, a<sub>2</sub>, ..._ is a given sequence of constants, and _x_ is a real variable.
    - Examples:
        - 1 + r + r<sup>2</sup> + r<sup>3</sup> + ... = 1/(1-r)
        - Represent as power series: 1/(1+x)
        - Find the corresponding function: 1 - x<sup>2</sup> + x<sup>4</sup> - x<sup>6</sup> + ... 


## Week 7
###### February 24, 2016
- **Introduction to Set Theory**
  - Set - *unordered* collection of *distinct* objects.
    - {a, b, c, d, e}
      <br> ↳ Set notation: curly braces with commas seperating out elements.
  - Empty Set { } = ∅ means no elements
    - {∅} not an empty set
  - Set Builder Notation {x | some property that x satisfies}
  - Membership
    - a ∈ {a, b, c, d}
- **Venn Diagram**
- **Set Identities**
|  **Law**  |  **Identity**  |
| :------: | :-----------------------------: |
|  Identity Laws  |  A ⋂ U ≡ A  <br>  A ⋃ ∅ ≡ A  |
|  Domination Laws  |  A ⋃ U ≡ U  <br>  A ⋂ ∅ ≡ ∅  |
|  Idempotent Laws  |  A ⋃ A ≡ A  <br>  A ⋂ A ≡ A  |
|  Complementation Law  |  (A¯)‾ ≡ A  |
|  Commutative Laws  |  A ⋃ B ≡ B ⋃ A  <br>  A ⋂ B ≡ B ⋂ A  |
|  Associative Laws  |  A ⋃ (B ⋃ C) ≡ (A ⋃ B) ⋃ C  <br>  A ⋂ (B ⋂ C) ≡ (A ⋂ B) ⋂ C  |
|  Distributive Laws  |  A ⋃ (B ⋂ C) ≡ (A ⋃ B) ⋂ (A ⋃ C) <br>  A ⋂ (B ⋃ C) ≡ (A ⋂ B) ⋃ (A ⋂ C)  |
|  De Morgan's Laws  |  (A ⋂ B)‾ ≡ A‾ ⋃ B‾  <br>  (A ⋃ B)‾ ≡ A‾ ⋂ B‾  |
|  Absorption Laws  |  A ⋃ (A ⋂ B) ≡ A  <br>  A ⋂ (A ⋃ B) ≡ A  |
|  Complement Laws  |  A ⋃ A‾ ≡ U  <br>  A ⋂ A‾ ≡ ∅  |
- **Subsets ⊆**
  - A set S is a subset of a set T (denotes S ⊆ T) if all elements of S are also elements of T
  - Example:  ℕ ⊆ ℤ (every natural number is an integer)
- **Power Set P(S)** = {T|T ⊆ S} - A set of all subsets.
- **Cardinality |S|** 
  - The number of element it contains
  - Infinite Cardinalities - alaph-null (0,1,2,3,...)

## Week 8
###### February 29, 2016
- **Function**
  - Let A and B be sets. A function of *f* from A to B is an assignment of *exactly one* element of B to each element of A.
  - *Function* - mapping or transformation
    - f: A to B
      <br> ↳ A: domain
      <br> ↳ B: co-domain
        - *Range* - actually occuring values
- **Types of Function**
  - *One-to-One (Injective)* - Functions that never assign the same value to two different domain elements.
  - *Onto (Surjective)* - Functions have equal range & co-domain.
  - *One-to-One Correspondense (Bijection)* - Function is both one - to - one and onto.

###### March 2, 2016
- **Algorithms**
  - A finite set of precise instructions for performing a computation or for solving a problem.
      - *Properties of Algorithms*
        - Input - has input values from a specified set 
        - Output - solution to the problem 
        - Definitness - defined precisely 
        - Correctness - produce the correct output values 
        - Finiteness - produce the desired output 
        - Effectiveness - perform exactly and in a finite amount of time 
        - Generality - applicable for all problems of the desired form
- **Pseudocode**
    - high - level desciption of an algorithm that uses the structural conventions of a programming language 
    - intended for human reading
    - Preconditions - describe valid input
    - Postconditions - conditions that the output should satisfy
    - Format:
  
              PROCEDURE max(a1, a2, ... an: Z)
               max = a1
               for i = 2 to n
                 if max < aj then max = aj
              {Output: max is the largest element}

## Week 9
###### March 7, 2016
- **Searching Algorithms** - Problem of locating an algorithm in an ordered list
  - *Linear Search* - Finding a particular value in a list that checks each element in sequence until the desired element is found

              Require: {a1, a2, ..., ai, ..., an} ≠ ∈ Z; x ∈ Z
              Ensure: result = k, where (ak = x) and k ∈ {1, ..., n} if the element is found; otherwise k = -1
                result ← -1
                for i = 1 to n do
                  if result == ai then
                     result ← i
                  end if
                end for

  - *Binary Search* - Comparing the middle values of a list then repeated until the desired output is found.

              Require: {a1, a2, ..., ai, ..., an} ≠ ∈ Z, where a1 < a2 < ... < an; x ∈ Z
              Ensure: result = k, where (ak = x) and k ∈ {1, ..., n} if the element is found; otherwise k = -1
                i ← -1
                j ← n
                while i < j do
                  mid ← ⌊(i + j)/2⌋
                  if x > amid then
                    i ← mid +1
                  else
                    j ← mid
                  end if
                end while
                if x == ai then
                  result ← i
                else
                  result ← -1
                end if

- **Sorting Algorithms** - Problem of assorting elements into increasing order
  - *Bubble Sort* - Compares the first two elements then interchanging them if they are in the incorrect order.

              Require: {a1, a2, ..., ai, ..., an} ∈ R; n ≥ 2
              Ensure: {a1, a2, ..., an} where a1 < a2 < ... < an
                for i = 1 to n-1 do
                  for j = 1 to n-i do
                    if aj > aj+1 then
                      temp ← aj+1
                      aj+1 ← aj
                      aj ← temp
                    end if
                  end for
                end for

  - *Insert Sort* - Compares the second element with the first and inserts it before the first element if it is less. 

              Require: {a1, a2, ..., ai, ..., an} ∈ R; n ≥ 2
              Ensure: {a1, a2, ..., an} where a1 < a2 < ... < an
                for j = 2 to n do
                  i ← 1
                  while aj > ai do
                    i ← i + 1
                  end while
                  temp ← aj
                  for k = 0 to j-i-1 do
                    aj-k = aj-k-1
                  end for
                  ai = temp
                end for

###### March 9, 2016
- **Greedy Algorithm** - Algorithms that make what seems to be the "best" choice at each step. Selects the best choice at each step, instead of considering all sequences of steps that may lead to optimal solution
  - *Greedy Change* - Making algorithm

              Require: {c1, c2, ..., ci, ..., cn} ∈ Coin Domination
                      where c1 > c2 > ... > cn; x - amount of money in cents
              Ensure: result[n] = minimum number of coins per domination
                for i = 1 to n do
                  resulti ← 0
                  while x ≥ ci do
                    x ← x - ci
                    resulti  ← resulti + 1
                  end while
                end for

- Also started on the **Growth of Functions** often described using Big-O Notation.

## Week 10
###### March 14, 2016
- We resume the discussion on the Growth of Functions.
- **Big-O Notation**
    - Let _f_ and _g_ be functions from R-R; _f(x)_ is _O(g(x))_ if there are constants _C_ and _k_ such that: </br>
        |f(x)| ≤ C|g(x)| </br>
    whenever _x > k_.

- **Big-Omega and Big-Theta Notation**
    - Big-O Notation does not provide a lowerbound for the size of f(x). </br>
        - **Big-Omega** (Big-Ω) - lower bound </br>
        - **Big-Theta** (Big-Θ) - both upper and lower bound
