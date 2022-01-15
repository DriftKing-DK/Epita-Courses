# Approximation de fonctions

# Introduction

Une suite $U_n$ converge vers $l$ si $\forall \epsilon > 0, \exists N \in \N, n >= N \rightarrow |U_n - l| < \epsilon$

-   $|U_n - l| < \epsilon$ => $U_n$ est à **au plus** $\epsilon$ de $f$.
-   $\forall \epsilon > 0, \exists N \in \N, n >= N$  => $f_n$ est à **distance** au plus $\epsilon$ de $f$.



## Question : Comment parler de distance entre deux éléments de $E$ ?

## Définitions

-   *Une distance est une fonction sur $E \times E$ à valeurs positives.*

-   *La distance entre un élément de $E$ et lui-même est nulle.*
-   *Étant donnés 2 éléments $x, y$ de E et un élément intermédiaire $z$, la somme des distances entre $x$ et $z$ puis $z$ et $y$ ne peut être plus petite que celle entre $x$ et $y$.*

>   Une **distance** sur un ensemble de $E$ est une application $d : E\times E \rightarrow \R_+$ qui satisfait :
>
>   -   Séparation : $\forall x,y \in E, d(x,y) = 0 \Leftrightarrow x = y$
>   -   Symétrie : $\forall x,y \in E, d(x,y) = d(y,x)$
>   -   Inégalité $\Delta$ : $\forall x,y,z \in E, d(x,y) \leq d(x,z) + d(z,y)$



>   On dit qu’une application $N:E \rightarrow \R_+$ est **une norme** sur $E$ si elle vérifie :
>
>   -   Définition : $\forall x \in E$, $N(x) = 0 \Leftrightarrow x = 0$
>   -   Homogénéité : $\forall x \in E, \forall \lambda \in K$, $N(\lambda x) = |\lambda|N(x)$
>   -   Inégalité $\Delta$ : $\forall (x,y) \in E²$, $N(x+y) \leq N(x) + N(y)$

