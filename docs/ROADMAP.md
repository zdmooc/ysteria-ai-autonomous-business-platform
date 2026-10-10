# Roadmap orientée première vente et boucle autonome mesurable

**État initial : cadrage seulement (10/10/2026).** Les jalons sont des objectifs, pas des réalisations. Une preuve Git, un test et, lorsque pertinent, un événement de production sont nécessaires pour toute fermeture.

## Règle de priorisation

**Ne jamais avancer l'industrialisation plus vite que la validation commerciale.** La chaîne cible est :

opportunité → produit → publication → vente → mesure de marge → décision suivante.

## Jalons

| Gate | Livrable | Definition of Done vérifiable | Statut |
|---|---|---|---|
| **M0** | Vision, budget, architecture, décisions, risques et expériences | Documents versionnés, hypothèses et décisions explicites | **EVIDENCED — documentation uniquement** |
| **M1** | Validation d'offre et socle local | Fiche hypothèse, 1 produit test défini, site/API/DB minimal reproductible, CI verte | PLANNED |
| **M2** | Boucle autonome **simulée** | Agent produit une proposition, politique refuse une action hors budget, événements/audit, mesure marge sur commandes fictives | PLANNED |
| **M3** | Produit et contenu originaux | Offre numérique prête, fiche sources/droits, article + 1 format vidéo, revue qualité, traduction relue | PLANNED |
| **M4** | Boutique web et distribution contrôlée | Landing page, checkout sandbox, délivrabilité produit, au plus 2 canaux autorisés, suivi source de trafic | PLANNED |
| **M5** | Première vente réelle instrumentée | Conformité et comptes activés, encaissement autorisé, livraison, support, remboursement testé, coûts réconciliés | PLANNED |
| **M6** | Décision d'investissement fondée sur données | Tableau de contribution, CAC/conversion, décision enregistrée (itérer / arrêter / étendre), backup/restore et runbook | PLANNED |

Les marketplaces Amazon et applications mobiles sont **hors chemin critique M1–M6** ; intégrations ultérieures uniquement si intérêt client mesuré, accès autorisé et marge acceptable.

## Périmètre MVP fixe

- **Une première venture : Mysteria** (contenus culturels et interprétation symbolique présentés honnêtement).
- **Un seul produit initial** : guide numérique original ; prix de test suggéré **6,99 €** (hypothèse à valider).
- **Site responsive d'abord** ; pas d'application native.
- **Français d'abord**, puis anglais avec assurance qualité ; pas de 10 langues simultanées.
- **Un site et au plus deux canaux externes**, pas de production de masse.
- **Trois fonctions d'agents réellement utiles** : opportunité, production contrôlée, mesure/décision. Les autres restent des responsabilités de workflow, pas des microservices séparés.

## Politique de stop / go

- Pas de paiement réel avant conformité, livraison, support et remboursement testés.
- Pas de diffusion automatique avant vérification droits, normes éditoriales et accès API.
- Pas d'achat publicitaire automatique sans budget préautorisé et plafond technique démontré.
- Pas de déploiement Kubernetes/GPU avant mesure d'une contrainte de disponibilité, performances ou coûts.
- Une faible conversion est un résultat valable ; arrêter une expérimentation est une décision de succès méthodologique, pas une panne du logiciel.

## Estimation de séquencement

**8–16 semaines indicatives** pour un MVP commercial restreint en développement personnel à temps partiel, non garanti. Les autorisations des canaux, la conformité et la validation marché peuvent allonger fortement le calendrier. Une entreprise largement autonome et multi-marques est un objectif plus lointain et non chiffré ici.

## Prochaine action technique M1

Créer uniquement le squelette local minimal (frontend, API, DB, tests, Docker Compose, CI) et le registre d'hypothèses. Aucun compte payant ou cloud permanent n'est une dépendance à cette étape.
