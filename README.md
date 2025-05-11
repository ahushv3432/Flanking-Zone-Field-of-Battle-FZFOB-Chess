# Flanking Zone Field of Battle (FZFOB) Chess

**FZFOB Chess** is a new 10×10 chess variant that builds on the rules of classical chess and Chess960. It introduces a surrounding “Flanking Zone” that only knights can enter, expanding the board without overcomplicating the game. The result is a tactically rich variant with new opening dynamics, creative mobility, and minimal rule changes.

---

## 📌 Variant Summary

- The game is played on a **10×10 board**.
- The inner **8×8 grid** (a1–h8) is the **Field of Battle (FOB)**, where all traditional rules apply.
- The surrounding ring (files `θ` and `χ`, and ranks `0` and `9`) is the **Flanking Zone**, accessible **only by knights**.
- All **non-knight pieces** must remain inside the FOB at all times.
- Opening theory expands: **26 legal opening moves**, up from 20 in classical chess.
- **Notation extension** uses Greek letters and zero-based ranks for clarity and engine friendliness.

---

## 🧭 Board Layout (Start Position)

FZFOB is played on a 10×10 board with a classical 8×8 center (Field of Battle) and a surrounding Flanking Zone. The flank columns are labeled `θ` and `χ` in tribute to the variant’s roots.

```CSS
   θ a b c d e f g h χ 
9  * * * * * * * * * *
8  * r n b q k b n r *
7  * p p p p p p p p *
6  * . . . . . . . . *
5  * . . . . . . . . *
4  * . . . . . . . . *
3  * . . . . . . . . *
2  * P P P P P P P P *
1  * R N B Q K B N R *
0  * * * * * * * * * *
```

- Pieces follow standard algebraic positions inside the central 8×8 Field of Battle (a1–h8).
- The outermost rank and file (0, 9, θ, χ) form the Flanking Zone.
- Knights can move into and out of the Flank. All other pieces must remain entirely within the central field.

---

## 📚 Rules Reference

For a full breakdown of gameplay, board setup, notation, and special mechanics, see the [📖 Rules Directory](rules/README.md).

- 🗺️ [Board Layout & Notation](rules/board-notation/README.md)
- ♞ [Knight Movement & Flanking Zone Mechanics](rules/knight-flank/README.md) *(Coming Soon)*
- 🧩 [FEN/PGN Specification](rules/notation-spec/README.md) *(TBD)*

---

## 🧠 Strategic Features

- **Flank-first options:** Knights can open games by jumping into the Flanking Zone, creating new threats or positioning.
- **Enhanced Na3/Nh3 ideas:** Previously dubious corner knight moves become gateways to broader maneuvering.
- **Simplified rule changes:** No modifications to classical piece rules; just one geographic restriction.
- **Engine-friendly design:** 10×10 board supports clean 0-based indexing, minimal encoding adjustments.

---

## 📜 License

This variant is released under the [Creative Commons Zero (CC0) 1.0 license](LICENSE), placing it in the public domain.  
**You are free to use, remix, adapt, or build upon this idea without asking permission or providing attribution.**

---

## 🚧 Future Plans

- 📄 Fully documented rulebook and FEN notation spec  
- ♟️ PGN and GUI support examples  
- 🤖 Sample engine support or play mode  
- 🧪 Playtest scenarios and suggested starting positions

---

## 📫 Feedback / Contributions

Have ideas, diagrams, or even your own fork of this variant? Feel free to open issues or submit PRs.  
Let's shape the FZFOB meta together!

---
