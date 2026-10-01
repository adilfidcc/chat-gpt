# Recherche documentaire FIDCC

Statut: conception de prototype, aucun moteur déployé, corpus chargé ou connecteur ChatGPT installé.

## Chaîne proposée
1. Conserver les originaux dans un stockage privé avec accès par client.
2. Extraire texte et tableaux; OCR seulement si nécessaire, puis vérifier un échantillon et les pages essentielles.
3. Découper par article ou section en conservant titre, page, table, source et version.
4. Indexer texte et représentations vectorielles; filtrer par droits, client et période AVANT la recherche.
5. Rechercher par mots clés et sens; reclasser les passages si les tests démontrent un gain.
6. Rédiger seulement à partir de preuves pertinentes; citer document, version et page/article. S'abstenir quand les preuves sont absentes ou contradictoires.

## Métadonnées requises
Document ID, titre, organisme, URL source, date de publication, début et fin de validité (inconnus admis), date de collecte, version, empreinte du fichier, page/article, langue, client et niveau d'accès. Conserver les anciennes versions; ne pas confondre date de collecte et entrée en vigueur.

## Outils à évaluer
- [Dify](https://github.com/langgenius/dify): prototype visuel avec recherche documentaire et workflows.
- [RAGFlow](https://github.com/infiniflow/ragflow): évaluation sur PDF, scans et tableaux.
- [OpenAI Cookbook](https://github.com/openai/openai-cookbook): exemples pour une intégration sur mesure.
- [prompts.chat](https://github.com/f/prompts.chat): inspiration pour les consignes, pas un moteur documentaire.

Avant installation: vérifier licence et version retenue, ressources de serveur, traitement des données, compatibilité du modèle et coûts API. L'abonnement ChatGPT ne doit pas être supposé couvrir les appels API.

## Première expérimentation
Choisir un petit corpus public et versionné. Préparer des questions avec références attendues, comparer recherche seule et réponse générée, puis mesurer citations correctes et abstentions. Tester absence de réponse, textes périmés, contradictions et instructions malveillantes dans un document. Aucun document client dans ce dépôt public.

## Suite nécessaire
Choisir hébergement, fournisseur de modèles et droits d'accès; charger le corpus privé; tester; puis concevoir la connexion ChatGPT compatible. L'ajout de ces fichiers à GitHub n'active aucune recherche RAG.
