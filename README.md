# 🌌 Cosmic Bio Template







A stylish, space-themed personal bio page featuring a "Cloudflare-style" verification entrance, animated background particles, and a custom audio player.






![Project Status](https://img.shields.io/badge/Status-Active-blueviolet)



![License](https://img.shields.io/badge/License-MIT-fab)






## ✨ Features






* **🕵️ Verification Gate:** A fake "Verify you are human" screen (Cloudflare style) that transitions smoothly into the main profile.



* **🎨 Cosmic Theme:** Deep purple and neon magenta color palette with a glowing, pulsating avatar effect.



* **✨ Particle Effects:** Interactive background using `particles.js` with a custom space color scheme.



* **🎵 Custom Audio Player:**



    * Auto-looping background music.



    * Custom play/pause button and seek bar styled to match the theme.



    * Time progression display.



* **⌨️ Tab Title Animation:** Typewriter effect for the browser tab title.






## 🛠️ Installation & Usage






1.  **Clone the repository:**



    ```bash



    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)



    ```






2.  **Add your media:**



    * Place your profile picture in the root folder and name it `myavatar.png`.



    * Place your background music file in the root folder and name it `background.mp3`.






3.  **Edit `index.html`:**



    * Open `index.html` in any text editor.



    * Find the `<h1>` tag to change the username.



    * Update the `links` section with your own social media URLs (Telegram, Twitch, etc.).






## 🎨 Customization






### Changing Colors



The entire color scheme is defined in the `<style>` section of `index.html`.



* **Background:** Look for `body` and `#particles-js`.



* **Accent Colors:** Search for hex codes like `#c724b1` (Magenta) and `#6a00f4` (Deep Purple) to change the glowing effects.






### Music Player



To change the starting volume, find the `handleVerify()` function in the script:



```javascript



audio.volume = 0.3; // Change 0.3 to any value between 0.0 and 1.0
