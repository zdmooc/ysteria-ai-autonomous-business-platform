# Operating model — hypothèses, expériences et apprentissage

## Objectif

Tester si une offre crée de la valeur et peut vendre avec une marge viable. **Les vues ne sont pas des ventes.** L'agent doit rechercher les preuves contraires aussi bien que favorables.

## Carte d'expérience (une par hypothèse)

| Champ | Exemple initial / règle |
|---|---|
| Venture | Mysteria |
| Identifiant | EXP-MYS-001 |
| Segment | Public francophone intéressé par les mystères historiques |
| Problème client | Trouver un guide original distinguant récit, sources et hypothèses |
| Offre | Guide PDF/ebook thématique (titre et sujet à tester) |
| Prix | 6,99 € (hypothèse) |
| Acquisition | Article blog + vidéo courte sur canal autorisé |
| Mesure | Sessions uniques, clics, checkout initié, ventes réglées, remboursement, coût de production |
| Budget maximal | Soumis à l'enveloppe validation commerciale de 500 € ; plafond de l'expérience à approuver |
| Durée / échantillon | À définir avant le test pour éviter les conclusions opportunistes |
| Critère continuer | Seuil de conversion et contribution **défini avant lancement** sur données suffisantes |
| Critère arrêter | Faible intérêt / marge négative persistante / échec conformité / coût hors enveloppe |
| Responsable | Agent propose ; opérateur approuve dépenses et activation en production |

Aucun taux de conversion, TAM, CAC ou chiffre d'affaires n'est affirmé à l'avance. Les critères numériques doivent être documentés selon les coûts et la taille du test.

## Événements minimum

```
opportunity_created
hypothesis_approved
asset_generated
asset_reviewed
publication_scheduled
publication_delivered
product_viewed
checkout_started
payment_confirmed
refund_completed
cost_recorded
experiment_evaluated
decision_approved
```

Chaque événement porte `timestamp`, `venture_id`, `experiment_id`, `source_channel` si pertinent, `cost_eur` si disponible, et une référence vérifiable. Ne pas enregistrer inutilement de données personnelles.

## Mesures et règles de calcul

- Conversion = achats confirmés / sessions qualifiées (indiquer la fenêtre et le périmètre).
- CA net HT = paiements encaissés HT − remboursements/avoirs HT.
- Marge sur contribution = CA net HT − coûts variables attribués (paiement, plateforme, production IA, support, acquisition).
- CAC = coût d'acquisition attribué / nouveaux clients payants attribuables.
- Payback = contribution cumulée par client / CAC, lorsque les données le permettent.
- Traiter le temps humain comme une **métrique séparée** si non comptabilisé dans le budget cash.

## Cycle de décision

1. Agent Research cite ses sources et explicite ses incertitudes.
2. Proposition avec alternatives, estimation de coûts et hypothèse falsifiable.
3. Approbation du périmètre et plafond financier par l'opérateur.
4. Production originale, contrôle qualité, conformité et droits.
5. Diffusion sur canaux autorisés, collecte consentie de mesures.
6. Réconciliation des encaissements, remboursements et coûts.
7. Recommandation documentée : **continuer / modifier / arrêter**.
8. Arbitrage humain pour toute nouvelle dépense, prix hors bornes ou nouvelle activité.

## Tableau de preuves

| Preuve attendue | Actuelle |
|---|---|
| Hypothèse de valeur écrite | Définie, non testée |
| Produit fini et droits revus | Non |
| Checkout sandbox | Non |
| Publication réelle conforme | Non |
| Premier paiement réel | Non |
| Contribution et coûts rapprochés | Non |
| Décision d'itération justifiée | Non |

Le passage en `EVIDENCED` exige une référence à une observation, un test, un commit, un rapport financier ou un runbook, selon le cas.
