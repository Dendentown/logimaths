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

## Activité 3 — Multiple de 3
- Entrée : `n = [   ]` (n ne change jamais), avec la variable k affichée à côté
- Actions : « k prend la valeur n », « k prend la valeur de la somme de ses chiffres » (le calcul s'affiche à côté du bloc en clignotant)
- Conditions : « k ≥ 10 », « k = 3 », « k = 6 », « k = 9 »
- Fin : « n est un multiple de 3 », « n n'est pas un multiple de 3 »

## Activité 4 — Multiple de 7 (division euclidienne)
- Entrée : `n = [   ]` (n ne change jamais)
- Actions (nouveaux blocs) : « r prend la valeur n », « r prend la valeur r − 7 » — permettent de faire une **boucle**
- Conditions : « r ≥ 7 », « r = 0 »
- Fin : « n est un multiple de 7 », « n n'est pas un multiple de 7 »
- Pendant la vérification, la valeur de r s'affiche à côté de n ; à la fin, le jeu affiche la division euclidienne (ex. 30 = 7 × 4 + 2).

## Activité 5 — Réciproque et contraposée, avec les calculs
- Entrée : figure cotée du triangle ABC.
- Conditions : « AB / AC / BC est le plus grand côté », « BC² = AB² + AC² », « AC² = AB² + BC² », « AB² = AC² + BC² »
- Actions : « On calcule AB² », « On calcule AC² », « On calcule BC² », « On calcule AB² + AC² », « On calcule AB² + BC² », « On calcule AC² + BC² » — le détail du calcul s'affiche à côté du bloc, ligne par ligne en clignotant.
- Fin : « ABC est rectangle en A / en B / en C », « ABC n'est pas rectangle », « C'est absurde »
- Bonne fin mais égalité du plus grand côté non testée, ou calculs non faits avant ce test : la réponse n'est pas fausse, il manque une étape dans le raisonnement (orange).

## Activité 6 — Réciproque et contraposée du théorème de Pythagore
- On connaît les longueurs des côtés du triangle ABC (figures cotées).
- Conditions : « BC² = AB² + AC² », « AC² = AB² + BC² », « AB² = AC² + BC² »
- Fin : « ABC est rectangle en A / en B / en C », « ABC n'est pas rectangle »

## Activité 7 — Calculer une longueur avec le théorème de Pythagore
- Les côtés sont notés a, b, c ; on connaît b et c, a = ? (en bleu sur la figure). Entrée : `Le triangle : [   ]`
- Conditions : « Le triangle est rectangle », « a est l'hypoténuse », « c est l'hypoténuse », « b est l'hypoténuse »
- Si une égalité est oubliée (Pythagore ou a² = …), la réponse n'est pas fausse : il manque une étape dans le raisonnement, la figure et la Fin passent en orange.
- Actions : « c² + b² = a² », « a² + b² = c² », « a² = c² − b² », « a² + c² = b² », « a² = b² − c² »
- Fin : « a = √c² − b² », « a = √b² − c² », « a = √c² + b² » (barre de la racine sur tout le calcul), « On ne peut pas utiliser le théorème de Pythagore », « C'est absurde »
- En arrivant sur une Fin de calcul, le bloc affiche l'égalité avec les valeurs, puis le terme sous la racine calculé, puis la valeur de a.

## Activité 8 — Théorème de Pythagore
- On connaît les angles du triangle ABC. Entrée : `Â ; B̂ ; Ĉ = [   ]`
- Conditions : « Le triangle ABC est rectangle en A », « Le triangle ABC est rectangle en B », « Le triangle ABC est rectangle en C »
- Fin : « BC² = AB² + AC² », « AC² = AB² + BC² », « AB² = AC² + BC² », « On ne peut pas conclure avec le théorème de Pythagore »

## Activité 9 — Un nombre est-il solution ?
- Équation : 3x − 5 = 2x + 1. Entrée : `x = [   ]` (nombres négatifs et décimaux possibles)
- Actions : « On calcule 3x − 5 », « On calcule 2x + 1 » — le calcul s'affiche à côté du bloc, ligne par ligne
- Condition : « 3x − 5 = 2x + 1 » (les deux blocs de calcul clignotent quand on la teste)
- Fin : « x est solution de l'équation », « x n'est pas solution de l'équation »
- Bonne fin sans avoir calculé les deux membres avant la comparaison : il manque une étape (orange).

## Conditions avec les valeurs
Pour chaque condition qui est une égalité ou une inégalité (k ≥ 10, r = 0, BC² = AB² + AC², 3x − 5 = 2x + 1…), la même relation écrite avec les valeurs apparaît sous la condition en clignotant, puis le losange s'allume. Le symbole s'adapte : « 25 = 9 + 16 », « 60,84 ≠ 25 + 36 », « 4 < 10 ».

## Comment jouer
- Glisser un bloc de la palette dans la zone (ou le toucher).
- Toucher un point jaune ● (sortie d'un bloc, « Oui » / « Non »), puis toucher le bloc d'arrivée pour tracer une flèche.
- Toucher une flèche pour l'effacer, × pour supprimer un bloc.
- Glisser un nombre dans la case `n = [   ]` (ou le toucher), puis cliquer sur « Lancer la vérification ».
- « Tester tous les nombres » : la machine est validée si elle répond juste pour tous.

## Créer un modèle
Le bouton **＋ Créer un modèle** (à côté de « Tout tester ») ouvre une fenêtre pour fabriquer sa propre valeur de test :
- activités avec un nombre : on choisit n ;
- activité 3 : longueurs b et c, hypoténuse (a, b, c ou aucune) ;
- activité 4 : les trois angles, et les mesures à écrire sur la figure ;
- activités 5 et 6 : les longueurs AB, AC et BC.
La figure se dessine en direct, les valeurs impossibles sont refusées (somme des angles ≠ 180°, triangle qui n'existe pas…).
Les modèles s'ajoutent aux valeurs de test (bordure en pointillés), sont gardés dans le navigateur et se suppriment avec la croix.

## Ajouter une activité
Dans `index.html`, copier un objet du tableau `ACTIVITES` (en haut du script) et changer les conditions, les sorties, la fonction `attendu` et la liste `nombres`.
