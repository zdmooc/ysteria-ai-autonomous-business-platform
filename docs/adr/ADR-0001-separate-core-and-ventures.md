# ADR-0001 — Séparer le moteur autonome des activités commerciales

- **Date :** 2026-10-10
- **Statut :** ACCEPTED FOR MVP DESIGN (pas de preuve d'implémentation)
- **Portée :** architecture conceptuelle du dépôt

## Contexte

L'idée initiale était une application mobile d'ésotérisme. Elle a évolué en entreprise numérique multi-activités pouvant gérer sites, contenus, produits numériques, boutiques, réseaux et marketplaces. Concevoir toute la plateforme autour de Mysteria créerait un couplage risqué et rendrait coûteux un pivot si la première offre ne se vend pas.

## Décision

1. Le **Core Platform** regroupe les services techniques réutilisables : orchestration, gouvernance, finances, expérimentations, paiement et canaux.
2. Chaque **Business Venture** possède ses propres produits, marque, contraintes, traductions et contenus.
3. Le **registre des expériences** stocke hypothèses, budget, observation et décision ; il n'affirme aucune rentabilité sans chiffres vérifiables.
4. La venture Mysteria est le **premier banc d'essai**, et non la raison d'être exclusive du core.
5. **Monorepo initial**, modules séparés ; aucun microservice/cluster imposé sans besoin mesuré.

## Conséquences

- Plus facile de tester une autre activité si Mysteria échoue commercialement.
- Validation explicite des interfaces inter-modules et des identifiants tenant/venture.
- Petite complexité supplémentaire de modélisation compensée par une capacité de réutilisation.
- Aucun budget supplémentaire dédié à une seconde marque tant que la boucle pilote n'est pas mesurée.

## Alternatives rejetées

- Application mobile Mysteria monolithique comme unique produit : trop restrictive au regard du besoin.
- Multi-tenant multi-marque intégral et microservices dès M1 : sur-ingénierie avant la première vente.
- AI CEO autonome sans limites : incompatible avec contrôle du risque, du budget et des obligations externes.
