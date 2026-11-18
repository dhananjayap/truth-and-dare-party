# 🍾 Truth & Dare Party — Endless Edition

An electrifying, neon-party web app for playing Truth and Dare with friends, campus squads, and parties!

---

## 🌟 Key Features

1. **Manual Player Management**:
   - Add as many players as you want by typing their name and pressing **Enter** or clicking **Add Player**.
   - Each player gets a fun party emoji avatar and neon gradient badge.
   - Quick **"Add Party Squad"** preset button if you want to jump straight into the fun with sample names.
   - Remove, clear, or edit players on the fly.

2. **Smart Anti-Repetition Turn Cooldown**:
   - **Cooldown Rule**: Once a player completes a Truth or Dare (or takes a forfeit), they enter a cooldown state and **will not be picked again for 2 or 3 turns** (configurable in settings).
   - Visual status badges at the top of the screen:
     - 🟢 **READY**: Eligible to be picked in the next spin
     - ⏳ **Resting (2 turns left)** / ⏳ **Resting (1 turn left)**: Temporarily resting
     - 🎯 **CHOSEN**: Currently on the hot seat!
   - Dynamic safety algorithm automatically ensures that even with small groups (e.g. 2, 3, or 4 players), the game never deadlocks.

3. **Unpredictable Holographic Suspense Spotlight**:
   - **Zero Predictability**: Rather than pre-rendering names in a scrollable track, candidates are dynamically scrambled in real time with random jitter and variable spin durations.
   - **Heart-Stopping "Near-Miss Fake-Out"**: As speed slows down, the portal intentionally hesitates on a near-miss candidate with a deep bass heartbeat audio thump before snapping to the true winner with a golden shockwave, screen shake, and confetti explosion!

4. **Freedom of Choice**:
   - The selected player chooses:
     - 🔵 **TRUTH**: Confess secrets, campus stories, crush confessions, and awkward moments.
     - 🔴 **DARE**: Perform hilarious acting, savage roasts, accents, and wild party challenges (including legendary acts like *Nagavalli*, *Kunjikoonan*, and *Zoo Animal sounds*!).
     - 🎲 **RANDOM / SURPRISE ME**: Let fate decide whether it's a Truth or a Dare!

5. **290+ Unique, Curated Questions & Tasks**:
   - 🎓 **Campus & College Life (60 Truths + 60 Dares)**: Rich Kerala / Malayalam college culture (KSRTC bus rushes, parotta-beef treats, Mammootty vs Mohanlal debates, supply/arrears stories, viva panic, bunking, ente ammo drama!).
   - 💀 **Savage Roast Pack (60 Truths + 60 Dares)**: Unfiltered friend group roasts, screen-time confessions, fake life gurus, mock interviews, and WhatsApp group safari roasts.
   - 🔥 **Extreme Spicy & Wild Bonus (25 Truths + 25 Dares)**: Juicy crush confessions, late-night DMs, telenovela love confessions, intense staring contests, and spicy forfeits.
   - **No Repetition**: The app tracks used questions in a session so you never see the same challenge twice until the entire deck has been played.

6. **Interactive In-Game Tools**:
   - 🗣️ **Read Aloud**: Uses Text-to-Speech so the phone or laptop reads out the question aloud to the room.
   - ⏱️ **Countdown Timers**: Quick 30-second and 60-second timers with audio ticking and buzzer for timed challenges.
   - 🔀 **Reroll Task**: Swap to another challenge if the group agrees.
   - 🔄 **Switch Type**: Switch between Truth and Dare if the player changes their mind.
   - 🐔 **Chicken Out / Forfeit**: If a player refuses, they get a hilarious forfeit challenge (pushups, mystery snack, villain voice) before the game moves to the next player.

7. **Endless Party Loop & 🚪 Exit Door Button**:
   - Pressing **"✅ Task Completed! (Continue)"** triggers a victory fanfare, releases confetti, applies turn cooldown, and seamlessly picks the next player.
   - The game goes on endlessly with no limits.
   - Whenever you want to pause or quit, click the **"🚪 Exit Door"** button in the top right to:
     - Resume playing
     - View the **Party Recap & Superlatives** (Daring Champion, Truth Confessor, Chicken of the Night, and full scoreboard)
     - Return to the player setup lobby
     - Close the game

8. **Zero Dependencies & 100% Offline**:
   - Built with pure HTML5, CSS3, and JavaScript.
   - Built-in **Web Audio API synthesizer** provides all sound effects without requiring any external audio files or internet access.

---

9. **Mobile-Ready & 100% Offline PWA**:
   - **Progressive Web App (PWA)**: Includes `manifest.json` and a Service Worker (`sw.js`). You can tap "Install App" or "Add to Home Screen" on Android (Chrome) or iPhone (Safari).
   - **Physical Vibration / Haptic Feedback**: On mobile phones, every button click, roulette tick, heartbeat thud, and winner selection triggers realistic haptic vibration in your hand.
   - **Standalone Mobile Bundle (`truth-and-dare-mobile.html`)**: A single self-contained 148 KB file containing all styles, questions, sound synthesizers, and logic. You can send it directly to your phone via WhatsApp or email, tap to open, and play anywhere without internet or setup!

---

## 📱 How to Play on Mobile (Android & iPhone)

### Method 1: The 1-File Share (Easiest & Completely Offline)
Send [`truth-and-dare-mobile.html`](file:///C:/Users/Lenovo/.gemini/antigravity/scratch/truth-and-dare-party/truth-and-dare-mobile.html) to your phone via:
- WhatsApp / Telegram
- Email / Google Drive / Bluetooth
- Tap the file on your phone -> Choose **Open in Chrome** (Android) or **Safari** (iPhone).
- **Plays 100% offline** on any phone with full audio, haptic vibration, and animations!

### Method 2: Wi-Fi Hotspot Party Server
1. Double-click `play-on-mobile.bat` on your PC.
2. It displays your local Wi-Fi URL (e.g. `http://192.168.1.5:8080/index.html`).
3. Connect your phone to the same Wi-Fi or mobile hotspot and open that link in your browser.
4. Tap **"Install App"** or **"Add to Home Screen"** to save it as a native app icon!

---

## 🚀 How to Launch on PC

### Option 1: Double-Click
Double-click `start.bat` (or open `index.html` directly in Google Chrome, Microsoft Edge, Mozilla Firefox, or Safari).

### Option 2: Browser
Open `index.html` located at:
`C:\Users\Lenovo\.gemini\antigravity\scratch\truth-and-dare-party\index.html`

---

## 📁 Project Structure

```
truth-and-dare-party/
├── index.html                   # Main responsive UI with lobby, roulette, task cards & modals
├── truth-and-dare-mobile.html   # Standalone single-file mobile version (send via WhatsApp!)
├── style.css                    # Neon-dark party theme with glassmorphism & responsive layout
├── app.js                       # Game state machine, cooldown logic, roulette animation & timers
├── questions.js                 # 290+ curated Truths, Dares & Forfeits database
├── sound.js                     # Offline Web Audio API party sound effects synthesizer + haptics
├── manifest.json                # PWA app configuration (for "Install App" on phones)
├── sw.js                        # Offline Service Worker cache
├── play-on-mobile.bat           # 1-click local Wi-Fi server for phones
├── serve.ps1                    # PowerShell HTTP server script
├── start.bat                    # 1-click PC launcher
└── README.md                    # Documentation
```
