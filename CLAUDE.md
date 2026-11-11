# Spectrogram Lab

Eli's hobby audio lab, all in the browser: a zoomable spectrogram that re-renders at higher
resolution as you zoom, event scan, aircraft Doppler curve fitting (the idea came from a
YouTube video about geolocating recordings by plane sounds), wildlife ID (YAMNet, BirdNET),
and room sonar. He wants it built properly in code, to the standard of paid tools.

Eli is not a programmer. Explain changes in plain words, tell him what to try, and walk him
through any GitHub step one tap at a time. Never use em dashes in anything written for him.

## Where the app lives

- **The real app is this repository, served by GitHub Pages**:
  https://eliman51.github.io/spectrogram-lab . Pushing to `main` updates it.
- The Claude artifact "Spectrogram Lab" (slug `b6ef8050-ea13-4ef8-80db-f4757781aef0`) is an
  older snapshot from before the phone-screen fixes. Do not copy from it and do not publish to
  it unless Eli asks.
- This repository is **public** (needed for free GitHub Pages). Nothing private goes in it.

## Files

- `index.html` the app (about 2,000 lines). `recorder.html` the sonar recorder page.
- `yamnet/`, `birdnet/` model weights (the `.wasm` names are only so static hosts serve them;
  they are TF.js weights). BirdNET is CC BY-NC-SA 4.0: non-commercial only. Do not change or
  re-download these unless a change needs it; they are large.
- `sonar/*.wav` test recordings. `.nojekyll` keeps GitHub Pages from hiding folders.
- Eli made a test recording, "County Road 335", with his iPhone and wants it in the app. It is
  not in this repository yet; if he sends it, add it under `recordings/` and load it from there.

## Every change

1. Edit the files.
2. Make sure every inline script still parses (copy the check from another of Eli's repos or
   run `node --check` on the extracted script).
3. Commit with a plain message and push to `main`. Tell Eli what changed and what to try.
