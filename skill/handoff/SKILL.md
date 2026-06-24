---
name: handoff
description: "Écrit une note de passation pour qu'une nouvelle session reprenne le travail. À utiliser en fin de session, avant /clear, ou sur « handoff » / « sauvegarde l'état »."
argument-hint: "À quoi servira la prochaine session ?"
disable-model-invocation: true
---

# handoff

Rédige un document de passation qui résume la session courante pour qu'une nouvelle session reprenne le travail. Reste court : un tremplin, pas une transcription.

Crée le dossier `aidd-docs/handoff/` à la racine du projet courant s'il n'existe pas (et ajoute `aidd-docs/handoff/` au `.gitignore` du projet s'il n'y est pas), écris la note dans `aidd-docs/handoff/<AAAA-MM-JJ-HHMM>.md`, puis affiche le chemin.

Règles :
- Ne duplique jamais un artefact durable (PRD, ADR, diff, issue, commit) → pointe-le par chemin/URL.
- N'inscris jamais de secret ni de donnée sensible (clé d'API, mot de passe, PII) dans la note → remplace-les par un repère générique.
- Adapte la note au focus annoncé pour la suite.
- Termine par une section « skills suggérés » nommant les skills utiles à la prochaine session.
