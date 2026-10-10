# Autonomous AI Business Platform — première activité : Mysteria

> Dépôt : `zdmooc/ysteria-ai-autonomous-business-platform`. Le slug historique `ysteria` est conservé ; **Mysteria** est une marque de travail, à vérifier avant usage commercial.

## Vision

Construire un **système d'exploitation d'entreprise numérique piloté par des agents IA** qui :
1. découvre des opportunités commerciales vérifiables ;
2. propose et produit des biens ou services originaux ;
3. les distribue par des canaux autorisés (site, contenus, marketplaces, éventuellement applications) ;
4. mesure encaissements, coûts complets, satisfaction et marge ;
5. propose de poursuivre, corriger ou arrêter une expérimentation dans les limites d'autorité fixées.

**La plateforme technologique est indépendante du secteur. Mysteria est sa première activité commerciale**, consacrée aux traditions ésotériques, aux interprétations symboliques, aux mystères et aux contenus culturels documentés. D'autres activités pourront être lancées si la demande réelle le justifie.

## Trois périmètres

| Couche | Mission | Limite |
|---|---|---|
| **Core Platform** | Agents, orchestration, outils, permissions, paiements, audit, coûts | Aucune dépendance au thème ésotérique |
| **Business Ventures** | Marques, produits, catalogues, contenus, langues, canaux de vente | Mysteria est le premier cas d'usage |
| **Experimentation & FinOps** | Hypothèses, tests, attribution, CAC, marge, arbitrages | Réinvestissement soumis aux budgets autorisés |

## Produit de départ

**Une seule boucle commerciale prouvée**, et non neuf agents, dix réseaux sociaux et plusieurs applications dès le départ :

**opportunité → produit → publication → vente → mesure de marge → proposition de décision**.

- Premier canal propriétaire : **site web responsive** et blog en français, puis traduction anglaise après contrôle qualité.
- Première offre à tester : **un guide numérique original** sur un thème culturel/mystérieux, à prix hypothétique de **6,99 €**.
- Acquisition : contenu éditorial et **au plus deux canaux externes** avec intégrations officielles.
- Paiement : fournisseur hébergé (mode test, puis réel après validation de conformité).
- Amazon KDP, plusieurs marques, application mobile, OpenShift et GPU dédiés : **extensions, pas prérequis**.
- Aucune vente ou conversion n'est acquise : chaque hypothèse doit être mesurée.

## Principes non négociables

- **IA décisionnelle, pas pouvoir illimité** : décisions économiques consignées, budgets plafonnés, approbation humaine des dépenses, contrats, premières mises en ligne et changements à risque.
- **Vérité et transparence** : distinguer connaissances établies, hypothèses, traditions, fiction et contenu symbolique ; interdiction de fausses preuves ou témoignages et des ventes fondées sur la peur.
- **Qualité plutôt que volume** : contenu original, droits vérifiés, citations des sources lorsque nécessaires et respect des conditions des plateformes.
- **FinOps dès M1** : coût par produit et par canal, quotas, alerte, coupe-circuit, suivi de marge nette.
- **Local et portable** : conteneurs, API hébergées, infrastructure IaC minimale. Ne pas réserver de cluster Kubernetes/GPU permanent sans démonstration du besoin.
- **Sécurité et conformité** : données minimales, RGPD, droit de la consommation, déclaration de contenus IA, règles des moyens de paiement et marketplaces.

## Références de cadrage

- [Vision et découpage produit](docs/VISION-AND-VENTURES.md)
- [Architecture technique](docs/ARCHITECTURE.md)
- [Budget et financement par étapes](docs/BUDGET-BASELINE.md)
- [Roadmap et preuves de sortie](docs/ROADMAP.md)
- [Expériences commerciales et indicateurs](docs/EXPERIMENTATION.md)
- [Gouvernance des agents et limites d'autonomie](docs/AGENT-GOVERNANCE.md)
- [Risques et conditions de lancement](docs/RISK-REGISTER.md)
- [ADR de séparation cœur / activités](docs/adr/ADR-0001-separate-core-and-ventures.md)

## Statut au 10/10/2026

**PROGRAMME EN PAUSE VOLONTAIRE : priorité à l'obtention d'une mission freelance.** La reprise est conditionnée à la sécurisation d'une mission professionnelle par le porteur du projet ; aucune date de reprise ni budget d'exécution n'est fixé. Le cadrage M0 et les documents existants sont conservés en l'état. Ne pas engager de nouvelles dépenses, lancer des déploiements ou démarrer M1 avant décision explicite de reprise.

**DOCUMENTATION UNIQUEMENT — PAS DE MVP FONCTIONNEL, PAS DE DEPLOIEMENT, PAS DE VENTE.**

M0 = cadrage documentaire initial réalisé. M1–M6 non réalisés ; aucune preuve d'exploitation commerciale n'existe dans ce dépôt.

Dépôts techniques connexes (Terraform, GitOps, architecture agentique) : **réutilisation possible** de motifs, **sans dépendance obligatoire**. Le dépôt `cadrage_202682030` n'est pas modifié par le présent chantier.
