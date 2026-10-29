# PedigreeFes

Éditeur d'arbres généalogiques médicaux, en français, selon la nomenclature NSGC (Bennett et al., 2022).

Fichier unique (`index.html`) sans dépendance : il s'ouvre hors ligne par double-clic ou se publie tel quel (GitHub Pages…). Rien n'est envoyé sur un serveur.

## Construire un arbre

- **Glisser-déposer** les symboles de la palette (homme, femme, sexe inconnu, grossesse, FCS, IMG) sur la feuille.
- **Clic droit** sur un symbole : ajouter les parents, un(e) conjoint(e), un enfant (fils, fille, jumeaux MZ/DZ, grossesse, FCS, IMG, mort-né), un frère ou une sœur ; statuts (atteint, porteur, présymptomatique, décédé, proposant, consultant), sexe, type, test génétique, adoption, infertilité ; relier à un conjoint ou à des parents existants ; supprimer (seul ou avec la descendance).
- **Clic droit sur un trait d'union** : enfants du couple, consanguinité, séparation, étiquette du lien (« cousins germains »).
- **Glisser** un symbole le déplace ; il s'aligne sur sa génération. `Maj` + glisser sur le fond : sélection rectangulaire.
- **Organiser** remet l'arbre en ordre (conjoints côte à côte, fratries centrées sous les parents) en gardant l'ordre gauche–droite.
- Panneau **Fiche** : nom, âge, année de naissance, décès, phénotypes avec précision (« K sein 42 a »), génotype, résultat E+/E−, notes.

## Consanguinité

- Le **double trait** s'ajoute automatiquement quand les deux conjoints ont un ancêtre commun dans l'arbre (forçable dans un sens ou dans l'autre).
- Onglet **Consanguinité** :
  - coefficient **F** d'un individu ou d'un enfant à naître, avec le détail des boucles de Wright (ancêtre commun, chemin, contribution) et leur surlignage sur l'arbre ;
  - coefficient de **parenté φ** entre deux individus, degré de parenté ;
  - **risque récessif** à partir de F et de la fréquence (q, porteurs 1/x ou prévalence), avec l'option « un parent porteur connu ».

## Export et sauvegarde

- PNG haute définition, SVG, impression / PDF — avec titre, indication, date, auteur et légende automatique.
- **Mode anonyme** : masque noms, années de naissance et notes à l'écran et à l'export.
- Fichier `.pedigree.json` par famille (Enregistrer / Ouvrir) ; l'arbre en cours est aussi sauvegardé automatiquement dans le navigateur.
- Annuler / rétablir illimité (200 étapes).

## Raccourcis

| Touche | Action |
|---|---|
| `P` `C` `G` `F` `R` `S` | parents, conjoint(e), fils, fille, frère, sœur |
| `A` `H` `M` `X` | atteint, porteur hétérozygote, décédé(e), proposant(e) |
| `Suppr` | supprimer la sélection |
| `Ctrl+Z` / `Ctrl+Y` | annuler / rétablir |
| `Ctrl+C` / `Ctrl+V` / `Ctrl+D` | copier / coller / dupliquer |
| `Ctrl+S` / `Ctrl+O` / `Ctrl+P` | enregistrer / ouvrir / imprimer |
| Flèches | déplacer (↑↓ : changer de génération) |
| `O` · `0` · `+` `−` | organiser · ajuster · zoom |

## Références

- Bennett RL et al. *Practice resource-focused revision: Standardized pedigree nomenclature update centered on sex and gender inclusivity.* J Genet Couns 2022.
- Bennett RL et al. *Genetic counseling and screening of consanguineous couples and their offspring.* J Genet Couns 2002.
- Wright S. *Coefficients of inbreeding and relationship.* Am Nat 1922.
