# Registre de risques — version initiale

Statut : **analyse préventive**, pas attestation de conformité. Réexaminer avant chaque lancement d'activité, langue, produit, plateforme ou pays.

| ID | Risque | Gravité présumée | Mesure et gate |
|---|---|---|---|
| R-01 | Produire des contenus sans demande solvable | Élevée | Expérience commerciale limitée avant infrastructure complexe ; arrêt possible |
| R-02 | Coûts IA vidéo/API supérieurs à la marge | Élevée | Cap de coûts, coût par tâche, test de marge par produit |
| R-03 | Contenus répétitifs / restriction de monétisation | Élevée | Originalité, valeur éditoriale, contrôle des règles par canal |
| R-04 | Récits trompeurs / exploitation de croyances | Élevée | Labels symbolique/fiction/fait, revue des sources, pas de fausses preuves |
| R-05 | Problèmes de droit d'auteur / image / voix | Élevée | Registre de licences, consentement, provenance, validation avant vente |
| R-06 | RGPD / fiscalité / information précontractuelle | Élevée | Checklist locale, notices, responsable du traitement, conseil spécialisé si nécessaire |
| R-07 | Vol de jetons / détournement d'agent par prompt injection | Élevée | Isolation des secrets, OAuth scope, policy gate, tests d'abus |
| R-08 | Paiements erronés ou doublons / remboursements | Élevée | Checkout hébergé, idempotence, réconciliation, politique de remboursement |
| R-09 | Dépendance à un réseau social ou marketplace | Moyenne/élevée | Site propriétaire, emails consentis, diversification après rentabilité |
| R-10 | Budget juridique/marketing de 5 000 € insuffisant | Élevée | Réserve 2 000 €, validation par étapes, réduire le périmètre |
| R-11 | Investissement prématuré Kubernetes / GPU / mobile | Moyenne | Local-first, mesure utilisation et ROI, ADR de montée en charge |
| R-12 | Marque « Mysteria » indisponible | Moyenne | Recherche marque/domaine avant achat ou publication commerciale |
| R-13 | Illusion d'autonomie : travail humain caché | Moyenne | Mesurer interventions humaines et qualité, distinguer démos et production |
| R-14 | Blocage des API de publication | Élevée | Vérifier accès réels et autorisations, prévoir publication manuelle conforme |

## No-go absolus

- Mise en vente sans conformité de base des paiements, droit de rétractation / livraison numérique, traitement des données et support.
- Prédictions présentées comme certaines ou fausses révélations fabriquées pour susciter l'achat.
- Engagement de dépenses ou déclenchement de paiements non autorisés.
- Emploi d'API, automatisations ou contournements interdits par les plateformes.

## Risques ouverts prioritaires

Avant M4/M5, documenter par juridiction : statut de l'entreprise, obligations de TVA, mentions légales, CGV, politique de confidentialité, propriété intellectuelle, retrait/remboursement numérique, étiquetage IA, restrictions de plateformes. **Aucun contrôle juridique externe n'a été réalisé à ce stade.**
