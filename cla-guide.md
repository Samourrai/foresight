# Méthodes Godet / LIPSOR — Guide opérationnel

## 1. Analyse structurelle / MICMAC

### Principe
Identifier les variables d'un système et classer leurs relations d'influence mutuelle.

### Étapes
1. **Lister les variables** du système (20-70 variables selon l'ampleur)
2. **Remplir la matrice d'influences directes (MID)** : pour chaque paire (i,j), noter l'influence de i sur j (0 = nulle, 1 = faible, 2 = modérée, 3 = forte, P = potentielle)
3. **Calculer les influences directes et indirectes** (multiplication matricielle)
4. **Classer les variables** dans le plan motricité/dépendance :
   - **Variables motrices** (haute motricité, faible dépendance) → leviers d'action
   - **Variables relais** (haute motricité, haute dépendance) → variables-clés, instables
   - **Variables dépendantes** (faible motricité, haute dépendance) → résultats, indicateurs
   - **Variables exclues** (faible motricité, faible dépendance) → peu pertinentes
   - **Variables autonomes** (au centre) → déconnectées du système

### Pièges courants
- Trop de variables → bruit. Viser 20-40 pour une analyse manuelle.
- Confondre influence et corrélation.
- Oublier les influences indirectes (souvent les plus importantes).

---

## 2. MACTOR — Analyse des acteurs

### Principe
Cartographier les acteurs d'un système, leurs objectifs, leurs alliances et conflits,
pour anticiper leurs comportements et stratégies dans différents scénarios.

### Étapes
1. **Identifier les acteurs** (institutions, groupes sociaux, organisations, individus clés)
2. **Lister leurs objectifs** stratégiques (3-5 par acteur)
3. **Remplir la matrice Acteurs × Objectifs** : position de chaque acteur sur chaque objectif
   (favorable +2/+1, neutre 0, défavorable -1/-2)
4. **Calculer les convergences et divergences** entre acteurs sur les objectifs
5. **Identifier les alliances potentielles et conflits structurels**
6. **Évaluer les rapports de force** (moyens d'action de chaque acteur)
7. **Produire des recommandations stratégiques** : qui mobiliser, qui neutraliser

### Outputs clés
- Tableau des positions acteurs/objectifs
- Graphe de convergences/divergences
- Hiérarchie des acteurs par rapport de force
- Stratégies possibles pour chaque acteur

---

## 3. Analyse morphologique / MORPHOL

### Principe
Explorer le champ des futurs possibles en décomposant le système en composantes
indépendantes, puis en combinant des hypothèses sur chacune.

### Étapes
1. **Décomposer le système** en dimensions indépendantes (5-8 idéalement)
2. **Pour chaque dimension**, formuler 2-4 états futurs possibles (hypothèses)
3. **Construire l'espace morphologique** : toutes les combinaisons possibles
4. **Réduire l'espace** en éliminant les combinaisons incohérentes
5. **Identifier les scénarios** les plus contrastés et pertinents parmi les combinaisons restantes

### Exemple simplifié
| Dimension | Hyp. A | Hyp. B | Hyp. C |
|---|---|---|---|
| Gouvernance mondiale | Fragmentée | Multipolaire | Intégrée |
| Transition énergétique | Bloquée | Partielle | Accomplie |
| IA dans l'économie | Marginale | Transformatrice | Dominante |

→ 3³ = 27 combinaisons → filtrage par cohérence → 5-8 scénarios retenus

---

## 4. SMIC-PROB-EXPERT

### Principe
Probabiliser des hypothèses sur les variables-clés (issues de MICMAC ou de l'analyse
morphologique) et identifier les scénarios les plus probables par consultation d'experts.

### Étapes
1. **Formuler 5-8 hypothèses** sur les variables déterminantes (binaires : réalisée / non réalisée)
2. **Consulter des experts** : chacun donne une probabilité simple et des probabilités conditionnelles
3. **Corriger les probabilités** conditionnelles pour assurer la cohérence mathématique
4. **Calculer la probabilité de chaque scénario** (combinaison d'hypothèses)
5. **Sélectionner les scénarios** les plus probables et les plus contrastés

### Note
SMIC est un outil de quantification, non de narration. Il doit être complété par
une **écriture de scénarios** (narratifs) pour être utile aux décideurs.

---

## 5. Construction de scénarios (synthèse)

### Structure type d'un scénario prospectif (école française)
1. **Titre évocateur** (souvent une métaphore)
2. **Image initiale** : état du monde aujourd'hui, hypothèses de départ
3. **Cheminement** : enchaînement d'événements cohérents menant au futur
4. **Image finale** : description de l'état du monde à l'horizon
5. **Implications** : pour les acteurs, les décideurs, les politiques

### Règle des 4C
- **Cohérence** : pas de contradiction interne
- **Crédibilité** : plausible compte tenu des tendances
- **Clarté** : compréhensible par des non-experts
- **Conséquence** : utile pour la décision
