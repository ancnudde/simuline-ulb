Simuline est un moteur permettant de créer et de jouer des jeux sérieux.

# Edition de jeu

## Fonctionnement global

Dans Simuline, il existe trois types de boîtes:

- les boîtes de question, qui contiennent acyuellement uniquement les boîtes de scènes, qui définissent la question à laquelle le joueur va devoir répondre.
- Les boîtes de réponses, qui définissent le type de réponse que le joueur pourra donner
- Les boîtes de supplément, qui s'attachent aux boites de question ou de réponse pour modifier la façon dont elles fonctionnent

## Scène

La scene correspond à l'écran de jeu principal, comprenant la question/ le dialogue du patient/ le contexte, ainsi que les images de fond, d'interlocuteur et les potentielles illustrations aditionnelles. Le texte correspond au texte affiché en haut à gauche lors du jeu

Une boite de scéne peut recevoir deux types de boîtes de suppléments:

- Des boîtes d'illustration, qui vont afficher soit
-   Background: Donne l'image de fond de la scène (officine, laboratoire, ...)
-   Interlocutor: Donne la personne présente en face du joueur (patient, professeur, ...)
-   Additional, qui s'affichera avant la scène, et permet d'afficher par exemple une ordonance, un spectre, une photo, ...

## Réponse

Les réponses sont les éléments qui vont permettre de définir les modalités de réponse proposées au joueur. Elles peuvent être de trois type:

- Fixe: Une réponse fixée à l'avance par l'éditeur du scénario, permettant de créer une question de type QCM
- Numérique: Une réponse sous forme de nombre, qui peut être un nombre exact ou une valeur comprise dans une fourchette donnée
- Textuelle: Une réponse sous forme de texte. Le texte peut être défini ou non comme sensible à la casse, et ne sera alors pas sensible aux différence de majuscules, de caractères spéciaux, d'espaces, ...
