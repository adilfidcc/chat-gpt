---
name: fidcc-classer-factures
description: Classer et renommer les factures PDF ou images, extraire les champs marocains et produire un index Excel avec anomalies. Utiliser pour préparer les pièces clients et les imports Scan2Sage.
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

# Classement des factures FIDCC

1. Inventorier les PDF et images fournis ; identifier le client et la période sans les déduire arbitrairement.
2. Extraire dans un index : fichier source, page, fournisseur, numéro de facture, date, ICE, IF, devise, HT, TVA, TTC, échéance et statut de lecture. Conserver les identifiants comme texte, avec leurs zéros initiaux. Ne pas propager un ICE ou IF entre factures sur la seule similitude du nom du fournisseur.
3. Marquer « absent » ou « illisible » pour toute valeur non établie. Ne jamais remplacer la date de facture par celle du fichier. Écarter toute qualification de déductibilité automatique.
4. Vérifier HT + TVA = TTC, signes des avoirs et cohérence des totaux. Signaler les arrondis avec une tolérance explicite. Ne pas mélanger les devises.
5. Repérer les fichiers identiques par empreinte et les doublons possibles par fournisseur, numéro, date et TTC. Conserver tous les originaux ; ne supprimer aucun document.
6. Copier les pièces vers Client/Exercice/Mois/Fournisseur. Utiliser AAAA-MM-JJ_Fournisseur_Numero.ext seulement si ces champs sont établis. Placer les cas incertains dans A_VERIFIER avec un identifiant unique. Éviter tout écrasement de fichier.
7. Livrer un index Excel ou CSV avec liens vers les copies, un journal ancien nom/nouveau nom et la liste des anomalies. Compter les fichiers entrants, copiés, doublons et pièces à vérifier.
8. Pour un export Sage, obtenir le format attendu et la correspondance des comptes, journaux et codes TVA. Ne pas annoncer une compatibilité Sage sans validation du fichier importable.
