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
  - The number of rows for the truth table is 2^n; n is the number of variables.

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
  - **Universal Quantifier (∀x)** - "for all", it asserts that a predicate is true for *all values* of a variable in a particular domain.
  - **Existential Quantifier (∃x)** - "then exist", it is true if and only if P(x) is true for *at least one value* of x in the domain.
- Lastly, I've learned the terminologies for **Rules of Inference**:
  - *Argument* - a sequence of statements that end with a conclusion.
    - Ex. (p1 ∧ p2 ∧ p3 ... ∧ pn) → q 
  - *Valid* - the conclusion of he argument must follow from the true of the preceding statements of the argument.
    - Ex. (p1 ∧ p2 ∧ p3 ... ∧ pn) → q  is *TAUTOLOGY*
    - *Tautology*- a statement is ALWAYS true
  - *Fallacy* - invalid argument.


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
|:--------------------:|:------------------------------:|:----------------------:|
|       p<br>p→q<br>∴q      |        (p ∧ (p → q)) → q       |      Modus ponens      |
|     ¬q<br>p→q<br>∴ ¬p     |       (¬q ∧ (p → q)) → ¬p      |      Modus tollens     |
|     p→q<br>q→r<br>∴p→r    |  ((p → q) ∧ (q → r)) → (p → r) | Hypothetical syllogism |
|      p∨q<br>¬p<br>∴q      |       ((p ∨ q) ∧ ¬p) → q       |  Disjunctive syllogism |
|       p<br>∴p ∨ q       |           p → (p ∨ q)          |        Addition        |
|       p ∧ q<br>∴p       |           (p ∧ q) → p          |      Simplication      |
|      p<br>q<br>∴p ∧ q     |      ((p) ∧ (q)) → (p ∧ q)     |       Conjunction      |
| p ∨ q<br>¬p ∨ r<br>∴q ∨ r | ((p ∨ q) ∧ (¬p ∨ r)) → (q ∨ r) |       Resolution       |

