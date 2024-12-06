# draw_triangle

<img alt="Fonction" src="./draw_triangle.png" style="width: 75%;"/>


## Formules

Dans un triangles avec ses sommets aux coordonnées $(x_1, y_1)$, $(x_2, y_2)$ et $(x_3, y_3)$ :

Nous pouvons calculer les longueurs  $a$, $b$, $c$ de chaque coté du triangle avec ces calculs simples :
```math
\begin{align}
a = \sqrt{(x_2 - x_3) ^ 2 + (y_2 - y_3) ^ 2} \\
b = \sqrt{(x_3 - x_1) ^ 2 + (y_3 - y_1) ^ 2} \\
c = \sqrt{(x_1 - x_2) ^ 2 + (y_1 - y_2) ^ 2} \\
\end{align}
```

Puis son périmètre $p$ :
```math
p = a + b + c
```

Grâce à cela nous pouvons calculer l'air du triangle grâce à la formule d'Heron :
```math
s = \frac{p}{2}
A = \sqrt{ s \times (s - a) \times (s - b) \times (s - c)}
```

Ainsi que les coordonnées $I$ :
```math
I = \left(\frac{ax_1 + bx_2 + cx_3}{p}, \frac{ax_1 + bx_2 + cx_3}{p}\right)
```

Et le rayon $r$ du cercle inscrit
```math
\begin{align}
A = \frac{r \times p}{2} \\
r = 2 \times \frac{A}{p} \\
\end{align}
```


## Exemple

<img alt="Utilisation de la fonction" src="./draw_triangle_input.png" style="width: 75%;"/>
<img alt="Sortie de la fonction" src="./draw_triangle_output.png" style="width: 75%;"/>
