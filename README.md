# Logimaths

Jeu de logique : l'élève construit une **machine de vérification** sous forme de logigramme, puis la teste avec des nombres.

## Activité 1 — Multiple de 5
- Entrée : `n = …`
- Conditions : « Le chiffre des unités de n est 0 », « Le chiffre des unités de n est 5 »
- Sorties : « n est un multiple de 5 », « n n'est pas un multiple de 5 »

Quand on choisit un nombre, le « … » est remplacé, les blocs traversés s'allument en **blanc**, et la sortie atteinte s'affiche en **vert** (bonne réponse) ou en **rouge** (mauvaise réponse).

## Comment jouer
- Glisser un bloc de la palette dans la zone (ou le toucher).
- Toucher un point jaune ● (sortie d'un bloc, « Oui » / « Non »), puis toucher le bloc d'arrivée pour tracer une flèche.
- Toucher une flèche pour l'effacer, × pour supprimer un bloc.
- « Tester tous les nombres » : la machine est validée si elle répond juste pour tous.

## Ajouter une activité
Dans `index.html`, copier un objet du tableau `ACTIVITES` (en haut du script) et changer les conditions, les sorties, la fonction `attendu` et la liste `nombres`.
