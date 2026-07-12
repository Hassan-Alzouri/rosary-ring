# Rosary Ring

A simple Flutter app that acts as a digital Tasbih (Islamic prayer bead counter), built to practice Flutter state management and custom UI design.

## Overview

The app displays a large circular counter with a Quranic verse in the app bar. Tapping the "+" button increments the count, and a reset button clears it back to zero — a digital stand-in for counting dhikr (remembrance) recitations traditionally tracked with physical prayer beads.

## Features

- ➕ **Tap-to-count** — large, easy-to-tap increment button
- 🔄 **Reset** — clears the counter back to zero
- 🎨 **Custom circular UI** — hand-built layered container design with shadows, built entirely with Flutter widgets (no external UI libraries)

## Tech Stack

| Layer | Technology |
|---|---|
| Framework | Flutter (Dart) |
| State management | Local widget state (`setState`) |

## Project Structure

```
Rosary-ring/
└── lib/
    └── main.dart   # App entry point and counter UI/logic
```

## Getting Started

### Prerequisites

- [Flutter SDK](https://docs.flutter.dev/get-started/install) (3.4+)

### Setup

```bash
git clone https://github.com/Hassan-Alzouri/rosary-ring.git
cd rosary-ring
flutter pub get
flutter run
```

## Status & Next Steps

This is a single-screen UI/state-management exercise — the count currently resets on app restart. A natural next step would be persisting the count locally (e.g. with `shared_preferences`) so it survives between sessions, plus support for multiple counters (e.g. different dhikr with different target counts).
