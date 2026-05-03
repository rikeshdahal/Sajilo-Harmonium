# 🎹 Sajilo Harmonium

> **A free, open-source web harmonium with real reed sound — play, learn, and compose right from your browser.**

**🌐 Live Demo → [rikeshdahal.github.io/Sajilo-Harmonium](https://rikeshdahal.github.io/Sajilo-Harmonium/)**

---

![Sajilo Harmonium Screenshot](https://rikeshdahal.github.io/Sajilo-Harmonium/preview.png)

---

## ✨ Features

### 🎹 Play
- Full **23-key harmonium keyboard** rendered in SVG
- Real harmonium reed audio sample (not synthesized MIDI)
- Play with **mouse, touch, or computer keyboard**
- **Octave shift** (Shift + ↑ / ↓) and **Transpose** controls
- **Reverb** toggle for room acoustics
- **Sa drone** — continuous tonic note for raga practice
- Indian swaram labels (S R G M P D N Ṡ) on every key

### 🎵 Songs
- **5 built-in songs** — Twinkle Twinkle, Sa Re Ga Ma, Yaman, Bhairav, Jai Ho
- **Auto-play** with golden key glow and chip highlight
- **Tempo control** (40–200 BPM)
- Import / Export songs as **JSON**
- Save unlimited custom songs in browser

### 📖 Learn Mode
- **Step-by-step guided learning** — one note at a time
- Green glow = correct key · Red flash = wrong key
- **Score tracker** — Correct / Wrong / Accuracy %
- Full song note chips with progress bar
- Works with any built-in or imported song

### ✍️ Compose
- Click-to-add note grid with **swara + key labels**
- Choose duration: ⅛ · Quarter · Half · Whole · Bar
- Live preview playback
- **Auto-saves draft** to browser
- Export composed song as JSON to share or reimport

### ⚙️ Settings
- Volume · Reverb · Sa Drone
- Keyboard shortcut reference
- Clean brass-themed UI

---

## 🎼 Keyboard Shortcuts

| Keys | Action |
|------|--------|
| `` ` q w e r t y u i o p [ ] \ `` | White keys (G A B C D E F G A B C D E F) |
| `1 2 4 5 7 8 9 - = '` | Black keys (komal / tivra swaras) |
| `Shift + ↑` | Octave up |
| `Shift + ↓` | Octave down |
| `Escape` | Stop playback |

**Default Sa = C (key `e`)**

| Swara | Key | Note |
|-------|-----|------|
| S (Sa) | `e` | C |
| R (Re) | `r` | D |
| G (Ga) | `t` | E |
| M (Ma) | `y` | F |
| P (Pa) | `u` | G |
| D (Dha) | `i` | A |
| N (Ni) | `o` | B |
| Ṡ (Taar Sa) | `p` | C' |

---

## 📦 Song JSON Format

You can write your own songs and import them into Sajilo Harmonium.

```json
{
  "name": "My Song",
  "notes": [
    { "k": "e", "n": "C", "s": "S" },
    { "k": "r", "n": "D", "s": "R" },
    "bar",
    { "k": "t", "n": "E", "s": "G" }
  ],
  "durs": [1, 2, 0, 1]
}
```

| Field | Description |
|-------|-------------|
| `k` | Keyboard key to press |
| `n` | Note name (C, D, E…) |
| `s` | Indian swaram (S, R, G…) |
| `"bar"` | Bar separator (use `0` in durs) |
| `durs` | Duration in beats — `1` = quarter, `2` = half, `4` = whole, `0` = bar |

---

## 🚀 Getting Started

### Use Online
Just visit → **[rikeshdahal.github.io/Sajilo-Harmonium](https://rikeshdahal.github.io/Sajilo-Harmonium/)**

No installation. No signup. Works on desktop and mobile.

### Run Locally

```bash
git clone https://github.com/rikeshdahal/Sajilo-Harmonium.git
cd Sajilo-Harmonium
```

Then open `harmonium.html` in your browser — OR serve it with any static server:

```bash
# Python
python -m http.server 8080

# Node.js
npx serve .
```

> ⚠️ The audio sample must be served over HTTP/HTTPS (not `file://`) due to browser security. Use the local server method above.

### Files Required

```
Sajilo-Harmonium/
├── harmonium.html              ← Main app
├── harmonium-kannan-orig.wav   ← Real reed audio sample
└── reverb.wav                  ← Optional reverb impulse
```

---

## 🛠️ Built With

- **Vanilla HTML / CSS / JavaScript** — zero frameworks, zero dependencies
- **Web Audio API** — real-time audio engine with pitch shifting
- **SVG** — scalable keyboard rendering
- **localStorage** — song persistence in browser

---

## 🤝 Contributing

Contributions are welcome! Here are some ideas:

- 🎵 Add more built-in songs (JSON format, easy to add)
- 🌏 Add more language support for swaram labels
- 🎛️ Pitch bend / vibrato effects
- 📱 Improve mobile touch experience
- 🔊 Additional instrument samples

### How to Contribute

```bash
# Fork the repo, then:
git clone https://github.com/YOUR_USERNAME/Sajilo-Harmonium.git
cd Sajilo-Harmonium

# Make your changes
# Submit a Pull Request
```

---

## 📄 License

This project is open source under the **MIT License** — free to use, modify, and distribute.

See [LICENSE](LICENSE) for full details.

---

## 👤 Author

**Rikesh Dahal**

- 🌐 Website: [rikeshdahal.com.np](https://rikeshdahal.com.np)
- 🐙 GitHub: [@rikeshdahal](https://github.com/rikeshdahal)

---

## ⭐ Support

If you find this project useful, please consider giving it a **star** on GitHub — it helps others discover it!

[![GitHub stars](https://img.shields.io/github/stars/rikeshdahal/Sajilo-Harmonium?style=social)](https://github.com/rikeshdahal/Sajilo-Harmonium/stargazers)

---

*Sajilo (सजिलो) means "Easy" in Nepali — making harmonium accessible to everyone.* 🇳🇵
