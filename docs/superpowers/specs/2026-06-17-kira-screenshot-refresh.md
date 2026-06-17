# Kira Screenshot Refresh — Design Spec

**Date:** 2026-06-17  
**Scope:** Replace 7 stale Kira screenshots in the showroom with new images that reflect the rethemed Kira UI (dark navy nav bar, colored lozenges, new tab bar with LangFuse/MLflow).

## Background

Kira's UI was rethemed significantly after the showroom screenshots were taken. The old images show a light beige/cream Kira with a teal logo and flat nav. The new UI has a dark navy header, white content area, compact colored lozenges, and a tab bar that now includes LangFuse and MLflow tabs.

## Image Mapping

All new source images come from:
`resources/lb2645-new-kira-mlflow-screenshots/`

All destination images go into:
`content/modules/ROOT/images/`

Images are copied with their **new filenames** and ADoc references are updated to match.

### Module 01 — Problem Domain (`03-module-01-problem-domain.adoc`)

| Old filename | New filename | What it shows |
|---|---|---|
| `kira-step-01-dashboard.png` | `kira-dashboard-zoomed-fullscreen.png` | Dashboard with 2 tickets, clean view of new nav and lozenges |
| `kira-step-02-ticket-detail.png` | `kire-ticket-portrait.png` | Full ticket detail (apache/httpd), includes Issues section |
| `kira-step-03-chatbot.png` | `kira-chatbot.png` | Chatbot panel showing a live conversation |

### Module 02 — Environment (`04-module-02-environment.adoc`)

| Old filename | New filename | What it shows |
|---|---|---|
| `kira-dashboard-web-ticket.png` | `kira-dashboard-fullscreen.png` | Full dashboard with 6 tickets incl. ticket #4 (RHEL web server apache→httpd) |
| `kira-web-ticket-detail.png` | `kira-ticket-zoomed-fullscreen.png` | Ticket #2 detail — apache/httpd wrong package name, zoomed and readable |
| `kira-chatbot-closeup.png` | `kira-chatbot-models.png` | Model dropdown open — supports the "choose Open Source models" text |

### Index (`index.adoc`, 150px thumbnail)

| Old filename | New filename | What it shows |
|---|---|---|
| `kira-fullscreen-01.png` | `kira-dashboard-fullscreen.png` | New UI dashboard at thumbnail size |

## Out of Scope

- ADoc prose changes (no text edits, only image references)
- MLflow screenshots (separate concern)
- RocketChat screenshots
- Old image files are left in `images/` (no deletion — may be referenced elsewhere or in archive pages)

## Success Criteria

- All 6 ADoc `image::` directives updated to new filenames
- 7 new image files present in `content/modules/ROOT/images/`
- No broken image references in active pages
- Visual check: new screenshots show dark navy Kira nav, not the old beige theme
