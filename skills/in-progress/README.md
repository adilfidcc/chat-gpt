# In Progress

Beta. These skills are public on purpose: try them and tell me what breaks. They're excluded from the plugin and the top-level README until they graduate to a stable bucket, they get no docs pages, and they can change or disappear without warning.

The plugin won't give you these. Install one directly:

```bash
npx skills@latest add mattpocock/skills --skill=<name>
```

- **[loop-me](./loop-me/SKILL.md)**: Grill yourself into implementable workflow specs over multiple sessions, using the current directory as a stateful workspace. User-invoked.
- **[writing-beats](./writing-beats/SKILL.md)**: Shape an article as a journey of beats, choose-your-own-adventure style. Pick a starting beat, write only that beat, then pivot to the next, until the article reaches a natural end.
- **[writing-fragments](./writing-fragments/SKILL.md)**: Grilling session that mines you for fragments (heterogeneous nuggets of writing) and appends them to a single document as raw material for a future article.
- **[writing-shape](./writing-shape/SKILL.md)**: Take a markdown file of raw material and shape it into an article paragraph by paragraph, arguing format choices at each step.
- **[claude-handoff](./claude-handoff/SKILL.md)**: Hand the current conversation off to a fresh background agent that picks up the work immediately, seeded with a handoff summary via `claude --bg`. User-invoked.
- **[setup-ts-deep-modules](./setup-ts-deep-modules/SKILL.md)**: Wire dependency-cruiser into a TypeScript repo so each package is a deep module: implementation hidden in subfolders, reachable only through its entry-point files, tests exercising it through those. User-invoked.

## Prototypes FIDCC

- **[fidcc-fiscalite-maroc](./fidcc-fiscalite-maroc/SKILL.md)**: Analyser une question fiscale marocaine et rédiger une note client sourcée.
- **[fidcc-controle-comptable](./fidcc-controle-comptable/SKILL.md)**: Contrôler une balance ou un journal comptable marocain et proposer des corrections.
- **[scan2sage-lecture-factures](./scan2sage-lecture-factures/SKILL.md)**: Extraire des factures multi-pages ou multi-documents et contrôler leurs montants.
- **[fidcc-documents](./fidcc-documents/SKILL.md)**: Préparer des rapports Word PDF et tableaux Excel cohérents pour FIDCC.
- **[fidcc-audit-contrats](./fidcc-audit-contrats/SKILL.md)**: Auditer un contrat commercial marocain du point de vue de la partie défendue.

Ces prototypes sont exclus du plugin publié. Les charger explicitement dans un environnement compatible pour les évaluer.
