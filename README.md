Simuline est un moteur permettant de créer et de jouer des jeux sérieux.

# Edition de jeu

## Fonctionnement global

Dans Simuline, il existe trois types de boîtes:

- les boîtes de question, qui contiennent acyuellement uniquement les boîtes de scènes, qui définissent la question à laquelle le joueur va devoir répondre.
- Les boîtes de réponses, qui définissent le type de réponse que le joueur pourra donner
- Les boîtes de supplément, qui s'attachent aux boites de question ou de réponse pour modifier la façon dont elles fonctionnent

Un jeu sur simuline se compose d'un ensemble de scènes. Dans une scène, une question ou un dialogue est présenté au joueur, qui aura la possibilité d'y répondre selon la modalité choisie par l'éditeur. En fonction de la réponse donnée et le chemin prévu par l'éditeur, le joueur passera à la scène suivante, rejouera la même scène ou sera renvoyé à une scène précédente.

Les connections entre une bôite de question et une boîte de réponse forment la scène. Les connections entre les boites de réponses et les boîtes de questions suivantes donnent la progression des scènes au cours du jeu en fonction des réponses de l'utilisateur.

Editeur           |  Jeu
:-------------------------:|:-------------------------:
<img width="400" alt="scene_ex" src="https://github.com/user-attachments/assets/140edef8-413f-43c0-a224-209d9d1bacc2" /> | <img width="600" alt="scene_vis" src="https://github.com/user-attachments/assets/9df2c350-0f21-4936-98ed-89d27c942e57" />




## Scène

La scene correspond à l'écran de jeu principal, comprenant la question/ le dialogue du patient/ le contexte, ainsi que les images de fond, d'interlocuteur et les potentielles illustrations aditionnelles. Le texte correspond au texte affiché en haut à gauche lors du jeu

<img width="450" alt="scene_num" src="https://github.com/user-attachments/assets/c368535d-aa28-4f82-8ec1-7a95a005be0e" />

1) Texte de la question
2) Ajouter un lien vers un site externe dans le texte
3) Rendre le texte sélectionné italique
4) Ajouter un retour à la ligne
5) Suprimer la boîte


Une boite de scéne peut recevoir deux types de boîtes de suppléments:

1) Des boîtes d'illustration, qui vont afficher soit
-   Background: Donne l'image de fond de la scène (officine, laboratoire, ...)
-   Interlocutor: Donne la personne présente en face du joueur (patient, professeur, ...)
-   Additional, qui s'affichera avant la scène, et permet d'afficher par exemple une ordonance, un spectre, une photo, ...

2) Une boîte de plugin, permettant d'ajouter un plugin au jeu. Pour le moment, le seul plugin accessible est le plugin *Computer*, qui permet d'afficher un ordinateur en bas de l'écran. Lorsque l'utilisateur clique sur écran d'ordinateur, il pourra accéder soit à un simulateur de microscope, soit à Pharmasoft, le simulateur de software officinal. L'option *Remove plugin* permet de retirer l'écran sur les scènes suivantes.

## Réponse

Les réponses sont les éléments qui vont permettre de définir les modalités de réponse proposées au joueur. Elles peuvent être de trois type:

- Fixe: Une réponse fixée à l'avance par l'éditeur du scénario, permettant de créer une question de type QCM
- Numérique: Une réponse sous forme de nombre, qui peut être un nombre exact ou une valeur comprise dans une fourchette donnée
- Textuelle: Une réponse sous forme de texte. Le texte peut être défini ou non comme sensible à la casse, et ne sera alors pas sensible aux différence de majuscules, de caractères spéciaux, d'espaces, ...
