![BeatForge Screenshot](images/Screenshot%202025-07-05%20at%2011.25.10.png)

# BeatForge Drum Machine Plugin: Features

BeatForge is a JUCE-based drum machine plugin available as a PKG for macOS and VST3 for Windows, designed for music producers to create, sequence, and shape drum patterns with precision and creativity. Below is a concise overview of its key features and what you can do with them.

## 1. Multi-Track Sequencing

- **Up to 64 Tracks**: Manage multiple drum tracks (e.g., kick, snare, hi-hat) for complex arrangements.
- **16-Step Sequencer**: Program rhythms per bar with toggleable step buttons and visual playback feedback.
- **Bar Control**: Adjust total bars, navigate between them, and copy/paste patterns for quick variations.

**What You Can Do**: Build intricate, evolving drum patterns across multiple tracks and bars.

## 2. Sample Management

- **Load Samples**: Import .wav, .mp3, or .aiff files via dropdown or drag-and-drop.
- **Random Sample Mode**: Randomly select samples from a folder for dynamic variation.
- **Clear Samples**: Reset a track’s sample to start fresh.

**What You Can Do**: Create custom drum kits, add randomization, and manage samples easily.

## 3. Sound Design Controls

BeatForge’s tabbed interface (Mix, Envelope, Pitch & Dist, EQ, LFOs) offers detailed sound shaping per track, with settings tied to edit groups.

### Mix Tab

- **Volume (-112 to +12 dB)**: Adjust track gain, modulatable by LFO.
- **Pan (-1 to +1)**: Control stereo placement, LFO-modulatable.
- **Swing (50% to 75%)**: Add groove to rhythms.
- **Phase Invert**: Flip phase for creative or corrective effects.

### Envelope Tab (ADSR)

- **Attack (0 to 20 ms), Decay (0 to 1000 ms), Sustain (0 to 1), Release (1 to 2000 ms)**: Shape dynamics, all LFO-modulatable.

### Pitch & Distortion Tab

- **Pitch Shift (-12 to +12 semitones)**: Transpose samples.
- **Distortion (0 to 30 dB)**: Apply Soft, Hard, Foldback, or Hardcore distortion via right-click.
- **FX Send (-112 to +12 dB)**: Route to global effects, LFO-modulatable.
- **Reverse Playback**: Reverse samples with adjustable trim (0 to 16 steps).
- **Micro-Timing (-50 to +50 ms)**: Fine-tune trigger timing.
- **Bit Depth (2 to 16 bits)**: Add lo-fi bitcrushing effects.

### EQ Tab

- **High/Low-Pass Filters (20 Hz to 20 kHz)**: Enable and adjust cutoffs, LFO-modulatable.

### LFOs Tab

- **Three LFOs per Track**: Configure waveform (Sine, Square, Sawtooth, Triangle, White Noise), frequency (0.1 to 20 Hz or per-beat), depth (0 to 100%), and targets (volume, pan, pitch, distortion, FX send, ADSR, filters).

**What You Can Do**: Sculpt drum sounds with dynamics, distortion, and modulation for unique, evolving textures.

## 4. Edit Groups

- **32 Edit Groups**: Assign steps to groups (1 to 32) for unique settings (volume, pitch, etc.).
- **Copy/Paste Settings**: Transfer settings between groups for efficiency.

**What You Can Do**: Create varied sounds within a track, like different kick timbres per step.

## 5. MIDI Integration

- **MIDI Triggers**: Assign MIDI notes (0 to 127) for live or DAW triggering.
- **MIDI Output**: Send note-on/off to external devices (channels 1 to 16).
- **Synth Roll Mode**: Retrigger samples at MIDI note frequencies for synth-like effects.

**What You Can Do**: Perform live, sequence via MIDI, or control external gear.

## 6. Effects and Routing

- **Reverb**: Use convolution reverb with loadable impulse responses and adjustable return.
- **External Output**: Route tracks to Main (1-2) or Aux channels.
- **FX Bus**: Control per-track send levels, LFO-modulatable.

**What You Can Do**: Add depth with reverb, route tracks for DAW processing, and modulate effects.

## 7. Song Management

- **Save/Load Songs**: Store setups as .drsong files, with seamless switching during playback.

**What You Can Do**: Save and recall projects or switch songs live for performances.

## 8. Creative Tools

- **Hit Chances (5% to 100%)**: Add probabilistic triggering for organic variation.
- **Flam Counts (0 to 16)**: Create drum rolls with adjustable hits.
- **Mute Groups (1 to 8)**: Mute tracks interactively (e.g., hi-hats).
- **Solo/Mute**: Isolate or silence tracks.

**What You Can Do**: Introduce randomness, craft realistic rolls, and manage track interactions.

## 9. Workflow Features

- **Resizable UI**: Adjust window size (800x400 to 1920x1080).
- **Tabbed Interface**: Access Mix, Envelope, Pitch & Dist, EQ, and LFOs tabs.
- **Visual Feedback**: Flashing steps and track labels during playback.
- **Context Menus**: Right-click for quick settings access.
- **DAW Sync**: Syncs with DAW tempo and transport.

**What You Can Do**: Work efficiently with an intuitive, responsive interface.

## Tips

- Use edit groups for varied step sounds.
- Modulate parameters with LFOs for dynamic effects.
- Enable random sample mode for natural variation.
- Adjust micro-timing for humanized grooves.
- Route tracks to Aux channels for external processing.
- Save songs regularly as .drsong files.

## Notes

- **Platform Support**: Available as PKG for macOS and VST3 for Windows.
- **Releases**: Download the latest version from the [GitHub repository](https://github.com/Paulllux/BeatForge/releases).
