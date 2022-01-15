# Structures algébriques

Notes de cours par `Thomas Peugnet`.

## Un anneau

Un anneau est définit par : $(A, +, *)$.

Triplé composé :

-   D’un ensemble $A$ qui contient deux éléments spéciaux 0 et 1.
    -   0 -> Élément neutre pour **l’addition**
    -   1 -> Élément neutre pour la **multiplication**
-   De deux opérations.
    -   $(A\times A)$ –> $A$
    -   le $+$ et le $*$ sont appelés par **addition** et **multiplication**



Qui satisfont :

### Pour l’addition :

-   Associativité : $a + (b + c) = (a+b)+c)$
-   $\exists$ neutre : $a+0=0+a=a$
-   Inversibilité : $\forall a \in A, \exists (-a) \in A$
    -   $a+(-a)=(-a)+a=0$
-   Commutativité : $a+b=b+a$



### Pour la multiplication : 

-   Associativité : $a *(b*c)=(a*b)*c$
-   $\exists$ neutre : $a*0=0*a=a$



### Pour la distributivité :

*À droite et à gauche.*

-   $a*(b+c)=a*b+a*c$
-   $(a+b)*c = a*c+b*c$



### Exemples

-   $M_5 (\R)$ : matrices carrées

    –> C’est un anneau non commutatif, car $A*B \neq B*A$.

-   $(\R,+,\times)$ est un anneau

    –> $\R [X], +,\times]$

-   $(\Z, +, \times)$ est un anneau

-   $(\N, +, \times)$ n’est pas un anneau

–> N’a pas d’inverse.



**Un anneau est intègre si toute relation du type $ab=0$ implique $a=0$ ou $b=0$**.



>   #### Exemple 1
>
>   $\Z /n \Z = \{0, 1, …, ,n-1\}$ avec tous les élément avec une **barre** au-dessus.
>
>   $x$ : classe d’équivalence pour la relation modulo $n$.
>
>   $x = \{y \in \Z, y\equiv x[n]\}$
>
>   -   $a \equiv 2[5]$ et $b\equiv 1[5]$
>       -   $a+b \equiv 2+1 [5]$

>   #### Exemple 2
>
>   –> $\Z / 6\Z$
>
>   $6 = 2 \times 3$
>
>   2(Barre) non nulle ($\equiv 2[6]$)
>
>   3(Barre) non nulle ($\equiv 3[6]$)
>
>   $2B * 3B = (2*3)B = 0B$
>
>   -   Avec $(2*3)B :\equiv 6[6]( = 0)$
>   -   Donc, non intègre.
>
>   On a donc $aB*bB = 0B$ alors que $aB \neq 0B$ et $bB \neq 0B$.



On dit qu’un élément $a$ d’un anneau $A$ est inversible si $\exists b\in A$ tel que : $ab = 1 = ba$.

L’ensemble des éléments inversibles de $A$ est noté $A^X$ : 

-   $Z ^X = \{-1;1\}$
-   $\R^X = R^{\times}$
-   $\C^X$ = …
-   $\R [x]^X = \{$polynômes constants $\neq$  0$\}$
-   $\Z[X]^X = \{$2 polynômes : $-1$ et $1\}$



>   *Soit $A$ un anneau **intègre**, un élément $p \in A|A^\times$* est irréductible si toute écriture de la forme $p=ab$ implique: 
>
>   -   $a$ inversible
>
>   **OU EXCLUSIF**
>
>   -   $b$ inversible



## Un sous anneau

C’est un sous-ensemble d’un anneau.

Un sous anneau d’un ensemble $A$ est un ensemble $B \subset A$ qui contient les éléments neutres de $A$ et pour lequel le produit et la somme d’éléments de $B$ est toujours dans $B$.



L’inverse d’un nombre est un nombre avec lequel on multiplie le premier nombre pour avoir 1. $(\frac{42}{42})$

Un **sous-anneau** est un **anneau**.



>   Anneau $A$
>
>   $A^X = $ éléments inversibles de $A$.
>
>   $A^X=\cup (A)=$ groupe des unités de $A$.
>
>   $U(\Z)=\Z^X = \{-1,1\}$
>
>   $U(\R)=\R^*$

>    $A$ –> un anneau intègre
>
>   $p \in A|A^X$ 
>
>   -   => $p$ n’est pas inversible.
>   -   => $p$ est irréductible.
>
>   *Si toute écriture de la forme $p=ab$ => $a$ est inversible ou $b$ est inversible.*

