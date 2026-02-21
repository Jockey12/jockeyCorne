# jockeyCorne

My VIAL layout for the **Corne 3×5 Light MX** — a 36-key split keyboard running [VIAL](https://get.vial.today/) firmware.

## Hardware

| Property  | Value                      |
|-----------|----------------------------|
| Keyboard  | Corne 3×5 Light MX         |
| Firmware  | VIAL                       |
| Keys      | 36 (5 cols × 3 rows + 3 thumb keys per side) |

## Loading the Layout

1. Install [VIAL](https://get.vial.today/) for your OS.
2. Connect your Corne keyboard via USB.
3. Open VIAL → **File → Load saved layout**.
4. Select `jockey.vil` from this repository.

---

## Layers

> **Legend**  
> `___` = transparent (passes through to the layer below)  
> `GUI` = Win / Cmd key  
> `LN` = hold to activate Layer N, tap = the key shown  
> `SFT/x` = hold for Shift, tap for `x`  
> `TD(n)` = tap-dance key (see [Tap Dance](#tap-dance))

---

### Layer 0 — Base (QWERTY + Home Row Mods)

```
,-----+-----+-----+-----+-----.   ,-----+-----+-----+-----+-----.
|  Q  |  W  |  E  |  R  |  T  |   |  Y  |  U  |  I  |  O  |  P  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|GUI/A|ALT/S|CTL/D|SFT/F|  G  |   |  H  |SFT/J|CTL/K|ALT/L|GUI/;|
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  Z  |  X  |  C  |  V  |  B  |   |  N  |  M  |  ,  |  .  |  /  |
`-----+-----+-----+-----+-----'   `-----+-----+-----+-----+-----'
          ,--------+--------+--------.  ,--------+--------+--------.
          | TD(1)  | SFT/⇥  | L2/SPC |  | TD(0)  | L3/↵   | L1/⌫  |
          `--------+--------+--------'  `--------+--------+--------'
```

#### Home Row Mods

Hold a home-row key to use it as a modifier; tap it for the letter:

| Key | Tap | Hold        |
|-----|-----|-------------|
| A   | A   | GUI (Win/Cmd) |
| S   | S   | Alt           |
| D   | D   | Ctrl          |
| F   | F   | Shift         |
| J   | J   | Shift         |
| K   | K   | Ctrl          |
| L   | L   | Alt           |
| ;   | ;   | GUI (Win/Cmd) |

---

### Layer 1 — Symbols

> Activated by **holding** `L1/⌫` (right thumb, inner key).

```
,-----+-----+-----+-----+-----.   ,-----+-----+-----+-----+-----.
|  _  |  '  |  <  |  {  |  ~  |   |  |  |  }  |  >  |  "  |  ?  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  !  |  @  |  #  |  $  |  %  |   |  ^  |  &  |  *  |  (  |  )  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  -  |  =  |  +  |  [  |  `  |   |  \  |  ]  |     |     |     |
`-----+-----+-----+-----+-----'   `-----+-----+-----+-----+-----'
          ,--------+--------+--------.  ,--------+--------+--------.
          |  ___   |  ___   |  ___   |  |  ___   |  ___   | [LY1] |
          `--------+--------+--------'  `--------+--------+--------'
```

---

### Layer 2 — Numbers & Function Keys

> Activated by **holding** `L2/SPC` (left thumb, inner key).

```
,-----+-----+-----+-----+-----.   ,-----+-----+-----+-----+-----.
|  F1 |  F2 |  F3 |  F4 |  F5 |   |  F6 |  F7 |  F8 |  F9 | F10 |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  1  |  2  |  3  |  4  |  5  |   |  6  |  7  |  8  |  9  |  0  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
| F11 | F12 | KP/ | KP* | KP- |   |  ←  |  ↓  |  ↑  |  →  | KP+ |
`-----+-----+-----+-----+-----'   `-----+-----+-----+-----+-----'
          ,--------+--------+--------.  ,--------+--------+--------.
          |  ___   |  ___   | [LY2] |  |  GUI   |   ⌫    |  ___   |
          `--------+--------+--------'  `--------+--------+--------'
```

---

### Layer 3 — Navigation & Media

> Activated by **holding** `L3/↵` (right thumb, middle key).

```
,-----+-----+-----+-----+-----.   ,-----+-----+-----+-----+-----.
|  Y  |  U  |  I  |  O  |  =  |   |BRID |BRIU |PGDN |PGUP |PSCR |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  H  |  J  |  K  |COPY |  -  |   |MPLY |  ←  |  ↓  |  ↑  |  →  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
|  N  |  M  |  ,  |PSTE | F1  |   |MPRV |MUTE |VOLD |VOLU |MNXT |
`-----+-----+-----+-----+-----'   `-----+-----+-----+-----+-----'
          ,--------+--------+--------.  ,--------+--------+--------.
          |  GUI   |  SFT   |  CTL   |  |  ALT   |  ___   |  ___   |
          `--------+--------+--------'  `--------+--------+--------'
```

| Symbol | Action                  |
|--------|-------------------------|
| BRIU   | Brightness up           |
| BRID   | Brightness down         |
| PSCR   | Print Screen            |
| MPLY   | Media Play/Pause        |
| MPRV   | Media Previous track    |
| MNXT   | Media Next track        |
| MUTE   | Mute                    |
| VOLU   | Volume up               |
| VOLD   | Volume down             |
| COPY   | Copy (KC_COPY)          |
| PSTE   | Paste (KC_PSTE — QMK/VIAL alias for KC_PASTE) |

---

### Layer 4 — Mouse

> This layer is available for assignment (e.g. via a combo or layer key).

```
,-----+-----+-----+-----+-----.   ,-----+-----+-----+-----+-----.
|  _  |  Q  | WH↑ |  E  |  R  |   |  _  |  _  |  _  |  _  |  _  |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
| CTL |BTN1 |BTN2 |BTN3 |  F  |   |  _  | MS← | MS↑ | MS↓ | MS→ |
+-----+-----+-----+-----+-----+   +-----+-----+-----+-----+-----+
| SFT |  Z  | WH↓ |  C  |  V  |   |  _  |  _  |  _  |  _  |  _  |
`-----+-----+-----+-----+-----'   `-----+-----+-----+-----+-----'
          ,--------+--------+--------.  ,--------+--------+--------.
          |  ___   |  ESC   |  SPC   |  |  ___   |  ___   |  ___   |
          `--------+--------+--------'  `--------+--------+--------'
```

| Symbol | Action             |
|--------|--------------------|
| BTN1   | Mouse button 1 (left click)  |
| BTN2   | Mouse button 2 (right click) |
| BTN3   | Mouse button 3 (middle click)|
| WH↑/↓  | Mouse wheel up/down          |
| MS←→↑↓ | Mouse cursor movement        |

---

## Tap Dance

Tap-dance keys behave differently based on how you press them:

| Key   | Single Tap    | Hold         | Tapping Term |
|-------|---------------|--------------|--------------|
| TD(0) | Tab           | GUI (Win/Cmd)| 170 ms       |
| TD(1) | Delete        | Escape       | 100 ms       |
| TD(2) | One-shot GUI  | Layer 1      | 180 ms       |

- **TD(0)** is on the right thumb (outermost key).
- **TD(1)** is on the left thumb (outermost key).
- **TD(2)** is defined in VIAL but not yet assigned to any key position in the current layout.

---

## Combos

The following output keys are defined (trigger keys can be configured in VIAL):

| # | Output Key |
|---|-----------|
| 0 | `[`       |
| 1 | `]`       |
| 2 | `-`       |
| 3 | `'`       |
| 4 | `(`       |
| 5 | `)`       |

---

## Settings

| Setting | Value | Description                    |
|---------|-------|--------------------------------|
| Tapping term | 175 ms | Default hold/tap decision time |
| Auto-shift timeout | 180 ms | — |
