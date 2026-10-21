# Memory Card Game — Unity

> University seminar paper · Course "Virtual Reality Systems" · University of Kragujevac · 2024

Unity C# coursework containing card-flipping, pair-matching and scoring scripts. The repository contains scripts rather than a complete ready-to-open Unity project.

---

## Gameplay

- **Grid configuration:** the script declares 6 × 6 positions but provides only 8 card IDs (4 pairs). Align these before running to avoid an index-out-of-range error.
- **Mechanics**: Click to reveal a card, find its matching pair
- **Scoring**: Score increases for each matched pair; attempts tracked
- **Restart**: Reload scene to shuffle and play again

---

## Scripts

| File | Description |
|---|---|
| `GameControllerScript.cs` | Grid generation, card layout, match checking logic |
| `MainImageScript.cs` | Individual card behaviour (flip, sprite display) |
| `ButtonScript.cs` | UI button interactions (restart) |

### Key implementation details

- Fisher-Yates shuffle for random card placement
- Coroutine-based match checking with 0.5s delay on mismatch
- `TextMesh` score and attempt display
- `SceneManager.LoadScene` for restart

---

## Tech Stack

`Unity` · `C#` · `UnityEngine.SceneManagement`
