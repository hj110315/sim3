# 🌿 Aura Planner (아우라 플래너)

> A calm, glassmorphic time-management web app built for college students to take proactive control of their academics, form positive habits, and manage deadlines without burnout.

---

## ✨ Features Implemented

* **🌅 Dynamic Hero Landing:** Random HD nature wallpapers and inspirational quotes fetched via API with offline fallback support. Includes the signature **"공부 시작하자!^^"** transition trigger.
* **✨ Glass-Curtain Transition:** Clicking the start trigger activates a smooth backdrop-blur scaling curtain over the nature visual to open your workspace cleanly.
* **🏛️ Central Lobby Command Center:**
  * **Today's Top 3 Focus:** Instant-save inputs for your non-negotiable daily priorities.
  * **Habit & Rest Tracker:** Interactive checklist for reading, non-academic goals, and guilt-free rest.
  * **Deadline Radar:** Visual D-Day status cards for exams and major assignments.
* **💾 Zero-Backend Data Persistence:** Uses a custom `useLocalStorage` React hook to automatically save all priorities, habit checks, and deadlines directly inside your browser memory.

---

## 🛠️ Tech Stack

* **Framework:** React (Vite)
* **Styling:** Tailwind CSS (Custom Glassmorphism Utilities)
* **Icons:** Lucide React (`lucide-react`)
* **Storage:** Browser `localStorage` (No server or database required)

---

## 📂 Project Structure

```text
aura-planner/
├── public/
│   └── .nojekyll             # Prevents GitHub Pages from running Jekyll fallback
├── src/
│   ├── components/
│   │   ├── HeroLanding.jsx   # Nature backdrop, dynamic quotes, start button
│   │   └── CentralLobby.jsx  # Top 3 focus, habit checklist, deadline radar
│   ├── hooks/
│   │   └── useLocalStorage.js # Custom React persistent state hook
│   ├── App.jsx               # Main view router & glass curtain effect
│   ├── index.css             # Tailwind CSS & glassmorphic utility rules
│   └── main.jsx              # React DOM entry
├── index.html                # Single-page HTML root
├── vite.config.js            # Vite build setup with GitHub base path
├── postcss.config.js         # PostCSS configuration
├── tailwind.config.js        # Tailwind theme extension
└── package.json
