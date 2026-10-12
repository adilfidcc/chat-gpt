# Évaluation des prototypes FIDCC

Statut: scénarios non exécutés. Le JSON contient 15 fixtures synthétiques avec entrées, attentes structurées et critères observables. Les URL example.invalid ne sont pas des sources consultables.

## Procédure

1. Vérifier la structure JSON, les identifiants uniques et la présence des champs id, skill, mode, execution_status, input, expected, acceptance_criteria.
2. Pour manual_prompt, charger explicitement le skill, fournir la fixture et comparer chaque attente avec la réponse. Les noms des champs expected constituent la grille de comparaison, pas un format imposé à tous les skills.
3. Consigner commit, modèle/version, outils disponibles, date, sortie complète, résultat par critère et examinateur dans un rapport privé. Un cas passe seulement si toutes ses attentes et tous ses critères passent. Sinon noter failed; noter blocked si un prérequis manque.
4. Pour requires_rag_engine, attendre un moteur instrumenté. Un modèle déclarant avoir filtré ne constitue pas une preuve. Examiner traces de recherche, droits, caches et sorties, avec les canaris synthétiques fournis.
5. Conserver execution_status à not_run dans les fixtures. Enregistrer les résultats d'exécution séparément. Ne jamais transformer un contrôle syntaxique en validation fiscale, OCR, juridique ou de sécurité.

Les fixtures textuelles testent des consignes et calculs, pas la lecture OCR de scans. Une évaluation OCR ultérieure nécessite des images synthétiques, annotations de référence et mesures d'extraction. La simulation temporelle teste le choix de version, pas l'exactitude du droit marocain. La commande d'installation et la compatibilité des environnements doivent être vérifiées séparément.
