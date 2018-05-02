<h1> Cahier de suivi de projet de Sacha CARNIERE </h1>

<em>Séance 1 (semaine 51) :<em> 
Binôme : Victor BACONNET

Nous nous étions mis d'accord sur un inventaire de frigo automatisé, qui permettrait de connaître le contenu de son frigo, ainsi que la quantité associée à un aliment quelconque (ex: jambon x2). Malheureseument cette idée, après plus amples recherche ce projet s'est avéré trop difficile à réaliser.
Cependant nous voulions rester sur le thème de l'environnement.
Après des recherches pendant le cours nous n'avons toujours pas trouvé un sujet.

Pendant les vacances de Noël nous avons décidé d'un sujet qui nous paraissait cohérent et réalisable : une poubelle connecté qui peut donner des information sur son remplissage (Poids, quantité..) et les transmettre.

<em>Séance 2 (semaine 2) :<em>
Pendant cette séance j'ai recherché un moyen de mesurer la masse de la poubelle. J'ai pensé a un prototype du WeightSystem et j'ai commencé à faire un schema.

<em> Séance 3 :</em>

Pendant ce cours nous avous peaufiner le WeightSystem et commencé a préparer la présentation pour la séance suivante. J'ai aussi commencé à faire le système de detection de remplissage avec les LEDs et le capteur de distance.

<em> Séance 4 :</em>

Présentation orale et acquisition du UCABoard, ainsi que de l'Arduino Mini Pro et du module LoRa. Nous avons commencé à regarder des exemples de code. 

<em> Séance 5 :</em>

Pendant cette séance j'ai essayé de programmer l'Arduino Pro Mini avec le CP2102 sans succès, en effet il semble y avoir un problème avec les pins TX et RX de la carte.

<em> Séance 6-7 :</em>

Grace aux nouvelles soudures, les problèmes de communication entre la Arduino mini pro et l'ordinateur sont réglés.
J'ai réussi à obtenir des valeurs pour le capteur de distance branché sur l'UCA board mais quand la distance est trop grande un 0 apparait après chaque mesure de distance.
De plus, avec l'aide d'un encadrant, nous avons connecté notre board au "The Things Network".

<em> Séance 8 :</em>

Présentation des avancements aux encadrants.
Bizarrement je n'obtiens plus aucune valeur avec le capteur de distance branché à l'UCA board alors que ça marche très bien avec notre carte arduino classique. Selon les recherches internet cela serait lié au fait que le HC-SR04 ne fonctionne pas en 3.3 volts.

<em> Séance 8 :</em>

On a eu confirmation que les problèmes avec le capteur de distances sont biens liés au voltage trop faible de la carte. Pour résoudre ce problème nous allons opter pour une alimentation 5 volts qui va etre adapté en 3.3 volts pour la carte avec la pin "RAW" et que nous pourrons utiliser pour le HC-SR04. Il faudra aussi faire un pont de diviseur de tension pour récupérer les infos en 3.3 volts sur la carte.
J'ai aussi compris comment envoyer des données sur Cayenne mais il faut encore faire les tests.

<em> Séance 9 :</em>

J'ai réussi a envoyer les données obtenues par le load cell sur Cayenne, j'ai aussi commencé a prévoir l'envoi des donnés du capteur de distance et les coordonnées GPS. Calcul des valeurs des résistances pour le pont diviseur de tension pour le capteur de distance.

<em> Séance 10 :</em>

