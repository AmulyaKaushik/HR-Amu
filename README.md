# HR Analytics Assignment Drill · NPTEL IIT Roorkee

An interactive, high-performance web application designed for students and professionals preparing for the **NPTEL HR Analytics** certification exam (IIT Roorkee).

Includes all **120 assignment questions across Weeks 1 to 12**, with instant feedback, examination discrepancy notes, progress persistence, smart navigation, and full offline PWA support.

---

## 🚀 Live Demo & Deployment

This project is built as a zero-dependency, static progressive web app (PWA). It can be deployed in seconds to any static web host.

### Option 1: Vercel (Recommended)
1. Push this directory to a GitHub repository or run in terminal:
   ```bash
   npx vercel
   ```
2. Vercel automatically detects `index.html` and uses `vercel.json` for security headers and cache optimization.

### Option 2: Netlify
- Drag and drop this folder into [Netlify Drop](https://app.netlify.com/drop), or connect your Git repository.
- Build settings are preconfigured in `netlify.toml`.

### Option 3: GitHub Pages
1. Push to your GitHub repository.
2. Go to **Settings** > **Pages**.
3. Under **Build and deployment**, select **Source: Deploy from a branch**.
4. Choose `main` (or `master`) branch and `/ (root)` folder, then click **Save**.

### Option 4: Local Offline Run
Simply double-click `index.html` in your file explorer to open it in any modern browser, or run:
```bash
npx serve .
```

---

## 🌟 Key Features

- **120 Verified Questions**: 10 questions per week covering Weeks 1 through 12.
- **Official NPTEL Clarifications**:
  - **Week 11 Q9**: Compa Ratio formula note explaining `Pay / Range Midpoint` vs the NPTEL sheet error.
  - **Week 4 Q8**: Structured vs Behavioural interview definition explanation.
- **Interactive Mastery Dashboard**:
  - SVG circular gauge showing overall mastery percentage.
  - Real-time counters for Attempted, Correct, Accuracy %, and Starred items.
- **Smart Navigation**:
  - `Next Unanswered` automatically locates and scrolls to the next incomplete question.
  - Floating action button (FAB) for mobile quick-jumping.
- **Dynamic Filters & Search**:
  - **Filter Chips**: All, Unanswered Only, Mistakes to Review, Starred (⭐).
  - **Week Carousel**: Filter by Week 1 to 12, with visual indicators when a week is 100% mastered.
  - **Instant Search**: Type keywords like *BARS*, *Compa Ratio*, *Tableau*, *Yield ratio*.
- **Question & Options Shuffling**:
  - Deterministic pseudo-random number generator (PRNG) shuffles questions or option choices while preserving answers and state.
- **PWA & Offline Capability**:
  - Progressive Web App with `manifest.webmanifest` and Service Worker (`sw.js`).
  - Installable to iOS home screen or Android as a native standalone app.
  - Works 100% offline without requiring internet.
- **Audio Feedback**:
  - Pleasant ascending chime on correct answers and soft feedback on incorrect answers using pure Web Audio API (zero audio file downloads).
- **Keyboard Shortcuts**:
  - `1`, `2`, `3`, `4`: Select option A, B, C, D on active card.
  - `N` or `J`: Jump to next unanswered question.
  - `P` or `K`: Previous question.
  - `S`: Star / Bookmark question.
  - `/`: Focus search bar.
  - `Esc`: Clear search / close modal.
  - `?`: View shortcuts dialog.
- **Themes**:
  - Built-in Dark and Light themes with smooth transitions and persistent preference.

---

## 📁 Project Structure

```
├── index.html                     # Primary entry point (PWA & responsive UI)
├── HR Analytics Assignment Drill.html  # Synchronized standalone copy
├── manifest.webmanifest           # Progressive Web App manifest
├── sw.js                          # Service Worker for offline asset caching
├── favicon.svg                    # Scalable SVG favicon
├── icon-192.png                   # PWA icon 192x192
├── icon-512.png                   # PWA icon 512x512
├── apple-touch-icon.png           # iOS home screen icon
├── vercel.json                    # Vercel deployment configuration
├── netlify.toml                   # Netlify deployment configuration
├── .gitignore                     # Git ignore rules
└── README.md                      # Documentation & deployment guide
```

---

## 🛡️ License & Acknowledgements

Created for educational purposes supporting candidates of the NPTEL HR Analytics course by IIT Roorkee. Questions belong to the respective NPTEL course creators.
