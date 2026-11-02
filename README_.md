# Trixordo Studio

A web app for learning rebetiko and laiko songs on the **trixordo** (3-course, 6-string bouzouki, tuned D–A–D).

Load a recording and the app transcribes the bouzouki line into tab. It then shows each note on an interactive fretboard with the fret, string and finger to use.

**Live site:** https://YOUR-USERNAME.github.io/trixordo-studio/

## Features

- **Fretboard view:** a trixordo neck that lights up the current note with its finger number and shows the next note.
- **Tab sheet:** fret numbers on the three courses, colored finger markers, note lengths, and an optional staff with Western (C D E) or Greek (Ντο Ρε Μι) note names.
- **Click to jump:** click any note in the tab to move playback there.
- **Practice tools:** slow down without changing pitch (50–100%), loop a section, and play the transcription on a synthesized bouzouki to compare it with the recording.
- **Transcription:** finds the main melody in the bouzouki's range, adjusts for out-of-tune old recordings, and skips sung notes so whole songs work.
- **Dromos guide:** guesses the dromos (Hijaz, Ousak, Rast, Sabah and others), shows it on the neck and plays the scale.
- **Editing:** fix a note by clicking the right spot on the fretboard. Undo, save to a library in your browser, and export or import tabs as JSON.
- **Demo:** an original practice phrase in Hijaz on D loads on startup.

## How it works

Everything runs in your browser. Audio files are never uploaded anywhere. The transcriber finds pitches by summing harmonics, follows the melody over time, detects note attacks, and tells plucked notes from sung ones by how steady their pitch is. Fingerings are chosen to keep hand movement small.

Built with plain HTML, CSS and JavaScript. It has no dependencies other than Google Fonts.

## Limitations

The transcriber hears one note at a time and can still pick up the singer or other instruments. Treat its output as a draft to check by ear.

## License

All rights reserved. See [LICENSE](LICENSE).
