[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/AtNXzL3S)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

### Proof 

Suppose I have a graph $G_1$ with 4 nodes $x_1, x_2, x_3, x_4$ all connected in a line. We'll have 3 edges I will call $E_{1,1}, E_{1,2}, E_{1,3}$ Where $E_{1,1}$ connects $x_1$ to $x_2$ and so on. Let's also create a graph $G_2$ with 3 nodes $y_1, y_2, y_3$ and therfore two edges $E_{2,1}, E_{2,2}$. So here is what they would look like.

$G_1$ = [$x_1$] - $E_{1,1}$ - [$x_2$] - $E_{1,2}$ - [$x_3$] - $E_{1,3}$ - [$x_4$]  ([] are nodes and pairs of - are edges)

$G_2$ = [$y_1$] - $E_{2,1}$ - [$y_2$] - $E_{2,2}$ - [$y_3$]

Then, we can make a bijection function $f$ that attempts to map every node in $G_1$ to $G_2$. 

$f = x_n \rightarrow y_n$ meaning any $x$ of one number maps to the $y$ with the same number.

If we try to map every node using the edges, we can map every node from $E_{k,1} to E_{k,2}$ but when we attempt to do the same with $E_{1,3}$ we have this. 

$(x_3,x_4) \in E_{1,3}$ iff $(f(x_3),f(x_4)) \in E_{2,3}$? 

This breaks our definition because $E_{2,3}$ doesn't exist and the other edges are already mapped, and $f(x_4) =$ undefined, there is no mapping in $f$ for our last node. 

So there doesn't exist a bijection function for these graphs because we can't map every node to another node. 

$\therefore$ two graphs that do not have the same number of nodes cannot be isomorphic, because there doesn't exist a bijection function that satisfies the definition. 

