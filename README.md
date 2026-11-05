# Spectrogram Lab

A hobby audio-analysis lab that runs entirely in the browser.

- **Analyze**: zoomable spectrogram that re-runs the FFT at the resolution of the current view, event scan (meows, Doppler-like tones, taps, swells), Doppler curve fitting.
- **Wildlife**: YAMNet sound classification plus BirdNET bird species ID with a regional filter, a timeline, and voice clustering to estimate how many individuals are calling.
- **Room sonar**: exponential-sweep impulse response, echo distances, reverb time per octave, 4-heading floor-plan fit, open-doorway detection.
- **recorder.html**: records the microphone (echo cancellation, noise suppression and auto gain off) while playing the sonar sweep, then analyzes on the spot and saves a WAV.

## Models and licenses
- YAMNet (Google), Apache 2.0, TF.js weights from TF Hub / Kaggle.
- BirdNET V2.4 (K. Lisa Yang Center for Conservation Bioacoustics), weights from the BirdNET Live project; model license CC BY-NC-SA 4.0 (non-commercial). Custom mel layer adapted from BirdNET Live (MIT).
- Weight shards use the `.wasm` extension only so static hosts serve them; they are TF.js binary weights.
