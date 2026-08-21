# Anweisungen für Claude Code

## Auto-Commit & Auto-Push

Dieses Repository ist sicherheitshalber auf GitHub gespiegelt. Committe und pushe **alle Änderungen automatisch, ohne vorher nachzufragen**:

- Nach jeder abgeschlossenen Änderung (neue/bearbeitete Datei) direkt `git add`, `git commit` und `git push` auf `main` ausführen — keine Rückfrage nötig, das ist hiermit für dieses Repo vorab genehmigt.
- Aussagekräftige, kurze Commit-Messages auf Basis der tatsächlichen Änderung schreiben (kein generisches "update").
- Ausnahmen, die weiterhin eine Rückfrage erfordern:
  - `git push --force` oder jede Historie umschreibende Operation
  - Löschen von Dateien, die nicht offensichtlich durch die aktuelle Aufgabe ersetzt/überflüssig geworden sind
  - Änderungen an `.env`-Dateien oder anderen Dateien mit Zugangsdaten/Secrets (diese generell nicht committen)
- Vor Commits mit breitem `git add` kurz `git status` prüfen, damit keine unbeabsichtigten Dateien mitgenommen werden.
