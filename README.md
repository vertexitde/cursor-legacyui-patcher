# Cursor Layout Patcher

Stellt das volle **Change Layout**-Menü wieder her (u. a. Agent, Editor, Zen, Browser, Toggles).  
Patcht `workbench.desktop.main.js` und aktualisiert die Checksums in `product.json` (optional `nls.messages.json`).

## Kurzinfo

- **Referenz (altes Menü):** `C:\Program Files\cursor-old` (falls vorhanden).
- **Aktuelle User-Installation:** typisch `%LOCALAPPDATA%\Programs\cursor`.

**Vor dem Patchen:** Cursor **komplett beenden**, dann im passenden Ordner `run-patcher.bat` ausführen (oder `patcher.ps1` mit PowerShell).

---

## Patcher nach Cursor-Version

Sortierung: **neueste Version oben**. Ordner unter `Outdated\` sind archivierte / ältere Patch-Sätze, bleiben aber nutzbar, wenn deine installierte Cursor-Version exakt passt.

| Cursor-Version | Status | Ordner / Patcher |
|----------------|--------|------------------|
| **2.7.0-pre.105** | Aktuell | `2.7.0-pre.105.patch.0\` |
| 2.7.0-pre.87 | Outdated | `Outdated/2.7.0-pre.87.patch.0\` |
| 2.7.0-pre.84 | Outdated | `Outdated/2.7.0-pre.84.patch.0\` |
| 2.7.0-pre.78 | Outdated | `Outdated/2.7.0-pre.78.patch.0\` |
| 2.7.0-pre.73 | Outdated | `Outdated/2.7.0-pre.73.patch.0\` |
| 2.7.0-pre.67 | Outdated | `Outdated/2.7.0-pre.67.patch.0\` |
| 2.7.0-pre.63 | Outdated | `Outdated/2.7.0-pre.63.patch.0\` |
| 2.7.0-pre.61 | Outdated | `Outdated/2.7.0-pre.61.patch.0\` |
| 2.7.0-pre.60 | Outdated | `Outdated/2.7.0-pre.60.patch.0\` |
| 2.7.0-pre.59 | Outdated | `Outdated/2.7.0-pre.59.patch.0\` |
| 2.7.0-pre.55 | Outdated | `Outdated/2.7.0-pre.55.patch.0\` |
| 2.7.0-pre.53 | Outdated | `Outdated/2.7.0-pre.53.patch.0\` |
| 2.7.0-pre.45 | Outdated | `Outdated/2.7.0-pre.45.patch.0\` |
| 2.7.0-pre.43 | Outdated | `Outdated/2.7.0-pre.43.patch.0\` |
| 2.7.0-pre.41 | Outdated | `Outdated/2.7.0-pre.41.patch.0\` |
| 2.7.0-pre.35 | Outdated | `Outdated/2.7.0-pre.35.patch.0\` |
| 2.7.0-pre.31 | Outdated | `Outdated/2.7.0-pre.31.patch.0\` |
| 2.7.0-pre.27 | Outdated | `Outdated/2.7.0-pre.27.patch.0\` |
| 2.7.0-pre.18 | Outdated | `Outdated/2.7.0-pre.18.patch.0\` |
| 2.7.0-pre.17 | Outdated | `Outdated/2.7.0-pre.17.patch.0\` |
| 2.7.0-pre.16 | Outdated | `Outdated/2.7.0-pre.16.patch.0\` |
| 2.7.0-pre.1 | Outdated | `Outdated/2.7.0-pre.1.patch.0\` |
| **2.6.19** | Aktuell | `2.6.19.patch.0\` |
| **2.6.18** | Aktuell | `2.6.18.patch.0\` |
| 2.6.13 | Outdated | `Outdated/2.6.13.patch.0\` |
| 2.6.12 | Outdated | `Outdated/2.6.12.patch.0\` |
| 2.6.8 | Outdated | `Outdated/2.6.8.patch.0\` |
| 2.6.0-pre.43 | Outdated | `Outdated/2.6.0-pre.43.patch.0\` |
| 2.6.0-pre.33 | Outdated | `Outdated/2.6.0-pre.33.patch.0\` |
| 2.5.26 | Outdated | `Outdated/2.5.26\` |
| 2.5.25 | Outdated | `Outdated/2.5.25\` |

### Sonstiges (ohne feste Versionsnummer)

| Beschreibung | Dateien |
|--------------|---------|
| Generischer / älterer Patcher im Repo-Root (nicht an eine der Tabellenversionen gebunden) | `patcher.ps1`, `run-patcher.bat` |

---

## Hinweise

- **Immer den Patcher nutzen, der zu deiner exakten Cursor-Version passt** (siehe `product.json` → `version` oder *About*). Falsche Patch-Sätze führen zu „Targets not found“ oder kaputtem Workbench-JS.
- **Outdated** heißt nur: es gibt neuere Patch-Ordner im Repo; der alte Ordner kann weiterhin stimmen, wenn deine Installation noch auf dieser Version steht.
- Ab **2.7.0-pre.87+** enthält `buildContent` u. a. **`appendGlassWindowButton`** („Switch to Glass Window“) — die aktuellen Patch-Sätze behalten das am Ende bei.

---

*Kurzfassung auch in `README.txt`.*
