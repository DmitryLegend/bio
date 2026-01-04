# 🌌 Cosmic Bio Template (DmitryLegend Edition)

A stylish, space-themed personal bio page featuring a "Cloudflare-style" verification entrance, animated background particles, and a custom audio player with synchronized video logic.

![Project Status](https://img.shields.io/badge/Status-Active-blueviolet)
![License](https://img.shields.io/badge/License-MIT-fab)

---

## ✨ Features

* **🕵️ Verification Gate:** A fake "Verify you are human" screen that transitions smoothly. While verifying, the background video loops the first 4 seconds.
* **🎥 Smart Video Background:** High-quality MP4 background that "unfreezes" and continues playing from the 4th second once verified.
* **🎭 Cascade Animations:** * The main block appears with a **Scale & Fade** effect.
    * Social buttons (Telegram & Google) fade in smoothly right after the main block appears.
* **🎨 Purple Neon Aesthetic:** Deep dark theme with a subtle, synchronized purple pulse effect on all borders.
* **🎵 Custom Audio Player:**
    * Synchronized purple progress dot and arc seeker.
    * Auto-looping background music with time display.
* **⌨️ Fixed Tab Title Animation:** Perfect typewriter effect for the browser tab title that never misses a letter.
* **⏳ Auto-Maintenance:** The page automatically reloads every 9 minutes to keep the session and video fresh.

---

## 🔗 Status & Contact

| Status | Personal Link |
| :--- | :--- |
| **Active** | [**Contact via Telegram**](https://t.me/DmitryLegend) |

---

## 🛠️ Installation & Usage

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/DmitryLegend/bio.git](https://github.com/DmitryLegend/bio.git)
    ```

2.  **Add your media:**
    * Profile picture: `image.png`
    * Background video: `videoplayback.mp4`
    * Background music: `ambient-space-arpeggio-350710.mp3`

3.  **Edit `index.html`:**
    * Change the `<h1>` tag for your username.
    * Update the social links in the `.social-links` div.

---

## 🎨 Customization

### Changing Animations
The appearance effects are defined in the `<style>` section:
* **Main Block:** Look for `@keyframes blockAppear`.
* **Buttons:** Look for `@keyframes buttonsFadeIn`.

### Music & Video Logic
To change the starting volume or video sync, check the `handleVerify()` function in the script:
```javascript
audio.volume = 0.5; // Change 0.5 to any value between 0.0 and 1.0
video.currentTime = 4; // The second where video continues after verification
