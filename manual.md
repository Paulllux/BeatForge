BeatForge Drum Machine Plugin: Features
BeatForge is a JUCE-based drum machine plugin available as a PKG for macOS and VST3 for Windows, designed for music producers to sequence and manipulate user-loaded audio samples with advanced control. Below is a concise overview of its key features and what you can do with them, based on the provided codebase.
1. Multi-Track Sequencing

Up to 64 Tracks: Manage multiple tracks, each hosting a user-loaded audio sample (e.g., kick, snare, hi-hat).
16-Step Sequencer: Program rhythms per bar with toggleable step buttons, offering visual feedback during playback.
Bar Control: Set total bars, navigate between them, and copy/paste patterns for efficient arrangement.

What You Can Do: Create complex, multi-layered drum patterns and manage extended sequences across bars.
2. Sample Management

Load Samples: Import .wav, .mp3, or .aiff files via dropdown or drag-and-drop into track-specific sample slots.
Random Sample Mode: Randomly select samples from the same folder as the loaded sample for varied playback.
Clear Samples: Reset a track’s sample to clear settings and buffer.

What You Can Do: Build custom sample-based drum setups, add randomization, and manage sample libraries.
3. Sound Design Controls
BeatForge’s tabbed interface (Mix, Envelope, Pitch & Dist, EQ, LFOs) provides per-track sound shaping, with settings tied to edit groups.
Mix Tab

Volume (-112 to +12 dB): Adjust track gain, modulatable by LFO.
Pan (-1 to +1): Control stereo placement, LFO-modulatable.
Swing (50% to 75%): Add groove to rhythms.
Phase Invert: Flip phase for corrective or creative effects.

Envelope Tab (ADSR)

Attack (0 to 20 ms), Decay (0 to 1000 ms), Sustain (0 to 1), Release (1 to 2000 ms): Shape sample dynamics, all LFO-modulatable.

Pitch & Distortion Tab

Pitch Shift (-12 to +12 semitones): Transpose samples with precomputed buffers for efficiency.
Distortion (0 to 30 dB): Apply Soft, Hard, Foldback, or Hardcore distortion via right-click menu.
FX Send (-112 to +12 dB): Route to global effects, LFO-modulatable.
Reverse Playback: Reverse samples with adjustable trim (0 to 16 steps).
Micro-Timing (-50 to +50 ms): Fine-tune trigger timing for humanized rhythms.
Bit Depth (2 to 16 bits): Apply lo-fi bitcrushing effects.

EQ Tab

High/Low-Pass Filters (20 Hz to 20 kHz): Enable and adjust cutoffs, LFO-modulatable.

LFOs Tab

Three LFOs per Track: Configure waveform (Sine, Square, Sawtooth, Triangle, White Noise), frequency (0.1 to 20 Hz or per-beat, synced to DAW tempo), depth (0 to 100%), and targets (volume, pan, pitch, distortion, FX send, ADSR, filters).

What You Can Do: Shape sample playback with precise dynamics, distortion, and LFO-driven modulation for evolving sounds.
4. Edit Groups

32 Edit Groups: Assign steps to groups (1 to 32) for unique settings (volume, pitch, distortion, etc.), color-coded for clarity.
Copy/Paste Settings: Transfer settings between groups for workflow efficiency.

What You Can Do: Apply varied sound parameters to different steps within a track, like unique pitch or distortion per step.
5. MIDI Integration

MIDI Triggers: Assign MIDI notes (0 to 127 or None) to trigger tracks via MIDI keyboard or DAW.
MIDI Output: Send note-on/off messages to external devices (channels 1 to 16), with velocity based on track volume.

What You Can Do: Perform live, sequence tracks via MIDI, or control external devices.
6. Effects and Routing

Reverb: Apply convolution reverb with loadable .wav or .aiff impulse responses and adjustable return level.
External Output: Route tracks to Main (1-2) or Aux channels for DAW processing.
FX Bus: Control per-track send levels to the effects bus, LFO-modulatable.

What You Can Do: Add spatial depth with reverb, route tracks for external processing, and modulate effects dynamically.
7. Song Management

Save/Load Songs: Save setups as .drsong files, including tracks, samples, and settings, with seamless switching during playback.

What You Can Do: Preserve and recall projects or switch songs live for performances.
8. Creative Tools

Hit Chances (5% to 100%): Set probabilistic triggering for randomized, organic patterns.
Flam Counts (0 to 16): Create drum rolls with adjustable hit counts.
Mute Groups (1 to 8): Configure tracks to mute each other (e.g., for hi-hat patterns).
Solo/Mute: Isolate or silence tracks for mixing.

What You Can Do: Add randomness, craft realistic rolls, and manage track interactions for dynamic arrangements.
9. Workflow Features

Resizable UI: Adjust window size (800x400 to 1920x1080).
Tabbed Interface: Navigate Mix, Envelope, Pitch & Dist, EQ, and LFOs tabs.
Visual Feedback: Step buttons and track labels flash during playback.
Context Menus: Right-click track labels or steps for quick settings access (e.g., MIDI, edit groups).
DAW Sync: Syncs with DAW tempo and transport.

What You Can Do: Work efficiently with an intuitive, visually responsive interface.
Tips

Use edit groups to vary step sounds within a track.
Experiment with LFO modulation for dynamic effects.
Enable random sample mode for natural variation.
Adjust micro-timing for humanized or precise rhythms.
Route tracks to Aux channels for DAW processing.
Save songs regularly as .drsong files.

Notes

Platform Support: Available as PKG for macOS and VST3 for Windows.
Releases: Download the latest version from the GitHub repository.
