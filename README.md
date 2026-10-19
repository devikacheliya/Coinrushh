
# Coin Rush

**Coin Rush** is a web-based game built using the **Godot Engine** Web Export template. It runs smoothly right inside your modern web browser via WebAssembly and HTML5 canvas.

---

## 🚀 Features

* **Browser-Based Gaming:** No installation or downloads required—play directly within your web browser.
* **Godot Engine Powered:** Built using optimized Godot HTML5 export configurations.
* **Responsive Layout:** Automatically scales the canvas to fit the viewport with touch-action handling support.
* **Loading & Error Management:** Includes an integrated loading progress bar, status splash screen, and built-in error/feature detection notices (such as missing cross-origin isolation or web feature checks).

---

## 🛠️ Technical Stack

* **Engine:** Godot Engine (Web Export)
* **Languages / Technologies:** HTML5, CSS3, JavaScript, WebAssembly (`.wasm`), and PCK resource packs (`.pck`).
* **Core Configuration:** 
  * Executable: `index`
  * WebAssembly Binary Size: $\approx 35.75 \text{ MB}$ (`index.wasm`)
  * Resource Pack Size: $\approx 45.37 \text{ KB}$ (`index.pck`)
  * Emscripten Memory Pool Size: $8$
  * Godot Pool Size: $4$

---

## 📁 Project Structure

```text
├── index.html              # Main HTML entry point & Godot engine bootstrapper
├── index.js                # Godot WebAssembly loader script
├── index.wasm              # Compiled engine WebAssembly binary
├── index.pck               # Game assets and project data pack
├── index.png               # Splash screen image
├── index.icon.png          # Favicon icon
└── index.apple-touch-icon.png  # Apple touch icon
```

---

## 🌐 Running Locally

Because modern web browsers enforce strict security policies regarding local file loading (`file://` protocol) for WebAssembly and module scripts, running this game locally requires a lightweight local development server.

1. Clone or download this repository into a local directory.
2. Spin up a local server using one of the following methods:
   * **Python:** 
     ```bash
     python3 -m http.server 8000
     ```
   * **Node.js (npx):** 
     ```bash
     npx serve
     ```
   * **PHP:** 
     ```bash
     php -S localhost:8000
     ```
3. Open your browser and navigate to `http://localhost:8000` (or the URL provided by your server tool).
