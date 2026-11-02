---
name: fidcc-verifier-etats
description: Vérifier les concordances des états comptables. Utiliser sur demande
  explicite pour tester ce moteur sur des fichiers de contrôle.
---

## Consignes FIDCC prioritaires

- Répondre en français et utiliser les devises réellement présentes dans les données.
- Confirmer société, période, unités, référentiel et correspondance des colonnes avant les calculs.
- Utiliser les fichiers fournis ou les connecteurs réellement disponibles. Ne pas prétendre être connecté à Sage.
- Pour un dossier marocain, ne pas appliquer automatiquement US GAAP, ASC, SOX, FICA, FUTA ou 401(k). Distinguer méthode de contrôle et règle juridique. Vérifier séparément les règles marocaines à jour et leurs sources officielles.
- Référencer chaque anomalie par fichier, feuille et ligne ou pièce. Distinguer erreur certaine, écart à expliquer et donnée manquante. Ne jamais inventer une justification.
- Effectuer les calculs par programme ou formules vérifiables. Préserver les sources. Proposer les écritures sans les comptabiliser automatiquement.
- Ne pas transmettre de données clients à un service externe ni publier de données réelles dans GitHub.
- Utiliser les skills bureautiques disponibles pour les livrables Excel, Word et PDF.

# Contrôle des états FIDCC

Statut : expérimental, ne pas utiliser comme validation autonome de comptes.

Lire references/file_formats.md et references/verification_rules.md. Exécuter `python scripts/reconcile.py --help`. Adapter explicitement les colonnes et catégories attendues ; le moteur et ses libellés sont initialement chinois et emploient des flottants. Vérifier indépendamment les écarts proches du seuil avec Decimal avant conclusion.

Lire references/upstream-skill.md pour la documentation originale. Préserver les fichiers sources et signaler les libellés non traduits. Produire une synthèse française et laisser les rapprochements ambigus en revue humaine.
