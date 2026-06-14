# CSM Account Dashboard — Adaptavist

A drag-and-drop Kanban board for managing your enterprise book of business.

## How to open it

1. **Clone the repository** (if you haven't already):
   ```bash
   git clone https://github.com/tim3t/Claude-code-dashboard-experiment.git
   cd Claude-code-dashboard-experiment
   ```

2. **Switch to the feature branch:**
   ```bash
   git checkout claude/enterprise-account-kanban-0hazzq
   ```

3. **Open the dashboard:**  
   Double-click `index.html` in Finder (Mac) or File Explorer (Windows), or run:
   ```bash
   # Mac
   open index.html

   # Windows
   start index.html

   # Linux
   xdg-open index.html
   ```

That's it — no server, no install, no build step. It runs entirely in your browser.

## What you get

- **53 enterprise accounts** pre-seeded across 8 status lanes (~$8.5M ARR)
- **Drag and drop** any account card between lanes
- **Live ARR subtotals** per lane update as you move cards
- **Your placements are saved automatically** in browser localStorage — they survive page refreshes and browser restarts (on the same machine/browser)

## Lanes

| Lane | Purpose |
|---|---|
| To Triage | Newly inherited accounts not yet assessed |
| Actively Engaged | Regular cadence, healthy relationship |
| Migration / Project | Active migration or implementation in flight |
| Feature Watch | Waiting on a specific release before next motion |
| Relationship Building | Building or rebuilding contacts |
| No Key Contact | Lost champion — need to find a new one |
| Dormant | Low activity, no current motion |
| At Risk | Health signals declining |

## Resetting to defaults

To reset all account placements back to their original positions, open your browser's developer console (F12) and run:

```javascript
localStorage.removeItem('csm-kanban-v1');
location.reload();
```