>   #### Exemples
>
>   -   8 irréductible dans $\Z$ ? Non, car on peut écrire $8=4\times 2$, etc.
>
>   -   5 irréductible dans $\Z$ ? Oui, car on peut **seulement** écrire $5=5\times 1$ ou $5 = -5 \times -1$.
>
>   -   $\Z[\sqrt(3)]=\{a+b\sqrt{3}| a,b \in \Z\}$
>
>   -   $\Q[\sqrt(2)]=\{a+b\sqrt{2}| a,b \in \Q\}$
>
>   
>
>   $F_p = \{\Z |p\Z\}$ où $p$ premier.
>
>   -   $F_2[X]$ 
>       -   => $2X^2 + 3X + 1$
>       -   => $X + 1$
>
>   *On fait un modulo 2, car $F_2$, sur tous les coefficients du polynôme.*
>
>   
>
>   Quels sont les éléments irréductibles de $\Z[i]$ ?
>
>   -   $i=i \times 1$ est non irréductible.

Un anneau $A$ est un **corps** si tout élément non nul est inversible.

>   -   $\Z n \Z $ est il inversible ? Oui, pour tout $p$ premier.



## Stathme

On appelle **Stathme** sur $(A, +, *)$ toute application $V: A^* $–> $\N$ qui satisfait  les deux propriétés :

-   $\forall a,b \in A^* \space V(a) \leq V(ab)$ 
-   $\forall a \in A, \forall b \in A^* \space \exists a,r \in A$  tels que 
    -   $a=bq + r$ avec $r=0$ ou $V(r) < V(b)$.



>   #### Exemples
>
>   Stathme sur $\Z$ ?
>
>   -   $V(a) = |a|$ 
>   -   $\Z^*$ –> $\N$.
>
>   $|a| \leq |ab|$ sur $\Z$, pour $\forall a \in \Z , \forall b \in \Z^*$ :
>
>   -   $a = bq + r$ 
>       -   –> $r=0$
>       -   –> $|r| < |b|$
>
>
>   Stathme sur $\R[X]$ ?
>
>   -   $V(P)=deg(P)$
>   -   $deg(P) \leq deg(PQ) \space \forall P,Q…$
>   -   $P = qQ+r$
>       -   $r = 0$
>       -   $deg(1)<deg(0)$



## Un anneau euclidien

Un anneau est euclidien s’il intègre **ET** s’il admet un Stathme.



>   #### Exemple
>
>   $\Z, \R[X]$



## Un anneau factoriel

Un anneau est factoriel s’il intègre **ET** si tout élément non nul s’écrit comme produit de facteurs irréductibles.

*Un anneau euclidien est nécessairement factoriel, mais un anneau factoriel n’est pas euclidien.*



>   #### Exemple
>
>   Sur $\R[X]|(X^2+X+1)$ le reste d’un polynôme de $\R[X]$ par $(X^2 + X + 1)$ :



## Espaces vectoriels

>   *Un espace vectoriel sur un corps $K$* ($K$-espace vectoriel) est un triplet $(V,+,*)$ où :
>
>   -   $V$ est un ensemble
>   -   $+$ est une opération internet $V^x$ –> $V$
>   -   $*$ est une opération externe $K \times V$ –> $V$
>
>   Tel que :
>
>   #### Addition
>
>   1.   Dans $V$ :
>
>   $$
>   u + (v+w) = (u+v) + w = u + v+ w
>   $$
>
>   2.   Élément neutre :
>        $$
>        V + 0 = 0 + V = V
>        $$
>
>   3.   Inverse :
>
>   $$
>   \forall v \in V, \exists w \in V \\
>   v + w = w + v = 0
>   $$
>
>   #### Multiplication
>
>   



>   5.   $$
>        \forall \lambda, \mu \in K, \Delta u \in V\\
>        \lambda(\mu, u) = (\lambda \mu)u
>        $$
>
>   
>
>   6.   Élément neutre :
>
>   $$
>   1.u = u
>   $$
>
>   #### Addition et Multiplication
>
>   7.
>   $$
>   (\lambda + \mu)u = \lambda u + \mu u
>   $$
>   8.
>   $$
>   \lambda (u+v) = \lambda u + \lambda v
>   $$

## A RÉ-ÉCRIRE ( Au dessus)





