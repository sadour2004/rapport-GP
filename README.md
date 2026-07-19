# rapport-GP

Rapport de projet universitaire — module **« Gestion de projets »**.

## ReadyToGo — Service de trottinettes électriques en libre-service à Tanger

Le rapport complet se trouve dans **[`RAPPORT_ReadyToGo.md`](RAPPORT_ReadyToGo.md)**.

Il couvre l'intégralité des sept étapes demandées (définition, planification, organisation,
gestion des risques, communication, suivi & indicateurs, livraison), ainsi qu'une
**simulation pédagogique des problèmes rencontrés**, l'analyse économique (budget en
3 scénarios, tarification, seuil de rentabilité), l'identité de marque, les recommandations,
la bibliographie et les annexes.

### Format et visualisation

- Le rapport est rédigé en **Markdown**. Les diagrammes (Gantt, courbe EVM, burndown,
  arbres à problèmes/objectifs, WBS, matrices, organigramme) utilisent la syntaxe
  **Mermaid**, rendue nativement sur GitHub.
- Pour l'afficher avec les diagrammes : ouvrir le fichier directement sur GitHub, ou
  dans un éditeur Markdown compatible Mermaid (VS Code + extension Mermaid, Obsidian, Typora…).

### Export en Word / PDF (optionnel)

Si `pandoc` est disponible :

```bash
pandoc RAPPORT_ReadyToGo.md -o RAPPORT_ReadyToGo.pdf
# ou
pandoc RAPPORT_ReadyToGo.md -o RAPPORT_ReadyToGo.docx
```

> Les blocs Mermaid nécessitent un filtre (par ex. `mermaid-filter`) pour être convertis
> en images lors de l'export ; à défaut, ils apparaîtront sous forme de code.

### À compléter par l'équipe

Les champs marqués *[À compléter]* (noms des 5 membres, établissement, filière, enseignant,
date de remise) et les données marquées *« Hypothèse de travail à valider »* doivent être
renseignés/vérifiés avant remise.
