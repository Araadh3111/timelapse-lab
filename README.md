#Timelapse Lab

A fully browser-native timelapse recorder. Record from your webcam for any duration, then render it into a compressed timelapse video — no uploads, no backend, no installs.

---

## Features

- **Record for any duration** — seconds, minutes, or hours
- **Adjustable capture interval** — grab a frame every 100ms to every 5 seconds
- **Adjustable output FPS** — control how fast your timelapse plays back
- **Instant preview** — watch your timelapse right in the browser before downloading
- **Download as `.webm`** — save the output video to your machine
- **100% local** — nothing leaves your browser, ever

---

## How to Use

1. Open `timelapse.html` in any modern browser.
2. Allow camera access when prompted
3. Set your **Capture Interval** — how often a frame is grabbed
4. Set your **Output FPS** — playback speed of the final video
5. Hit **Start Recording** and let it run
6. Hit **Stop Recording** when done
7. Click **Generate Timelapse** and wait for it to render
8. Preview inline, then hit **Download**

---

## Speed Reference

| Record Duration | Capture Interval | Output FPS | Timelapse Duration | Speed Factor |
|---|---|---|---|---|
| 10 min | 500ms | 30 fps | ~40 sec | 15× |
| 1 hour | 2s | 30 fps | ~60 sec | 120× |
| 1 hour | 5s | 30 fps | ~24 sec | 150× |
| 8 hours | 10s | 30 fps | ~96 sec | 960× |

---

## Tech Stack

| Layer | Tech |
|---|---|
| Capture | `getUserMedia` Web API |
| Frame extraction | HTML5 `<canvas>` |
| Video encoding | `MediaRecorder` API |
| Output format | `.webm` (VP9 / VP8) |
| Dependencies | **None** — pure HTML/CSS/JS |

---



## 📁 Project Structure

```
timelapse-lab/
├── timelapse.html   
└── README.md
```

---

## Browser Compatibility

| Browser | Support |
|---|---|
| Chrome / Edge | ✅ Full |
| Firefox | ✅ Full |
| Safari | ⚠️ Partial (WebM may not play natively) |

---

## License

MIT — free to use, modify, and distribute.
