# Mein UNI-Tag – Study Guide App

A small mobile app for students, built with Flutter, that combines a weekly class schedule with a simple to-do style event list. It shows the current date and time, the student's profile, and the events for the selected weekday. The interface is in German and was designed around the TU Dresden timetable format.

<img src="https://github.com/TanyaBanina/StudyGuideApp/assets/115241739/53680427-b242-422d-b87c-2296b3a665e1" alt="Home screen" width="300">

## Features

- **Live clock** showing the current date and time, updated every second
- **Student profile card** with name, student ID, program, and semester (placeholder data)
- **Weekday selector** that automatically opens on today's day
- **Per-day schedule**: events are filtered by the selected weekday
- **Add events** through a dialog with title and description, with a warning if a field is left empty
- **Delete events** with a double tap
- **Navigation drawer** linking to the home, events, resources, and help pages

## How to run

Requires the [Flutter SDK](https://docs.flutter.dev/get-started/install).

```bash
git clone <repo-url>
cd study-guide-app
flutter pub get
flutter run
```

## Limitations and possible improvements

This was one of my first Flutter projects, built without a tutorial. Looking back, I would improve:

- **Persistence**: events are stored in memory only and reset when the app restarts (e.g. use local storage or SQLite)
- **State management**: state is passed between widgets manually; a state management approach (e.g. Provider) would scale better
- **Editable profile** instead of hard-coded student data

## Built with

- Flutter, Dart
- `intl` package for date formatting
