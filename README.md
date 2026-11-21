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

## Activité 3 — Théorème de Pythagore
- On connaît les angles du triangle ABC. Entrée : `Â ; B̂ ; Ĉ = [   ]`
- Conditions : « Le triangle ABC est rectangle en A », « Le triangle ABC est rectangle en B », « Le triangle ABC est rectangle en C »
- Fin : « BC² = AB² + AC² », « AC² = AB² + BC² », « AB² = AC² + BC² », « On ne peut pas conclure avec le théorème de Pythagore »

## Activité 4 — Réciproque et contraposée du théorème de Pythagore
- On connaît les longueurs des côtés du triangle ABC (figures cotées).
- Conditions : « BC² = AB² + AC² », « AC² = AB² + BC² », « AB² = AC² + BC² »
- Fin : « ABC est rectangle en A / en B / en C », « ABC n'est pas rectangle »

## Activité 5 — Multiple de 7 (division euclidienne)
- Entrée : `n = [   ]` (n ne change jamais)
- Actions (nouveaux blocs) : « i prend la valeur n », « i prend la valeur i − 7 » — permettent de faire une **boucle**
- Conditions : « i ≥ 7 », « i = 0 »
- Fin : « n est un multiple de 7 », « n n'est pas un multiple de 7 »
- Pendant la vérification, la valeur de i s'affiche à côté de n ; à la fin, le jeu affiche la division euclidienne (ex. 30 = 7 × 4 + 2).

## Comment jouer
- Glisser un bloc de la palette dans la zone (ou le toucher).
- Toucher un point jaune ● (sortie d'un bloc, « Oui » / « Non »), puis toucher le bloc d'arrivée pour tracer une flèche.
- Toucher une flèche pour l'effacer, × pour supprimer un bloc.
- Glisser un nombre dans la case `n = [   ]` (ou le toucher), puis cliquer sur « Lancer la vérification ».
- « Tester tous les nombres » : la machine est validée si elle répond juste pour tous.

## Ajouter une activité
Dans `index.html`, copier un objet du tableau `ACTIVITES` (en haut du script) et changer les conditions, les sorties, la fonction `attendu` et la liste `nombres`.
