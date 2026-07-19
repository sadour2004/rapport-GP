# rapport-GP

Rapport de projet universitaire — module **« Gestion de projets »**.

## ReadyToGo — Service de trottinettes électriques en libre-service à Tanger

Le rapport complet se trouve dans **[`RAPPORT_ReadyToGo.md`](RAPPORT_ReadyToGo.md)**.

### Téléchargement direct (Word & PDF)

Versions prêtes à l'emploi, avec les diagrammes rendus en images et la charte graphique appliquée :

- 📄 **PDF** : [`RAPPORT_ReadyToGo.pdf`](RAPPORT_ReadyToGo.pdf) — [lien de téléchargement direct](https://github.com/sadour2004/rapport-GP/raw/cursor/rapport-readytogo-e15f/RAPPORT_ReadyToGo.pdf)
- 📝 **Word (.docx)** : [`RAPPORT_ReadyToGo.docx`](RAPPORT_ReadyToGo.docx) — [lien de téléchargement direct](https://github.com/sadour2004/rapport-GP/raw/cursor/rapport-readytogo-e15f/RAPPORT_ReadyToGo.docx)

> Les liens « téléchargement direct » pointent vers la branche `cursor/rapport-readytogo-e15f`. Après fusion dans `main`, remplacez `cursor/rapport-readytogo-e15f` par `main` dans l'URL. Depuis GitHub, vous pouvez aussi ouvrir le fichier puis cliquer sur **Download**.

Les figures rendues (Gantt, EVM, burndown, etc.) sont dans [`assets/diagrams/`](assets/diagrams/).

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

### Régénérer les fichiers Word / PDF

Les fichiers `.docx` et `.pdf` fournis ont été générés ainsi (les blocs Mermaid sont
d'abord rendus en PNG dans `assets/diagrams/`, puis intégrés) :

```bash
# 1. Rendu des diagrammes Mermaid -> PNG + markdown intermédiaire
#    (nécessite mermaid-cli et un Chrome/Chromium)
# 2. Word :
pandoc RAPPORT_processed.md -o RAPPORT_ReadyToGo.docx --resource-path=.
# 3. PDF (via HTML stylé + Chrome headless) :
pandoc RAPPORT_processed.md -s --embed-resources --css style.css -o rapport.html
google-chrome --headless=new --print-to-pdf=RAPPORT_ReadyToGo.pdf rapport.html
```

> `RAPPORT_ReadyToGo.md` reste la source ; les diagrammes y sont en **Mermaid**
> (rendu automatique sur GitHub). Les `.docx`/`.pdf` en sont l'export mis en page.

### À compléter par l'équipe

Les champs marqués *[À compléter]* (noms des 5 membres, établissement, filière, enseignant,
date de remise) et les données marquées *« Hypothèse de travail à valider »* doivent être
renseignés/vérifiés avant remise.
