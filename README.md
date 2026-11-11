# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:

### Project Title or Name of the Application	: PyChem: Learn to balance chemical equations.
### Section			   	      : 9 - Lithium
### Group Members			    : LIBARIOS, Yezhequille Alea C., NISPEROS, Ma. Andrea Charlize B., SALINAS, Sebastian Mathieu T.
### Date (Proposal Date)  : 

### Project Description:
This project creates an interactive chemistry study tool designed for high school Chemistry students as a review material to those that want to improve their knowledge on chemical reactions. By letting learners combine virtual elements into compounds and test equations, the software provides immediate visual feedback and verified chemical formulas as expected outputs.

System Components & Class Interactions:

Atom Class. Stores core elemental data including atomicNumber, symbol, and valenceElectrons. Its canBond() and getAvailableBonds() methods calculate how many covalent or ionic connections an element can still form.

Molecule Class. Aggregates multiple Atom objects into a bondedAtoms list and tracks connections via bondCount. It interacts directly with Atom methods inside addAtom() and isStable() to apply the octet rule and generate a string output via getFormula().

ReactionBalancer Class. Manages lists of reactants and products composed of Molecule instances. It uses checkConservation() to compare atom counts across both sides and balanceEquation() to output the final stoichiometric coefficients.

UML Diagram:

### Goals:

This project ultimately aims to help students understand the theory behind chemistry, allowing them to independently understand basic concepts of chemistry and therefore increase retention within STEM subjects. Students will become more confident when using chemical formulas and balancing equations due to the interactive nature of this study aid. This will give students a good understanding at the beginning of their studies, preparing them for higher science courses. The application can be used as a helpful teaching aid by teachers so that they can easily teach their students about chemistry.


Objective 1: Help students learn how to balance chemical equations

Objective 2: Reinforce chemistry concepts like covalent/ionic bonding and conservation of mass

Objective n: 
[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
