# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:

### Project Title or Name of the Application	: PyChem: Learn to balance chemical equations.
### Section			   	      : 9 - Lithium
### Group Members			    : LIBARIOS, Yezhequille Alea C., NISPEROS, Ma. Andrea Charlize B., SALINAS, Sebastian Mathieu T.
### Date (Proposal Date)  : 

### Project Description:
This project creates an interactive chemistry study tool designed for high school and introductory college students who struggle with abstract chemical bonding and reaction balancing concepts. By letting learners combine virtual elements into compounds and test equations, the software provides immediate visual feedback and verified chemical formulas as expected outputs.

System Components & Class Interactions:

Atom Class. Stores core elemental data including atomicNumber, symbol, and valenceElectrons. Its canBond() and getAvailableBonds() methods calculate how many covalent or ionic connections an element can still form.

Molecule Class. Aggregates multiple Atom objects into a bondedAtoms list and tracks connections via bondCount. It interacts directly with Atom methods inside addAtom() and isStable() to apply the octet rule and generate a string output via getFormula().

ReactionBalancer Class. Manages lists of reactants and products composed of Molecule instances. It uses checkConservation() to compare atom counts across both sides and balanceEquation() to output the final stoichiometric coefficients.

**Sample class Diagram from https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png:**

![Sample Diagram](https://static.visual-paradigm.com/web/images/tutorials/class-diagram-tutorial/01-class-diagram-example.png)

### Goals:

This project ultimately aims to help students understand the theory behind chemistry, allowing them to independently understand basic concepts of chemistry and therefore increase retention within STEM subjects. Students will become more confident when using chemical formulae and balancing equations due to the interactive nature of this study aid. This will give students a good understanding at the beginning of their studies, preparing them for higher science courses. The application can be used as a helpful teaching aid by teachers so that they can easily teach their students about chemistry.


Objective 1: Build an Interactive Bonding Sandbox: Implement the Atom and Molecule classes to let users combine elements and receive immediate, rule-based feedback on duet and octet stability.

Objective 2: Develop a Real-Time Reaction Balancer: Create the Reaction module to visually track atom counts across reactants and products, reinforcing the Law of Conservation of Mass through instant validation.

Objective 3.: Design a Low-Stakes Learning Interface: Connect the core chemistry logic to an intuitive user interface via the StudyToolController, encouraging students to test hypotheses freely and learn from mistakes without penalty.


[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
