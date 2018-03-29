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
<li> Si possible, un système qui permettrait de changer le sac (moteurs?). Il faudrait changer le sac si la poubelle est remplie ou si le poids dépasse un certain seuil (à fixer, il ne faut pas que la poubelle soit trop lourde ou trop difficile à déplacer).</li>
</ol>

<em>Séance 3 (Victor seul) :</em>

Nous avons trouvé un moyen de peser le sac: le WeightSystem. Avec un support placé en dessous du sac poubelle, on peut, à l'aide d'un load cell et de ressorts, mesurer la masse du sac (cf dossier WeightSystem pour plus de détails).

<em>Séance 3 (bis):</em>

Petits changements sur le WeightSystem, il suffit de placer une plaque de plexiglas sur le load cell (avec des vis), donc on supprime les ressorts. J'ai aussi changé le schéma dans le readme du WeightSystem.

<em> Séance 4 :</em>

Présentation orale et acquisition du UCABoard, ainsi que de l'Arduino Mini Pro et du module LoRa. Nous avons commencé à regarder des exemples de code. 

<em> Séance 5 :</em>

Objectif: Faire marcher le WeightSystem.

Résultat: Succès. A des intervalles de 1000ms, on observe des mesures de masse relativement correctes. Des mesures précises et éventuels recalibrages seront effectués avec des masses de valeurs différentes (1kg, 500g...). 

<em> Séance 6 :</em>

Problème des Tx/Rx réglé (cf cahier de suivi de projet de Sacha, paragraphe "Séance 5"): Soudures rééffectuées.
Inscription sur Internet Of Things. Tentative de synchronisation de la board avec le routeur aux Templiers: échec. 

Objectif: synchroniser la board, puis tester le WeightSystem et le FullBinDetector avec la board.

<em> Séances 7/8 :</em>

Inscription sur mydevices.com pour visualiser les données envoyées et pour localiser la LoRa. WeightSystem opérationnel, reste à rajouter une alerte lorsque le poids de la poubelle est supérieur à un poids défini (LED pour l'instant, puis alerte grâce à Cayenne LPP). Nouvelle idée: pouvoir verrouiller la poubelle avec une serrure à électroaimant ou simplement avec bobine + aimant, et pouvoir désactiver ce système simplement avec un relais. 

Prochaine séance : présentations mi-parcours et simulation/estimations pour savoir si le système de verrouillage est viable (trop grosse consommation pour un système qui est censé être portable). Sinon, essayer de trouver un autre moyen pour verrouiller automatiquement à distance (et efficacement surtout).
