# Delphi — Protocole et variantes

## Origine et principe

Développée à la RAND Corporation dans les années 1950-1960, la méthode Delphi est
une technique de **consultation structurée d'experts** visant à produire un consensus
éclairé (ou à cartographier les divergences) sur des questions d'avenir.

**Principe fondamental** : l'anonymat brise les biais de hiérarchie et de conformité sociale.
Le feedback agrégé permet à chaque expert de réviser son jugement en connaissance de celui des autres.

---

## Protocole classique (2-3 tours)

### Tour 1 — Exploration ouverte
- Questionnaire ouvert : "Quels sont selon vous les développements majeurs dans [domaine] d'ici [horizon] ?"
- Réponses libres, non structurées
- L'équipe organisatrice **code et regroupe** les réponses en items thématiques

### Tour 2 — Évaluation structurée
Pour chaque item issu du Tour 1, les experts évaluent :
- **Probabilité** de réalisation (souvent sur 0-100% ou échelle de Likert)
- **Désirabilité** (souvent : très indésirable → très désirable)
- **Horizon temporel** estimé
- Justification libre (optionnelle)

Les résultats sont agrégés (médiane, quartiles Q1/Q3) et renvoyés à chaque expert
avec sa propre réponse positionnée dans la distribution.

### Tour 3 — Révision éclairée
Les experts peuvent **confirmer ou réviser** leur évaluation du Tour 2.
Ceux qui restent en dehors du consensus (interquartile range) sont invités à justifier leur position.

### Résultats finaux
- **Items consensuels** : faible dispersion autour de la médiane
- **Items divergents** : forte dispersion → à traiter comme incertitudes majeures dans les scénarios
- **Justifications des outliers** : souvent les insights les plus précieux

---

## Critères de qualité d'un panel Delphi

| Critère | Recommandation |
|---|---|
| **Taille du panel** | 15-30 experts pour un Delphi ciblé ; 50-100 pour un Delphi large |
| **Diversité** | Géographique, disciplinaire, sectorielle, générationnelle |
| **Compétence** | Auto-évaluation de l'expertise par domaine |
| **Taux de réponse** | Viser >70% entre les tours (prévoir des relances) |
| **Anonymat** | Strict — même l'organisateur ne doit pas commenter publiquement |
| **Durée totale** | 6-12 semaines pour 2 tours ; 3-6 mois pour 3 tours |

---

## Variantes importantes

### Delphi temps-réel (Real-Time Delphi)
- Tous les tours simultanés sur plateforme numérique
- Les experts voient les résultats agrégés **en temps réel** après leur réponse
- Réduit la durée à quelques jours ou semaines
- Moins de temps pour la réflexion approfondie entre les tours
- Utilisé par le Millennium Project (https://millennium-project.org)

### eDelphi / Delphi numérique
- Plateforme dédiée (ex : eDelphi.org) pour la gestion automatisée des tours
- Facilite la gestion de grands panels internationaux
- Intègre souvent des fonctionnalités d'analyse statistique intégrées

### Policy Delphi
- Objectif : **cartographier les options politiques** plutôt que chercher un consensus
- Les divergences sont aussi précieuses que les convergences
- Adapté aux questions de politiques publiques où le consensus n'est pas l'objectif

### Delphi de groupe (Mini-Delphi / Estimate-Talk-Estimate)
- Groupe restreint en présentiel (5-10 personnes)
- Estimation individuelle → discussion anonymisée → ré-estimation
- Plus rapide mais perd l'anonymat strict

---

## Intégration avec d'autres méthodes

### Delphi + SMIC
Utiliser Delphi pour collecter les probabilités simples et conditionnelles
nécessaires au SMIC (méthode Godet). Le panel d'experts fournit la matière première
probabiliste que SMIC traite ensuite mathématiquement.

### Delphi + Scénarios
- Tour 1 Delphi : identifier les tendances et incertitudes clés
- Analyse morphologique ou SMIC : construire les scénarios
- Tour 2 Delphi : valider et probabiliser les scénarios produits

### Delphi + CLA
Utiliser Delphi pour explorer les différences de worldview entre experts :
les divergences persistantes au Tour 3 révèlent souvent des différences de Niveau 3 (CLA).

---

## Erreurs fréquentes à éviter

1. **Panel trop homogène** → faux consensus, confirmation bias
2. **Questions trop vagues** → réponses inutilisables au Tour 2
3. **Trop de questions** → fatigue, taux d'abandon
4. **Feedback trop directif** → pression vers le consensus au détriment des outliers précieux
5. **Ignorer les justifications** → perdre la substance au profit des chiffres
6. **Pas de restitution aux experts** → démotivation pour les prochains tours
