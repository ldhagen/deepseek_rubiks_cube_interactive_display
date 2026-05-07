```markdown
# 🧩 Interactive 3D Rubik’s Cube

A fully interactive, locally hosted Rubik’s Cube built with Three.js and vanilla JavaScript. Rotate the camera, make moves with buttons, scramble, and solve by undoing your move history.

![Interactive display screenshot](https://raw.githubusercontent.com/ldhagen/deepseek_rubiks_cube_interactive_display/refs/heads/main/screenshot.png)

## ✨ Features

- **Fully 3D** – Realistic colors, lighting, and smooth animations
- **Complete move set** – All face turns (U, D, L, R, F, B) and slice moves (M, E, S)
- **Keyboard‑free controls** – Use on‑screen buttons for all moves
- **Scramble** – Randomizes the cube with 45–80 random moves
- **Solve** – Reverses your entire move history (undoes everything you did) – 100% reliable
- **Reset** – Returns the cube to solved state instantly
- **Camera control** – Drag to rotate view, scroll to zoom
- **Move counter** – Tracks total moves performed
- **Responsive UI** – Works on desktop and mobile devices

## 🖱️ Controls

| Action                    | How to do it                     |
|---------------------------|----------------------------------|
| Rotate camera             | Drag mouse / finger              |
| Zoom                      | Scroll / pinch                   |
| Turn a face               | Click U, D, L, R, F, B buttons   |
| Turn in opposite direction| Click U', D', etc.               |
| Slice moves (M, E, S)     | Click M, M', E, E', S, S' buttons|
| Randomize cube            | Click **SCRAMBLE**               |
| Solve cube                | Click **SOLVE** (undoes all moves)|
| Reset to solved           | Click **RESET**                  |

> **Note:** The cube is controlled entirely by buttons. Clicking directly on the 3D model does nothing (prevents accidental moves).

## 🚀 How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/rubiks-cube.git
   cd rubiks-cube
   ```

2. **Open the HTML file**
   - Simply double-click `index.html` in your file explorer, or
   - Serve with any local web server (e.g., `npx serve .` or `python -m http.server`)

3. **Play** – Use the buttons at the bottom of the screen.

## 🧠 How the Solver Works

This cube does **not** use complex solving algorithms. Instead, it **records every move you make** (including slice moves) and then **reverses the sequence** when you click SOLVE. This guarantees a correct solution regardless of how scrambled the cube is.

- Move history is stored in an array.
- SOLVE generates the inverse of each move in reverse order.
- The cube animates through the solution step by step.

## 🔮 Future Roadmap

- **API integration** – Send the scrambled cube state to an external solving engine (e.g., Kociemba solver) and execute optimal solutions.
- **Speedcubing timer** – Track solving time.
- **Custom colors** – Allow users to change face colors.
- **Keyboard shortcuts** – For advanced users.

## 🛠️ Technology Stack

- [Three.js](https://threejs.org/) – 3D rendering and animations
- [OrbitControls](https://threejs.org/examples/#misc_controls_orbit) – Camera rotation & zoom
- HTML5 / CSS3 – Responsive UI
- Vanilla JavaScript – No external dependencies beyond Three.js

## 📁 Project Structure

```
rubiks-cube/
├── index.html          # Complete application (HTML, CSS, JS)
├── README.md           # This file
└── screenshot.png      # Screenshot of the application
```

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

## 📄 License

[MIT](https://choosealicense.com/licenses/mit/) – feel free to use, modify, and distribute.

## 🙏 Acknowledgements

- Three.js community for the excellent 3D library
- Rubik’s Cube color scheme is standard
- Inspired by classic cube simulators

---

**Enjoy solving – or just scrambling!** 🎲
```
