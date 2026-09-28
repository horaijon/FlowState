<div align="center">

  <img src="public/flowie-logo.png" alt="FlowState Mascot Logo" width="300" />

  # FlowState

  <p><strong>AI-Powered Ergonomic Focus & Posture Monitoring Workspace</strong></p>

  <p>
    <a href="https://react.dev/"><img src="https://img.shields.io/badge/React-18.3-61DAFB?style=flat-square&logo=react&logoColor=black" alt="React 18" /></a>
    <a href="https://vitejs.dev/"><img src="https://img.shields.io/badge/Vite-6.0-646CFF?style=flat-square&logo=vite&logoColor=white" alt="Vite" /></a>
    <a href="https://tailwindcss.com/"><img src="https://img.shields.io/badge/Tailwind_CSS-3.4-38BDF8?style=flat-square&logo=tailwind-css&logoColor=white" alt="Tailwind CSS" /></a>
    <a href="https://ai.google.dev/edge/mediapipe/solutions/vision/pose_landmarker"><img src="https://img.shields.io/badge/MediaPipe-Vision_AI-00A896?style=flat-square&logo=google&logoColor=white" alt="MediaPipe Vision" /></a>
    <a href="https://flow-state-hzlm.vercel.app/"><img src="https://img.shields.io/badge/🚀_Live_Demo-Vercel-000000?style=flat-square&logo=vercel&logoColor=white" alt="Live Demo" /></a>
  </p>

  <h3>🔗 <a href="https://flow-state-hzlm.vercel.app/">Try FlowState Live →</a></h3>

  <p>
    <a href="#-key-features">Key Features</a> •
    <a href="#-tech-stack">Tech Stack</a> •
    <a href="#-getting-started">Getting Started</a> •
    <a href="#-project-structure">Project Structure</a>
  </p>

</div>

---

## 🌟 Overview

**FlowState** is a web-based, AI-assisted productivity workspace designed to keep you focused, hydrated, and ergonomically aligned during deep work sessions. Using real-time computer vision right inside your browser, FlowState continuously monitors posture alignment, alerts you to slouching, evaluates screen distance and room lighting, and tracks daily focus streaks.

All camera processing is computed **100% locally on your device** via MediaPipe landmark tracking—no video feed is ever transmitted or recorded.

---

## ✨ Key Features

### Real-Time Computer Vision Engine
- **Posture Score & Slouch Detection**: Calculates body alignment using MediaPipe pose landmarks and triggers alerts when slouching is detected.
- **Screen Distance Monitoring**: Warns when you lean too close to prevent eye strain.
- **Ambient Lighting Analysis**: Evaluates room lighting conditions for optimal focus environments.

### Interactive AI Companion ("Flowie")
- **Dynamic Mascot**: Features animated shader mesh graphics that react to your focus state.
- **Contextual States**: Automatically transitions between *Asleep* (idle), *Active* (focused), and *Alert* (slouching detected).

### Analytics & LeetCode-Style Activity Heatmap
- **Month-Grouped Focus Graph**: Displays daily focus activity grouped by month with zero text truncation and distinct month separators.
- **Brand Theme Integration**: Adaptive color intensity matching the signature Solarized magenta/pink theme across light and dark modes.
- **Streak & Hydration Counters**: Tracks consecutive focus days and logs in-session water intake goals.

### Solarized Theme System
- **Light & Dark Mode**: Instant toggling powered by CSS custom properties and high-contrast color tokens.

---

## Tech Stack

| Component | Technology |
| :--- | :--- |
| **Frontend Framework** | [React 18](https://react.dev/) + [Vite](https://vitejs.dev/) |
| **Styling** | [Tailwind CSS v3](https://tailwindcss.com/) |
| **Vision AI Engine** | [Google MediaPipe Pose Landmarker](https://ai.google.dev/edge/mediapipe/solutions/vision/pose_landmarker) |
| **Animations & Shaders** | [Framer Motion](https://www.framer.com/motion/) + `@paper-design/shaders-react` |
| **Icons** | [Lucide React](https://lucide.dev/) |

---

## 🚀 Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) (v18.0.0 or higher)
- `npm` or `pnpm` / `yarn`

### Installation & Run

```bash
# 1. Clone the repository
git clone https://github.com/Karanpreet-Singh07/FlowState.git

# 2. Navigate to project directory
cd FlowState

# 3. Install dependencies
npm install

# 4. Start local development server
npm run dev
```

Open your browser at `http://localhost:5173` to launch the workspace.

---

## 📁 Project Structure

```text
FlowState/
├── public/
│   └── flowie-logo.png        # Halo-free mascot brand logo
├── src/
│   ├── components/
│   │   ├── ui/
│   │   │   ├── FlowieLogo.jsx # Reusable logo mark & two-tone text branding
│   │   │   └── shader-svg.jsx # Flowie mascot animated mesh shader
│   │   ├── AnalyticsDashboard.jsx # Analytics page & summary statistics
│   │   ├── Dashboard.jsx      # Main live workspace & camera feed
│   │   ├── Login.jsx          # User sign-in & guest entry
│   │   ├── SessionHeatmap.jsx # Month-grouped contribution activity graph
│   │   ├── SessionHistoryDrawer.jsx # Slide-out navigation & history log
│   │   └── VisionEngine.jsx   # MediaPipe computer vision detection engine
│   ├── utils/
│   │   └── storage.js         # LocalStorage persistence & streak logic
│   ├── App.jsx                # Root app state & theme controller
│   ├── main.jsx               # Entry point
│   └── index.css              # Solarized theme variables & CSS directives
├── tailwind.config.js
├── vite.config.js
└── README.md
```

---

<div align="center">
  <sub>Built for focused, healthy, and ergonomic deep work.</sub>
</div>
