---
*Created: September 2026 | Status in September: Complete*

A tense temporal language $ℒ_{T_{p}}$ consists in:


1. A countably infinite set of atomic propositions letters p , q , r ...
2. Eight logical connectives: Five unary ¬ , F , P , G , H , three binaries ∨ , ∧ , → .
3. Punctuation ( , ).

Also, $ℒ_{T_{p}}$ = $ℒ_{P_{c}}$+ F , P , G , H , where $ℒ_{P_{c}}$ means a classical propositional logic.

The set of wffs of $ℒ_{T_{p}}$ is recursively defined:

a) Every atomic proposition is an $ℒ_{T_{p}}$ -wff.

b) If $\phi$ and $\psi$ are $ℒ_{T_{p}}$ -wff , then so are ($\phi \land \psi$) , ($\phi \lor \psi$) , and ($\phi \to \psi$) .

c) If $\phi$ is an $ℒ_{T_{p}}$ -wff, then so are $\lnot \phi$, $F\phi$ , $P\phi$ , $G\phi$ , $H\phi$ .


Intuitively, we will read the new operators as follows:

$F\phi$ "It will sometime be the case that $\phi$ "

$P\phi$ "It was sometime the case that $\phi$ "

$G\phi$ "It will always be the case that $\phi$ "

$H\phi$ "It was always the case that $\phi$ "


We can understand F and P as tense analogous of $\lozenge$ , and G , H , of $\Box$ , i.e. , tense operators are a type of modal operator. More precisely, tense logic is a multi-modal system. The semantics of tense operators, like their modal counterparts, follow a semantics defined via Kripke frame.

Definition (Kripke model). A Kripke model is a pair 𝔐 = ⟨ 𝔉, V ⟩ where 

a) 𝔉 = $⟨ W, V ⟩$ is a Kripke frame, and

b) $V$ is a function from the atomic propositions and the possible worlds to the truth values T and F, (i.e. , P being a set of atomic propositions, V: P × W → {T , F } ).


The truth conditions of these tense operators are defined as follows:

Let 𝔐 be a Kripke model as defined previously. Then: 

𝔐 , $w$ , $\models$ $P\phi$ iff there is $w'$ such that $w'Rw$ and 𝔐, $w'$ $\models$ $\phi$

𝔐 , $w$ , $\models$ $F\phi$ iff there is $w'$ such that $wRw'$ and 𝔐, $w'$ $\models$ $\phi$
 
𝔐 , $w$ , $\models$ $H\phi$ iff for all $w'$ such that $w'Rw$ and 𝔐, $w'$ $\models$ $\phi$ 

𝔐 , $w$ , $\models$ $G\phi$ iff for all $w'$ such that $wRw'$ and 𝔐, $w'$ $\models$ $\phi$

The point-based temporal models considered here are characterized by the following properties:

$\forall x \in W$  $\quad$  $\lnot xRx$ is the property of irreflexivity. 

$\forall x \forall y \in W$ $\quad$  xRy $\to$ $\lnot yRx$ is the property of asymmetry.

$\forall x \forall y \forall z \in W$ $\quad$ $xRy \land yRz \to xRz$ is the property of transitivity. 

$\forall x \exists y \in W$ $\quad$ $xRy$ is the property of no last point.

$\forall x \exists y \in W$ $\quad$ $yRx$ is the property of no first point.

$\forall x \forall y \exists z \in W$ $\quad$ $xRy \to xRz \land zRy$ is the property of density. 

$\forall x \forall y \forall z \in W$ $\quad$  $xRz \land yRz \to xRy \lor yRx \lor x = y$ is the property of backwards linearity. 

$\forall x \forall y \forall z \in W$ $\quad$ $zRx \land zRy \to xRy \lor yRx \lor x = y$ is the property of forwards linearity.

Some of these properties correspond to temporal formulas, such as transitivity, while others, such as irreflexivity, do not.

The propositional temporal logic $K_{t}$ has the following axioms and inference rules:
 
Ax. 1 $\phi$ , where $\phi$ is a tautology of classical propositional logic.

Ax. 2 $G(p \to q) \to (Gp \to Gq)$ . 

Ax. 3 $H(p \to q) \to (Hp \to Hq)$ .

Ax. 4 $p \to HFp$ 

Ax. 5 $p \to GPp$

Rule 1 (Modus Ponens). If $\vdash \phi$ and $\vdash \phi \to \psi$ then $\vdash \psi$

Rule 2 (Uniform Substitution). Replacing uniformly atoms $p_{1}$ , ... , $p_{n}$ by wffs $\phi_{1}$ , ... , $\phi_{n}$ in a theorem is also a theorem. 

Rule 3 (RG). If $\phi \vdash G \phi$ .

Rule 4 (RH). If $\phi \vdash H \phi$ .

Axioms 2 and 3 are temporal analogues of the K axiom, while RG and RH are rules temporal analogous of the Rule of Necessitation.
