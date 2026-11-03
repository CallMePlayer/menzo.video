# Menzo Video

A browser-based **film slate for music videos**. Point a camera at the board, clap to mark the take, and play a loop of the track so the performance, picture, and audio stay in sync.

Traditional slates assume a live boom and a linear scene. Music videos usually shoot to playback: one chorus, one verse, or a few measures on repeat while the take count climbs. Menzo Video is built around that workflow.

## What it does

- **On-camera slate** — Production, scene, shot, take, director, date, and the audio sync point, laid out like a clapperboard.
- **Visual clap** — The stick opens and slams shut, with a clap sound, so the camera has a clear picture and audio mark.
- **Loop playback** — Load an MP3 (or other supported audio), then loop a frame range or a measure range at a chosen frame rate.
- **Scene markers** — Name verse, chorus, and other sections, then send that range to the loop and the slate’s scene field.
- **Take counting** — After a clap, take number increases each time the loop wraps, matching how a music-video set actually works.

## Using it on set

1. Open `menzo.video` in a browser.
2. Fill in production, scene, shot, take, director, and date.
3. Load the playback track and set BPM, time signature, and frame rate.
4. Mark the section you are shooting (measures, or a named scene marker).
5. Put the slate in **Fullscreen slate** so it is easy to read on camera.
6. Hit **CLAP & PLAY LOOP**. The board claps, the sync timecode is written, and the loop starts.
7. Hit **Stop** on the slate when the take is over. Use **Next take** if you need to bump the number by hand.

## Slate controls

| Control | What it is for |
| --- | --- |
| **CLAP & PLAY LOOP** | Marks the loop start as the sync point, animates the clap, and starts looping. |
| **Stop** | Stops playback from the slate itself, without leaving the board. |
| **Next take** | Increments take without clapping. |
| **Fullscreen slate** | Fills the screen with the board so it is easier to film and read. |

Loop in/out can also be dragged on the waveform. In Measures mode, those handles snap to whole measures.

## Scene markers

Name a range such as `Chorus` from measure 17 to 24, then **Loop this**. The loop and the slate scene both follow that section. Point markers can still be dropped at the playhead, by double-clicking the waveform, or by pressing `M`. Markers are stored in the browser per filename.

## Playback notes

- **Frames mode** includes the start frame up to, but not including, the end frame.
- **Measures mode** starts at the start measure and ends at the start of the measure after the selected end measure.
- Supported frame rates: 24, 25, 29.97, 30, and 60 fps.

No build step or server is required. Everything runs locally in the page.
