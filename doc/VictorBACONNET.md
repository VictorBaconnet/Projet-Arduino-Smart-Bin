<h1> Cahier de suivi du projet de Victor BACONNET </h1>

<em>Séance 1 (semaine 51) :<em> 
Binôme : Sacha CARNIERE

Nous étions partis sur l'idée d'un frigo intelligent, qui permettait de scanner tous les aliments et d'avoir une liste du contenu du frigo. En faisant nos recherches nous avons remarqué qu'il fallait des connaissances en Javascript, que nous n'avons pas, et il est trop compliqué d'apprendre le Javascript rapidement. Finalement, il a été décidé de changer de projet.
Avant la fin de la séance, une thématique avait été ciblée: l'écologie.

<em>Séance 2 :</em>

Pendant les vacances, nous avons décidé de réaliser une poubelle intelligente, qui pourrait donner comme informations:
<ol>
<li> Son poids, avec un module spécifique ou une puce prévue à cet effet. On pourrait utiliser une simple balance mais une contrainte principale est de pouvoir avoir toutes les informations nécessaires depuis un seul endroit. Donc si la poubelle est située à un autre endroit que l'utilisateur, on veut que ce dernier n'aie pas a se déplacer pour avoir accès au poids de la poubelle. Cela permet de prévoir aussi si le sac risque de casser, car parfois la poubelle n'est pas forcément remplie à ras bord et pourtant elle peut être très lourde.</li>
<li> Son taux de remplissage, probablement indiqué par des LED (vert -> rouge) </li>
<li> Lorsque la poubelle est remplie, elle envoie sa localisation (on imagine qu'il y a plusieurs poubelles réparties dans une ville entière), pour pouvoir la cibler directement. </li>
<li> Si possible, un système qui permettrait de changer le sac (moteurs?). Il faudrait changer le sac si la poubelle est remplie ou si le poids dépasse un certain seuil (à fixer, il ne faut pas que la poubelle soit trop lourde ou trop difficile à déplacer).</li><br>

<em>Séance 3 (Victor seul)</em>

Nous avons trouvé un moyen de peser le sac: le WeightSystem. Avec un support placé en dessous du sac poubelle, on peut, à l'aide d'un load cell et de ressorts, mesurer la masse du sac (cf dossier WeightSystem pour plus de détails).
