# 🗺️ Board Layout & Notation – FZFOB Chess

This document outlines the notation system used in **Flanking Zone Field of Battle (FZFOB) Chess**, which expands classical chess to a 10×10 grid. The goal is to retain compatibility with traditional notation where possible while clearly denoting the additional Flanking Zone (FZ) squares.

---

## 📐 Board Dimensions

- **Total Grid**: 10 files × 10 ranks
- **Field of Battle (FOB)**: Central 8×8 square (files `a`–`h`, ranks `1`–`8`)
- **Flanking Zone (FZ)**:
  - **Files**: `θ` (left), `χ` (right)
  - **Ranks**: `0` (bottom), `9` (top)

---

## 🔠 File and Rank Naming

| Type           | Files         | Ranks        |
|----------------|---------------|--------------|
| Flanking Zone  | `θ`, `χ`      | `0`, `9`     |
| Field of Battle| `a`–`h`       | `1`–`8`      |

All classical square names (`a1` through `h8`) are preserved. New squares are named by combining their flank file/rank with the usual format. For example:

- `θ2`: Left flank square in rank 2
- `f9`: Top flank square above FOB file `f`
- `χ7`: Right flank square in rank 7
- `e0`: Bottom flank square below FOB file `e`

---

## ♟ Notation Guidelines

### ✅ Classical Moves
Use standard algebraic notation for all actions within the Field of Battle (FOB):

- `e4`, `Nf3`, `Bb5`, `O-O`, etc.

---

### ⚔️ Flanking Zone Moves

#### 🧭 Knight Movement Into/Out of the Flank
Only knights can enter or exit the Flanking Zone.

- `Nθ3`: Knight moves to left flank, rank 3
- `Nχ5`: Knight moves to right flank, rank 5
- `Nχ3+`: Knight checks the king from `χ3` (would thus mean the checked king is positioned at `h1`, `g2`, `g4` or `h5`)
- `Nχ6#`: Knight delivers checkmate from `χ6` (would thus mean the checkmated king is positioned at `h8`, `g7`, `g5` or `h4`)

#### 🔄 Returning to the FOB
- `Nθ3-f5`: Knight reenters the FOB from the flank (optional long-form for clarity)
- `Nχ4→e3`: Directional alternative (informal)

---

### ❌ Captures in the Flank

- `N×θ6`: Knight captures a piece on `θ6` (would thus imply the captured piece is also a Knight)
- `N×χ7+`: A Knight captures another Knight on `χ7` that delivers check
- `N×χ8#`: Knight delivers checkmate with a capture of another Knight in the Flank

---

### 👑 Castling
Castling notation remains unchanged and only applies within the FOB:

- `O-O`: Kingside castle
- `O-O-O`: Queenside castle

---

### ✍️ FEN/PGN Support
To be defined. PGN may extend square naming conventions and FEN may require a 10×10 board representation. See [notation-spec](../notation-spec/README.md) (TBD).

---

## 🎨 Visual Reference

```CSS
   θ a b c d e f g h χ
9  * * * * * * * * * *  9
8  * r n b q k b n r *  8
7  * p p p p p p p p *  7
6  * . . . . . . . . *  6
5  * . . . . . . . . *  5
4  * . . . . . . . . *  4
3  * . . . . . . . . *  3
2  * P P P P P P P P *  2
1  * R N B Q K B N R *  1
0  * * * * * * * * * *  0
   θ a b c d e f g h χ
```

*In rendered interfaces, FOB squares follow the standard chessboard color scheme. Flanking Zone squares should be visually distinct—e.g., via alternate color tinting, thicker borders, or other visual cues such as the `*` in the unicode example above.*

---

## 📎 See Also

- [📜 FZFOB Rules Overview](../README.md)
- [♞ Knight Movement & Flanking Strategies](../knight-flank/README.md)
- [📝 FEN & PGN Adaptations (TBD)](../notation-spec/README.md)
  
