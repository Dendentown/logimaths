# Logimaths

Jeu de logique : l'élève construit une **machine de vérification** sous forme de logigramme, puis la teste avec des nombres.

## Activité 0 — Multiple de 10
- Entrée : `n = [   ]`
- Condition : « Le chiffre des unités de n est 0 »
- Sorties : « n est un multiple de 10 », « n n'est pas un multiple de 10 »

## Activité 1 — Multiple de 5
- Entrée : `n = [   ]` (case où l'on glisse un nombre)
- Conditions : « Le chiffre des unités de n est 0 », « Le chiffre des unités de n est 5 »
- Sorties : « n est un multiple de 5 », « n n'est pas un multiple de 5 »

On glisse un nombre dans la case vide de `n = [   ]`, puis on clique sur **Lancer la vérification** : les blocs traversés s'allument en **blanc**, et la sortie atteinte s'affiche en **vert** (bonne réponse) ou en **rouge** (mauvaise réponse).

## Activité 3 — Réciproque et contraposée du théorème de Pythagore
- ABC est un triangle dont le plus grand côté est [BC]. Entrée : `AB ; AC ; BC = [   ]` (on glisse un triangle).
- Condition : « BC² = AB² + AC² »
- Sorties : « ABC est rectangle en A », « ABC n'est pas rectangle en A »

## Comment jouer
- Glisser un bloc de la palette dans la zone (ou le toucher).
- Toucher un point jaune ● (sortie d'un bloc, « Oui » / « Non »), puis toucher le bloc d'arrivée pour tracer une flèche.
- Toucher une flèche pour l'effacer, × pour supprimer un bloc.
- Glisser un nombre dans la case `n = [   ]` (ou le toucher), puis cliquer sur « Lancer la vérification ».
- « Tester tous les nombres » : la machine est validée si elle répond juste pour tous.

## Ajouter une activité
Dans `index.html`, copier un objet du tableau `ACTIVITES` (en haut du script) et changer les conditions, les sorties, la fonction `attendu` et la liste `nombres`.
