# Irotokazoo — Color & Number Zoo

A kid‑friendly, bilingual (Japanese/English) web game for learning **colors** and **numbers** through fast, joyful quizzes. Runs entirely in the browser as a single HTML file—no build tools or servers required.

## ✨ Features

* **Two topics**

  * **Colors**: identify a color by name or by swatch
  * **Numbers**: read Arabic numerals as words
* **Bilingual UI**: toggle between **English** and **Japanese (hiragana)** at any time
* **Game styles**

  * **Time Attack**: answer as many as you can in 30/60/90s
  * **Question Count**: aim for accuracy across 5/10/20 questions
* **Color modes**

  * **Easy** (answers shown in their color)
  * **Hard** (answers in black text)
  * **Word + Color** (word is black; choose from **color‑only buttons**, no text)
* **Number levels**

  * Level 1: **0–10**
  * Level 2: **0–20**
  * Level 3: **0–20 + specials** (hundred/thousand/**million**, **billion**; Japanese **まん**, **おく**)
* **Kid‑friendly feedback**

  * Bright **correct chime**, bold **wrong buzzer** (with gentle vibration on supported devices)
  * Per‑question visual **border “flash”** (no distracting sparkles)
  * **Result screen logic**:

    * **100%** → fireworks + celebratory fanfare
    * **≤ 50%** → sad fanfare, no confetti/fireworks
    * **in‑between** → confetti + happy fanfare
  * Shows **score**, **best streak**, and **correct/total**
* **Quality of life**

  * Remembers preferences via **localStorage**
  * Works fully **offline** (static HTML, CSS, JS only)

> 🪄 Hidden fun: tap the title **5 times** to toggle a playful “kazoo‑style” fanfare.

## 🧩 How to Play

1. Open `index.html` in any modern browser.
2. Choose **Language**, **Topic**, and the game options you like.
3. Press **Start**.
4. In **Colors**, pick the correct color name or color swatch. In **Numbers**, pick the correct word (e.g., “one”, “いち”).
5. Check results at the end—fireworks if you aced it!

## 🚀 Run Locally

No install needed.

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
# Just open index.html in your browser (double‑click or drag‑drop)
```

## 📷 Screenshots (optional)

Add images like:

```md
![Start screen](docs/screenshot-start.png)
![Color quiz](docs/screenshot-color.png)
![Results](docs/screenshot-result.png)
```

## 💡 Design & Accessibility Notes

* **Readable contrasts**: text color adapts to background luminance.
* **Color‑only answers** include **ARIA labels** for screen readers.
* **Vibration feedback** on wrong answers (where supported).
* **Hiragana** for Japanese to be kinder to early readers.

## 🛠 Tech Stack

* **Vanilla HTML/CSS/JavaScript**
* **Web Audio API** for sounds
* **Canvas** for fireworks animation
* No frameworks, no bundlers

## 📁 Project Structure

```
index.html        # All UI, styles, logic, and assets in one file
```

## 🔧 Customization

* **Colors/labels**: edit the `COLORS` list.
* **Special numbers**: tweak `NUM_SPECIAL_JA` / `NUM_SPECIAL_EN`.
* **Sounds**: adjust synth envelopes in `successChime()`, `wrongBuzz()`, and fanfares.
* **Result effects**: change thresholds/animations in `endGame()`.

## ✅ Browser Support

Latest Chrome, Edge, Safari, and Firefox. Mobile Safari/Chrome work too (tap once to enable sound due to browser policies).

## 🤝 Contributing

PRs welcome! For code changes:

1. Keep the game **accessible** and **kid‑friendly**.
2. Prefer small, readable functions and no dependencies.
3. Test both languages and all game modes.

## 📜 License

MIT © You — feel free to use, modify, and share.

---
