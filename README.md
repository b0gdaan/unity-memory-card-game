# Memory Card Game — Unity

> University seminar paper · Course "Virtual Reality Systems" · University of Kragujevac · 2024

A memory card matching game implemented in Unity (C#). Players flip cards to find matching pairs on a 6×6 grid, with score and attempt tracking.

---

## Gameplay

- **Grid**: 6 × 6 cards (4 unique image pairs, randomly shuffled)
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
