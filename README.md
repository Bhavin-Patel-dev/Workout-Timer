## Introduction

Workout Timer is a **demo learning project** built with React to explore concepts like state management with hooks, derived/calculated state, memoization, side effects, and modular component design. The app allows users to select a workout type, adjust parameters (sets, speed per exercise, break length), and instantly see the calculated total workout duration.

It also includes a real-time clock display and an optional sound effect that plays when parameters change. This project is designed for beginners learning React fundamentals while building something interactive and visually appealing.

## 🌟Features

- **Workout Selection** — Choose from predefined workout types with varying numbers of exercises.

- **Dynamic Parameter Control** — Adjust:

  - Number of sets (1–5)
  - Speed per exercise (30–180 sec)
  - Break duration (1–10 min)

- **Real-Time Calculation** — Updates total workout duration automatically as inputs change.

- **Sound Toggle** — Mute or unmute click sound effects with a single button.

- **Live Clock** — Displays current date and time, updated every second.

- **Memoization Optimization** — Uses `useMemo` to avoid unnecessary recalculations.

## 🛠️ Tech Stack

- **React** (Functional Components + Hooks)

  - `useState`, `useEffect`, `useMemo`

- **CSS** for styling

- **JavaScript ES6+** features

- **Audio API** for sound playback

## 📁 Project Structure

```
/src
  ├─ App.js           # Main app component with clock, workout list, sound toggle
  ├─ Calculator.js    # Calculator component for duration logic and input controls
  ├─ ToggleSounds.js  # Button to toggle sound effects on/off
  ├─ ClickSound.m4a   # Audio file for click sound effect
  ├─ index.js         # App entry point
  ├─ index.css        # Styling for layout and components
```

## 🚀 Installation & Run

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Bhavin-Patel-dev/Workout-Timer.git
   cd Workout-Timer
   ```
2. **Install dependencies**:
   ```bash
   npm install
   ```
3. **Run the app**:
   ```bash
   npm start
   ```
4. Open `http://localhost:3000` in your browser.

## 🎮 How It Works

1. **Clock**: `useEffect` sets up an interval to update the current time every second.

2. **Workout List**: Uses `useMemo` to define workout options dynamically based on AM/PM.

3. **Duration Calculation**: Automatically recalculates total workout time whenever inputs change.

4. **Sound Effects**: Plays an audio clip when duration changes, unless muted.

5. **Increment/Decrement**: Plus and minus buttons allow manual adjustment of total time.

## 🎯 Learning Objective

- Managing multiple pieces of state with `useState`.

- Running side effects with `useEffect` (intervals, audio playback).

- Using `useMemo` for performance optimization.

- Passing props between components for interactivity.

- Styling and layout creation in CSS for a professional look.

- Integrating media assets (audio) in React.

## 🤝 Contributions

Contributions are welcome!

1. Fork the repository.
2. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit changes and push:
   ```bash
   git push origin feature/your-feature-name
   ```
4. Open a Pull Request describing your changes.
