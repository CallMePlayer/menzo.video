# Menzo Video

A music video film slate and audio loop tool that runs in the browser and installs as an app on your phone, tablet or computer. Load a song, loop a section by measures or frames, and slate each take with a clap sound, a timecode sync point and an automatic take counter.

Everything runs on the device. There is no server, no account and nothing is uploaded, and once installed it works fully offline.

## Features

- **Film slate**: production, scene and take fields on a clapperboard display, with the audio sync timecode.
- **CLAP & PLAY LOOP**: plays a clap sound and starts the loop. The slate records the loop's **In** and **Out** timecodes and frame numbers when you clap, so the audio can be lined up in the edit.
- **Automatic take counting**: the take number goes up each time the loop comes round again while the slate is running.
  - **Next take** adds one.
  - **Reset take to 1** sets it back to 1 at any time.
  - Slating a different scene (a different loop range or a different audio file) starts again at take 1 by itself.
- **Loop by Measures or Frames**: set the loop with BPM, beats per measure and a measure range, or with start and end frames at 24, 25, 29.97, 30 or 60 fps.
- **Scene markers**:
  - **Add measure range** saves a named scene from a measure range.
  - **Add at playhead** (or press `M`) drops a named marker at the current position.
  - **Loop this**, **Start** and **End** on a saved marker set the loop from it. They work in both Measures and Frames mode, and the marker's name goes onto the slate as the scene when you clap.
  - Markers are saved on the device, per audio file.
- **Fullscreen slate**: a large display for the set, sized to fit the screen with the buttons always visible. Press `Esc` to leave it.
- **Installable and offline**: works as a PWA on Android, iOS and desktop browsers.

## Quick start

1. Open the app and load an audio file with the file picker.
2. Set the BPM and beats per measure, or switch to Frames mode and choose a frame rate.
3. Choose the loop range, or tap **Loop this** on a saved scene marker.
4. Fill in the production and scene names (both start empty).
5. Press **CLAP & PLAY LOOP**. The take number increases each time the loop repeats.
6. Use **Next take** or **Reset take to 1** whenever you need to change the number by hand.

The audio file is not stored by the app. Pick it from your device at the start of each session. Your scene markers are remembered.

## Notes

- Keyboard shortcuts: `M` adds a marker at the playhead, `Esc` leaves fullscreen.
- Frame numbers from measure-based markers are rounded to the nearest whole frame, so they can be off by up to half a frame when a measure does not land exactly on a frame edge.
- Clearing the browser's site data removes your saved scene markers.