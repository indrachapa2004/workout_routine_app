# Project: Workout Routine App (mobile)

## Stack (do not deviate without asking)
- Expo (latest SDK) + Expo Router + TypeScript (strict)
- expo-sqlite + Drizzle ORM (local-first, no backend yet)
- Zustand for state
- NativeWind for styling
- expo-notifications, expo-audio, expo-haptics, expo-keep-awake
- Jest for unit tests

## Rules
- Timers MUST be timestamp-based: store an absolute endsAt timestamp and derive remaining time from Date.now(). Never count down with setInterval decrements.
- Every timer interval (work/rest) schedules a local notification so alerts fire when backgrounded; cancel it on pause/skip/stop.
- Keep timer logic in pure functions in /src/timer (no React imports) so it is unit-testable.
- Folder structure: /app (routes), /src/db, /src/features/{routines,workout,history}, /src/timer, /src/components, /src/store.
- No backend, auth, or analytics until told.
- Small, focused commits per task. Explain what changed after each task.
- Never add dependencies without listing them and why.
- Work only on the current phase. Stop and wait for review at the end of each phase.