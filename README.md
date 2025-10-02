# SURF

> **A modern, polished reimplementation of CustomCurve Pro** — a Python Tkinter app for creating, editing, and testing custom mouse sensitivity curves. Designed for precision, performance, and a clean dark UI.

[![Release](https://img.shields.io/github/v/release/awarzu/Surf)](https://github.com/awarzu/Surf/releases)
[![License](https://img.shields.io/github/license/awarzu/Surf)](https://github.com/awarzu/Surf/blob/main/LICENSE)
[![Stars](https://img.shields.io/github/stars/awarzu/Surf?style=social)](https://github.com/awarzu/Surf/stargazers)

<p align="center">
  <img src="https://raw.githubusercontent.com/awarzu/Surf/main/icon.png" alt="Surf icon" width="160"/>
</p>

---

## Overview

Surf recreates the best parts of CustomCurve Pro and adds modern UX touches: interactive curve editing, independent horizontal/vertical tuning, profile management, sandboxed testing canvas, bias multipliers, and a responsive dark theme — all in a single-file Python/Tkinter app.

---

## Key Features

* Input DPI & in-game sensitivity with instant preview.
* Interactive curve editor (horizontal + vertical): add, move, remove control points.

  * Add point: double-click
  * Remove point: right-click a point
  * Move point: hold left mouse and drag
  * Zoom: mouse wheel
  * Pan: middle mouse button + drag
* Curve bias sliders for independent horizontal/vertical multipliers (0.1x — 3.0x).
* Profile system: save/load JSON profiles, rename, delete, import/export via file dialog.
* Import `.ccurve` files and convert/apply them instantly.
* Sandboxed test canvas — visual, real-time mouse movement simulation and gain readouts (no system changes).
* Modern dark theme with responsive scaling compatible with Windows 10/11.

---

## Installation

1. Download the latest release from the [Releases page](https://github.com/awarzu/Surf/releases).
2. Extract the package.
3. Run the executable file directly — no manual setup required.

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

If you would like to see how Surf works before downloading:

* Check the [Releases page](https://github.com/awarzu/Surf/releases) where usage notes and version highlights are included.
* Read the feature breakdown above — it mirrors the actual workflow in the application.
* User-shared profiles in Issues/Discussions can also serve as practical demonstrations of real setups.

---

## Contributing

Since the repository currently contains only compiled releases, contributions can be made in the following ways:

* **Feedback** — Report bugs, unexpected behavior, or UI issues in the [Issues section](https://github.com/awarzu/Surf/issues).
* **Feature Requests** — Suggest improvements or new features via Issues.
* **Profile Sharing** — Upload and share your custom profile configurations to help others.
* **Testing** — Download releases, test across different systems, and report compatibility or performance issues.

Pull requests with code changes are welcome once source files are available.

---

## Changelog & Releases

See the [Releases tab](https://github.com/awarzu/Surf/releases) on GitHub for packaged builds and release notes.

---

## License

Include your license file (e.g., MIT). If you want, I can add a standard `LICENSE` file content here.
