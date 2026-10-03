---
language:
- de
- en
license: cc-by-4.0
pretty_name: SapientBlock Blockchain Use Cases
size_categories:
- n<1K
task_categories:
- text-retrieval
- question-answering
tags:
- blockchain
- dlt
- distributed-ledger
- use-cases
- enterprise
- german
- industry
- research
configs:
- config_name: default
  data_files:
  - split: train
    path: use_cases.jsonl
---

# SapientBlock Blockchain Use Cases

Der Datensatz enthält **333 dokumentierte Blockchain-Use-Cases aus 74 Branchen** (4 Sektoren), Stand 03.10.2026. Jeder Fall nennt die umsetzende Organisation, Branche, Reifegrad, Projektstatus, Beleglage und Quellen mit Prüfdatum. 333 von 333 Fällen haben die redaktionelle Prüfung mit ausgewiesenem Reviewer und Prüfdatum abgeschlossen.

*English:* 333 documented real-world blockchain use cases from 74 industries, each with the implementing organisation, maturity level, project status, evidence level and dated sources. Every record has German and English titles, summaries and full Markdown content. Licensed under CC BY 4.0.

Der Datensatz ist ein Export der öffentlichen [SapientBlock-Datenbank](https://www.sapientblock.com/blockchain-use-case-datenbank). SapientBlock ist ein öffentliches Research- und Community-Projekt von ShapeNeural Lab.

## Felder

| Feld | Inhalt |
|---|---|
| `id`, `slug` | stabile ID und URL-Kennung |
| `title_de`, `summary_de`, `title_en`, `summary_en` | Titel und Kurzfassung auf Deutsch und Englisch |
| `sector`, `industry`, `provider` | Sektor, Branche, umsetzende Organisation |
| `maturity_level` | Reifegrad: `concept`, `pilot`, `production` |
| `project_status`, `project_status_date` | Projektstatus (z. B. Pilot, Produktiv, Eingestellt) und Datum |
| `evidence_level` | Beleglage: `high`, `medium`, `open` |
| `keywords` | Schlagwörter |
| `date_published`, `date_modified` | Veröffentlichung und letzte Änderung |
| `reviewed_by`, `reviewed_at` | redaktionelle Prüfung (leer, wenn ausstehend) |
| `sources_checked_at`, `source_count`, `citations` | Quellen mit Typ, Prüfdatum und Erreichbarkeit |
| `canonical_url`, `canonical_url_en`, `markdown_url`, `jsonld_url` | Links zur Fallseite (DE/EN) und zu den Maschinenfassungen |
| `content_markdown`, `content_markdown_en` | vollständiger Inhalt der Fallseite als Markdown |
| `source_name`, `source_url`, `required_attribution` | verpflichtende Herkunfts- und Namensnennung |
| `license` | Lizenz-URL |

Der Split heißt aus technischen Gründen `train`; der Datensatz ist kein Benchmark und hat keine Train/Test-Aufteilung.

## Herkunft und Aktualität

- Website: https://www.sapientblock.com/use-cases
- Datenbank-Seite mit Methodik: https://www.sapientblock.com/blockchain-use-case-datenbank
- Katalog: https://www.sapientblock.com/use-cases/catalog.json
- Dataset-Metadaten: https://www.sapientblock.com/use-cases/dataset.jsonld

Der Exportzeitpunkt steht in `export-metadata.json`. Die Website ist die maßgebliche Fassung; dieser Export wird bei größeren Änderungen aktualisiert.

## Lizenz

[CC BY 4.0](https://creativecommons.org/licenses/by/4.0/): Nutzung, Weitergabe und Bearbeitung sind erlaubt, auch kommerziell. **Die Namensnennung ist verpflichtend.** Dabei ist folgende Angabe zu verwenden:

> Quelle: SapientBlock (sapientblock.com), lizenziert unter CC BY 4.0.

Die Angabe soll auf https://www.sapientblock.com verlinken. Bei einzelnen Fällen ist zusätzlich die jeweilige `canonical_url` anzugeben. Die Pflichtangabe ist außerdem maschinenlesbar in jedem Datensatz unter `required_attribution` enthalten.

Die verlinkten Primär- und Sekundärquellen bleiben Eigentum ihrer Rechteinhaber. Der Datensatz enthält Quellenangaben und Links; eine Lizenz an den Inhalten der verlinkten Seiten entsteht daraus nicht.

## Hinweise zur Qualität

Die Beschreibungen werden KI-gestützt recherchiert und formuliert und redaktionell geprüft; der Prüfstand steht in jedem Record. Trotz Quellenangaben gibt es keine Gewähr für Richtigkeit, Vollständigkeit oder Aktualität. Wesentliche Aussagen bitte anhand der Originalquellen prüfen. Die Inhalte sind keine Rechts-, Investitions-, Unternehmens- oder technische Beratung.

## Zitiervorschlag

> SapientBlock (2026): Blockchain-Use-Case-Datenbank. 333 dokumentierte Fälle, Stand 03.10.2026. https://www.sapientblock.com/blockchain-use-case-datenbank

## Kontakt

- Projekt: https://www.sapientblock.com
- Träger: https://shapeneural.com
