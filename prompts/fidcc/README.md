# Prompts FIDCC

Adapter les champs entre accolades avant utilisation. Fournir les documents dans un espace privé. Ces prompts originaux ne copient pas les collections externes.

## Fiscalité
Analyser {question} pour {statut fiscal}, exercice {année}, opérations du {dates}. Vérifier les sources officielles applicables. Donner conclusion, articles et liens, calculs, impact client, actions et informations manquantes. Ne pas inventer taux ou échéances.

## Comptabilité
Contrôler la balance et le journal fournis pour {période}, en {devise}. Vérifier équilibres, mouvements et doublons; identifier les lignes concernées et proposer des écritures équilibrées à valider. Ne pas modifier les données originales.

## Contrat
Auditer ce contrat pour défendre {partie}. Présenter risques par clause et priorité, puis proposer des clauses de remplacement. Vérifier les fondements officiels et signaler les annexes manquantes.

## Factures
Lire ces documents facture par facture. Il y a {nombre ou inconnu} factures, avec {pagination ou inconnue}. Exclure les BL du décompte comptable. Extraire désignation et montant des articles, distinguer HT/TVA/TTC/net à payer, utiliser null pour l'inconnu et signaler les incohérences avec page source.

## Note client
Transformer les faits fournis en une note FIDCC pour {destinataire}, au format {Word/PDF/Excel}. Séparer faits et hypothèses, citer les sources utiles et contrôler la présentation du fichier.
