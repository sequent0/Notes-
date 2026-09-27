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

Definition (Kripke model). A Kripke model is pair 𝔐 = ⟨ 𝔉, V ⟩ where 

a) 𝔉 = ⟨ W, V ⟩ is a Kripke frame, and

b) V is a function from the atomic propositions and the possible worlds to the truth values T and F, (i.e. , P being a set of atomic propositions, V: P × W $\to$ {T , F}).


The truth conditions of these tense operators are defined as follows:

Let 𝔐 be a Kripke model as defined previously. Then: 

𝔐 , w , $\models$ $P\phi$ iff there is w' such that w'Rw and 𝔐, w' $\models$ $\phi$

𝔐 , w , $\models$ $F\phi$ iff there is w' such that wRw' and 𝔐, w' $\models$ $\phi$
 
𝔐 , w , $\models$ $H\phi$ iff for all w'such that w'Rw and 𝔐, w' $\models$ $\phi$ 

𝔐 , w , $\models$ $G\phi$ iff for all w' such that wRw'and 𝔐, w' $\models$ $\phi$

All of the Kripke models above are point-based. 







