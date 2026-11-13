# CS3SY26_ProjectProposal by Aline Teresa Mendoza from CS Unit of PSHS


## Project Proposal Template:

### Project Title or Name of the Application	: PyChem: Learn to balance chemical equations.
### Section			   	      : 9 - Lithium
### Group Members			    : LIBARIOS, Yezhequille Alea C., NISPEROS, Ma. Andrea Charlize B., SALINAS, Sebastian Mathieu T.
### Date (Proposal Date)  : November 13 2026

### Project Description:
This project develops an interactive chemistry study application designed specifically as a digital review tool for high school chemistry students. These introductory learners need accessible, hands-on practice to master foundational chemical reactions, prepare for assessments, and build confidence with core concepts. Currently, many students struggle to grasp abstract principles such as valence electrons, the octet rule, and the conservation of mass. This software allows students to virtually combine elements into compounds and test chemical equations. By delivering instant visual feedback alongside verified chemical formulas, the application helps learners identify and correct misconceptions immediately, making independent study both engaging and effective. 

System Components & Class Interactions:

Atom Class.(Parent) Stores core elemental data including atomicNumber, symbol, and valenceElectrons. Its canBond() and getAvailableBonds() methods calculate how many covalent or ionic connections an element can still form.

Metal Class (Subclass of Atom). Inherits from Atom and represents metallic elements that lose electrons when bonding. It overrides get_valenceElectrons() to return donatable outer electrons, and implements canBond() and getAvailableBonds() to calculate positive ionic bonding capacity.

NonMetal Class (Subclass of Atom). Inherits from Atom and represents non-metallic elements that gain or share electrons. It overrides get_valenceElectrons() to return outer electrons available for sharing or receiving, and implements canBond() and getAvailableBonds() based on how many electrons are needed to satisfy the octet or duet rule.

Metalloid Class (Subclass of Atom). Inherits from Atom and represents borderline elements with intermediate bonding behavior. It overrides get_valenceElectrons(), canBond(), and getAvailableBonds() to allow flexible covalent electron sharing up to a full valence shell.

NobleGas Class (Subclass of Atom). Inherits from Atom and represents inert Group 18 elements with full valence shells. It overrides get_valenceElectrons() to return a complete octet or duet, while implementing canBond() to always return False and getAvailableBonds() to return 0 to enforce chemical stability restrictions. 

Molecule Class. Aggregates multiple Atom objects into a bondedAtoms list and tracks connections via bondCount. It interacts directly with Atom methods inside addAtom() and isStable() to apply the octet rule and generate a string output via getFormula().

IonicBond Class / IonicMolecule (Subclass of bond). Inherits from Molecule and models compounds formed through electron transfer. It overrides addAtom() and isStable() to restrict bonding strictly to combinations of Metal and NonMetal instances whose net ionic charges balance to zero.

CovalentBond Class / CovalentMolecule (Subclass of bond). Inherits from Molecule and models compounds formed through electron sharing. It overrides addAtom() and isStable() to restrict bonding strictly to NonMetal and Metalloid instances where all shared electron pairs satisfy the octet or duet rule. 

ReactionBalancer Class. Manages lists of reactants and products composed of Molecule instances. It uses checkConservation() to compare atom counts across both sides and balanceEquation() to output the final stoichiometric coefficients.


UML Diagram:

<img width="512" height="512" alt="image" src="https://github.com/user-attachments/assets/9562d8ce-f3ba-4d5f-9f33-0158a2843e87" />


### Goals:

This project ultimately aims to help students understand the theory behind chemistry, allowing them to independently understand basic concepts of chemistry and therefore increase retention within STEM subjects. Students will become more confident when using chemical formulas and balancing equations due to the interactive nature of this study aid. This will give students a good understanding at the beginning of their studies, preparing them for higher science courses. The application can be used as a helpful teaching aid by teachers so that they can easily teach their students about chemistry.


Objective 1: Help students learn how to balance chemical equations

Objective 2: Reinforce chemistry concepts like covalent/ionic bonding and conservation of mass

Objective 3: Help students distinguish how metals, non-metals, metalloids, and noble gases behave differently when forming ionic and covalent bonds.

[Click here for Rubrics and Sample projects](https://docs.google.com/document/d/1xKd1CqK6DcNWS2_oJPBNtY5n3I3Hqiw8FY3W295Iqfk/edit?usp=sharing)
