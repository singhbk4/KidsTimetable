# KidsTimetable

A single-file, browser-based **Kids Task Dashboard** that gamifies daily chores and routines for children using a superhero theme. No server, no framework — just open `index.html` in any browser.

---

## Features

### Dynamic Multi-Kid Support
- On first launch, prompts for the number of kids (1–8) and their names.
- Each kid gets their own card, colour theme, superhero identity, and progress tracking.
- All data is stored in `localStorage` — no account or internet required.

### Superhero Selection
- Each kid picks a superhero from a full roster (Iron Man, Thor, Batman, Wonder Woman, and more).
- Superhero can be changed at any time via the **Change Superhero** button.

### Daily Tasks
- 10 pre-defined daily tasks (brushing teeth, homework, reading, etc.).
- Each task can be marked **Yes (+1 pt)** or **No (−1 pt)**.
- Net task points are shown per kid.

### Extra Perks
- Bonus tasks (e.g. Garage Cleanup, Learn New Vocabulary) that award +1 perk each.
- Perk value is configurable in Settings (default: **$0.20 AUD** per perk).

### Penalties
- Negative behaviours (e.g. screen time abuse, arguing) deduct points.
- Penalty value is configurable in Settings (default: **$0.10 AUD** per penalty).

### AUD Earnings
- Points are converted to Australian Dollars using **separate, configurable rates**:
	- **Daily Tasks**: configurable points per $1 AUD (default: 10 pts = $1.00)
	- **Extra Perks**: configurable cents per perk (default: 20¢)
	- **Penalties**: configurable cents per penalty (default: 10¢)
- AUD totals are shown on each kid's card and in the header.

### Achievements & Badges
- Unlockable badges for milestones: first task, 7-day streak, 30-day streak, 100 pts, 500 pts, perfect day, and extra achiever.
- Locked badges are shown greyed out as motivation.

### Monthly Calendar
- Visual calendar showing daily completion status for the current month.
- Monthly points total displayed per kid.

### History View
- **Day view**: select any date to see task, perk, and penalty breakdown per kid with AUD values.
- **Month view**: table showing monthly points and earnings per kid with a combined total.

### Settings Panel
- ⚙️ Accessible via the fixed settings button (top-right corner).
- Options:
	- 🌙 Dark Mode toggle
	- 📋 Daily Task points per $1 AUD
	- ✨ Extra Perk value (cents per perk)
	- ⚠️ Penalty deduction (cents per penalty)
	- 🎨 Per-kid colour customisation
	- 📥 Export all data as JSON backup
	- 🗑️ Clear all data

### Dark Mode
- Full dark theme toggled from Settings, persisted across sessions.

---

## Getting Started

1. Download or clone this repository.
2. Open `index.html` in any modern browser (Chrome, Edge, Firefox, Safari).
3. Enter the number of kids and their names when prompted.
4. Each kid selects their superhero.
5. Start tracking daily tasks!

---

## Data Storage

All data is stored in the browser's `localStorage`. Nothing is sent to any server. To back up data, use **Export Data as JSON** in Settings.

---

## Version History

| Version | Notes |
|---------|-------|
| v0.1 | Initial release — two hardcoded kids (Advik & Viaan), basic task tracking |
| v0.2 | Fully dynamic multi-kid architecture, separate AUD rates for tasks/perks/penalties, achievements, dark mode, settings panel |