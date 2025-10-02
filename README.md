# SURF

> A modern, polished reimplementation of CustomCurve Pro — a Python Tkinter app for creating, editing, and testing custom mouse sensitivity curves. Designed for precision, performance, and a clean dark UI.

[![Release](https://img.shields.io/github/v/release/awarzu/Surf)](https://github.com/awarzu/Surf/releases) [![License](https://img.shields.io/github/license/awarzu/Surf)](LICENSE) [![Stars](https://img.shields.io/github/stars/awarzu/Surf?style=social)](https://github.com/awarzu/Surf/stargazers)

<p align="center">
  <img src="docs/assets/surf_logo.png" alt="Surf logo" width="300"/>
</p>

---

## Table of Contents

1. [Overview](#overview)
2. [Key Features](#key-features)
3. [Installation](#installation)
4. [Controls & Interactions](#controls--interactions-in-app)
5. [Testing Area](#testing-area)
6. [Profile Format (JSON)](#profile-format-json)
7. [Demonstration](#demonstration)
8. [Contributing](#contributing)
9. [License](#license)

---

## Overview

Surf recreates the best parts of CustomCurve Pro and adds modern UX touches: interactive curve editing, independent horizontal/vertical tuning, profile management, sandboxed testing canvas, bias multipliers, and a responsive dark theme — all in a single-file Python/Tkinter app.

---

## Key Features

* Input DPI & in-game sensitivity with instant preview
* Interactive curve editor (horizontal + vertical): add, move, remove control points

  * Add point: double-click
  * Remove point: right-click a point
  * Move point: hold left mouse and drag
  * Zoom: mouse wheel
  * Pan: middle mouse button + drag
* Curve bias sliders for independent horizontal/vertical multipliers (0.1x — 3.0x)
* Profile system: save/load JSON profiles, rename, delete, import/export via file dialog
* Import `.ccurve` files and convert/apply them instantly
* Sandboxed test canvas — visual, real-time mouse movement simulation and gain readouts (no system changes)
* Modern dark theme with responsive scaling compatible with Windows 10/11

---

## Installation

1. Download the latest release from the [Releases page](https://github.com/awarzu/Surf/releases)
2. Extract the package
3. Run the executable file directly — no manual setup required

For developers who wish to build from source, clone the repository and run the Python script:

```bash
git clone https://github.com/awarzu/Surf.git
cd Surf
python surf.py
```

---

## Controls & Interactions (in-app)

* Add point — Double-click on graph
* Delete point — Right-click an existing point
* Drag point — Left-click + drag
* Zoom — Mouse wheel over the graph
* Pan — Middle mouse (wheel) + drag
* Bias sliders — Adjust horizontal/vertical sensitivity curve multipliers
* Profile management — Use the profile panel to create, rename, delete, import, export

---

## Testing Area

The built-in test canvas simulates mouse movement with current curve + DPI + sensitivity settings, showing:

* Current gain (live numeric readout)
* Trajectory preview
* Option to reset the simulated pointer

This is intentionally sandboxed — Surf does **not** modify system mouse settings.

---

## Profile Format (JSON)

Example of a saved profile (pretty-printed):

```json
{
  "name": "my_profile",
  "dpi": 800,
  "sensitivity": 2.0,
  "horizontal": {
    "bias": 1.0,
    "points": [[0.0, 0.0], [0.5, 0.6], [1.0, 1.0]]
  },
  "vertical": {
    "bias": 1.0,
    "points": [[0.0, 0.0], [1.0, 1.0]]
  }
}
```

---

## Demonstration

* Check the [Releases page](https://github.com/awarzu/Surf/releases) for usage notes and version highlights
* Read the feature breakdown above — it mirrors the actual workflow in the application
* User-shared profiles in Issues/Discussions can also serve as practical demonstrations

---

## Contributing

Since the repository currently contains only compiled releases, contributions can be made in the following ways:

* **Feedback** — Report bugs, unexpected behavior, or UI issues in the [Issues section](https://github.com/awarzu/Surf/issues)
* **Feature Requests** — Suggest improvements or new features via Issues
* **Profile Sharing** — Upload and share your custom profile configurations to help others
* **Testing** — Download releases, test across different systems, and report compatibility or performance issues

Pull requests with code changes are welcome once source files are available.

---

## License

This project is licensed under the terms provided in the [LICENSE](LICENSE) file.
