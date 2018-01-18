WeightSystem est un système qui nous permet de récuperer la masse d'un objet beacoup plus imposant que le load cell utilisé.

Voilà à quoi il ressemble (load cell):
![loadcell](https://www.robotshop.com/media/catalog/product/cache/1/image/900x900/9df78eab33525d08d6e5fb8d27136e95/m/i/micro-load-cell-20-kg.png)

Vissé sur cette cellule de pesage, on place une plaque de plexiglas qui va servir de support.

Le WeightSystem fonctionne de la manière suivante:

1. le WeightSystem, connecté à l'Arduino, prend en compte la masse du sac à vide, et "tare" pour fixer le point de mesure 0.
2. Au fur et à mesure que l'on remplit le sac, on peut mesurer sa masse.

![fig1](weightsystem.png)
