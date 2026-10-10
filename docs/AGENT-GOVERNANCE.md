# Gouvernance : agents, permissions et autonomie graduelle

## Principe

Un **AI CEO** n'est pas détenteur d'un compte bancaire ni propriétaire d'une autorisation générale. C'est un composant de proposition et d'optimisation. Les décisions réelles passent par un moteur de politiques, des permissions vérifiables et des validations humaines.

## Niveaux d'autonomie

| Niveau | Exemple | Exécution |
|---|---|---|
| A0 — Proposition | recherche de sujet, étude de prix, choix de canal | Automatique, sans effet externe |
| A1 — Interne réversible | brouillon, résumé, classification, simulation de marge | Automatique avec audit |
| A2 — Publication préapprouvée | programmation d'un contenu sûr, droits contrôlés, compte officiel | Automatique uniquement après validation des règles et de l'enveloppe |
| A3 — Engagement limité | modification de prix dans bornes ou campagne sous plafond | Déblocage explicite et contrôle technique des limites |
| A4 — Impact élevé | ouverture de compte, contrat, nouvelle marque, transfert, gros budget, suppression, politique fiscale | Validation humaine spécifique obligatoire |

**Par défaut : refus** si permission, état de conformité, limites fournisseur ou preuve d'approbation manquent.

## Matrice d'actions

| Action | Décision IA | Autorisation humaine |
|---|---|---|
| Choisir hypothèse / produire brouillon | Oui | Non pour la proposition |
| Générer une vidéo | Oui, si budget déjà alloué et contenu autorisé | Oui pour dépassement ou nouvelle politique |
| Publier sur un compte social | Préparer/planifier | Autorisation initiale et revue sensible |
| Produire une fiche Amazon KDP | Préparer contenu et métadonnées | Vérification des droits, politique et publication |
| Encaisser via checkout déjà configuré | Workflow technique | Activation de l'offre et paramètres d'encaissement |
| Acheter de la publicité | Proposer | Budget, plafond et périmètre approuvés |
| Rembourser un client | Automatisable sous politique explicite | Hors politique, revue humaine |
| Lancer nouveau site, pays, marque | Proposer | Validation humaine |
| Transferer fonds, signer ou souscrire contrat | Non en autonomie générale | Validation humaine et processus financier indépendant |

## Garde-fous implémentables

- Journal append-only : motif, source, modèle utilisé, version politique, approbateur, budget disponible, action, réponse de l'API, résultat.
- Toutes les API à effet externe sont appelées **par un exécuteur contrôlé**, jamais directement par le modèle.
- Plafond par tâche, jour, mois, venture et fournisseur ; comptabilisation prévisionnelle puis réelle ; aucun retry infini sur APIs facturantes.
- Suspension globale des workers et révocation des jetons en cas d'anomalie.
- Validation de contenu : provenance des sources, incertitude, respect des droits, pas de faux avis/témoignages/identités, pas de manipulation anxiogène.
- Les sources web et messages utilisateurs sont des **données non fiables** : prompt injection et liens malveillants ne deviennent jamais une autorisation.
- Protection des données des clients, consentement, minimisation et demandes RGPD.
- Pour les domaines ésotériques : présenter tarot, prédictions et interprétations comme symboliques/divertissement, non comme certitudes ou diagnostics.
- L'automatisation ne contourne pas les conditions des réseaux, d'Amazon ou des moyens de paiement.

## Preuves de recette requises

1. Tentative de publication non autorisée → refus.
2. Tâche IA dépassant le plafond → refus et signal.
3. Texte externe demandant d'ignorer les politiques → aucun effet sur l'autorisation.
4. Même webhook paiement livré deux fois → une seule commande.
5. Expérience arrêtée → plus de dépense ni publication planifiée.
6. Coupure générale → reprise sûre après autorisation.

Aucune de ces preuves n'est encore produite dans le dépôt ; elles constituent les tests à construire.
