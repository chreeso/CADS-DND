---
title: "Wiki-Regeln"
type: "meta"
aliases:
  - "Regeln"
  - "Frontmatter"
tags:
  - "meta"
knowledge: "party"
---

# Wiki-Regeln

Kurze Sätze. Eine Seite pro Ding. Dateiname = Name der Seite.

## Allgemeine Felder
| Feld | Bedeutung |
|---|---|
| `title` | Name der Seite |
| `type` | `pc`, `npc`, `location`, `organization`, `ship`, `item`, `lore`, `quest`, `session`, `meta`, `index` |
| `aliases` | Andere Schreibweisen. Links darauf funktionieren. |
| `tags` | Erstes Tag = Typ. Dann Thema (`crew`, `sternenzirkel`, `veymora` …). |
| `knowledge` | Wer es weiß: `party`, `theron`, `mixed` |
| `first_seen` | Link auf die Session des ersten Auftritts |

## Wissensstand (`knowledge`)
- `party`: Die ganze Gruppe weiß es.
- `theron`: Nur Theron (der Charakter) weiß es.
- `mixed`: Die Seite enthält geheime Teile. Sie stehen in einer Box:

```
> [!warning] Nur Theron weiß
> Text
```

## Felder je Typ
| Typ | Zusatzfelder |
|---|---|
| `pc` | `player`, `race`, `status` |
| `npc` | `race`, `role`, `affiliation`, `disposition`, `status`, `location` |
| `location` | `location_type`, `region` |
| `organization` | `org_type`, `disposition` |
| `ship` | `ship_type`, `cannons`, `owner`, `status` |
| `item` | `item_type`, `holder`, `magical` |
| `lore` | `lore_type` |
| `quest` | `status`, `giver` |
| `session` | `session`, `date`, `session_title`, `previous`, `next`, `sources`, `locations` |

## Werte
- `disposition`: `freundlich`, `verbündet`, `neutral`, `feindlich`, `unbekannt`
- `status` (NPC): `lebend`, `tot`, `gefangen`, `unbekannt`
- `status` (Quest): `aktiv`, `erledigt`, `gescheitert`
- Links im Frontmatter immer in Anführungszeichen: `"[[Name]]"`

## Schreibweisen
Bei Streit gilt die Schreibweise aus dem Recap. Abweichende Varianten stehen in `aliases`.

## Vorlagen
Ordner `_Templates`. Neue Seite → Vorlage einfügen.
