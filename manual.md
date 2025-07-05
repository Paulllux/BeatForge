# BeatForge Manual

## Introduction

BeatForge is a powerful drum sequencer and sampler plugin designed for crafting dynamic drum patterns and beats. It provides a comprehensive set of tools for track management, step sequencing, effects processing, and song creation, making it an ideal choice for music producers.

The Idea was to make something that looks like your basic step sequencer, untill you dig deeper. 

### Key Features

- Up to 64 tracks
- 16-step sequencer per bar
- Multiple bars per song
- Sample loading and management
- Solo and mute functionality
- Volume, pan, swing, and phase invert controls
- ADSR envelope
- Pitch shift, distortion, and FX send
- High-pass and low-pass filters
- Three LFOs per track
- MIDI input and output support, including Synth Roll Mode
- Song saving and loading

## Installation

### macOS

1. **Download the Installer:**
   - Obtain the BeatForge PKG installer from the [GitHub repository](https://github.com/your-repo/beatforge).

2. **Run the Installer:**
   - Double-click the downloaded `.pkg` file and follow the on-screen instructions to install BeatForge.

3. **Automatic File Placement:**
   - The PKG installer will automatically install the plugin components into the following standard locations:
     - **VST3 Plugin:** `/Library/Audio/Plug-Ins/VST3/BeatForge.vst3`
     - **Audio Unit (AU) Plugin:** `/Library/Audio/Plug-Ins/Components/BeatForge.component`

4. **Post-Installation:**
   - Restart your Digital Audio Workstation (DAW) to allow it to scan and recognize the newly installed plugins.

### Windows

1. **Download the Plugin:**
   - Download the BeatForge VST3 plugin file (`BeatForge.vst3`) from the [GitHub repository](https://github.com/your-repo/beatforge).

2. **Manual Installation:**
   - Copy the `BeatForge.vst3` file to the standard VST3 directory:
     - `C:\Program Files\Common Files\VST3\`

3. **DAW Configuration:**
   - Open your DAW and rescan your plugin folders if the plugin isn’t automatically detected. Check your DAW’s settings to ensure `C:\Program Files\Common Files\VST3\` is included in the plugin search path.

### Notes

- **DAW Compatibility:** Ensure your DAW supports VST3 (Windows and macOS) or AU (macOS) formats.
- **Verification:** If the plugin doesn’t appear in your DAW, confirm the files are in the correct locations and rescan plugins manually.

## User Interface Overview

The plugin's user interface is intuitive and divided into several key sections:

- **Track Selector:** Manage tracks by adding, deleting, or selecting them.
- **Track Controls:** Adjust track name, sample selection, solo, and mute settings.
- **Step Sequencer:** Program drum hits with 16-step buttons per bar.
- **Tab Controls:** Switch between parameter tabs: Mix, ADSR, FX, EQ, and LFO.
- **Bar Controls:** Set total bars, navigate between bars, and copy/paste bar data.
- **Song Controls:** Save and load songs via the "Song" button.

## Track Management

- **Adding a Track:** Click the "Add Track" button to create a new track (up to 64 tracks).
- **Deleting a Track:** Right-click the track name and select "Delete Track" from the context menu.
- **Track Settings:**
  - **Name:** Double-click the track name to edit it.
  - **Sample:** Use the dropdown to select or load a sample, or drag and drop an audio file onto the track.
  - **Solo (S):** Mutes all other tracks when enabled.
  - **Mute (M):** Silences the track.

Right-clicking a track name opens a context menu with additional options:
- **Delete Track:** Removes the track.
- **Delete Sample:** Clears the loaded sample.
- **Random Sample Mode:** Toggles random sample selection from a folder.
- **Output Settings:** Choose the audio output channel pair (e.g., Main 1-2, Aux 3-4). Set more output in your DAW first to options besides Main 1-2.
- **MIDI Settings:** Set MIDI note (0-127 or None) and channel (1-16 or None). Choose Direction, midi in or midi out to control other VST instruments.
- **Mute Group:** Assign to a mute group (1-8 or None) to mute other tracks in the same group when triggered. Usually used for open and closed hihats
- **Synth Roll Mode:** Enable to trigger a continuous roll of the sample at the frequancy of the midi note while a MIDI note is held (requires MIDI note and channel).

## Step Sequencing

Each track features a 16-step sequencer for programming drum hits:

- **Step Buttons:** Click to toggle a hit on or off.
- **Hit Chance:** Right-click a step to set its probability (5% to 100% in 5% increments).
- **Groups:** Assign steps to edit groups (1-32) via right-click menu for shared settings.
- **Roll (Flam):** Right-click to set roll count (1-16) for repeated hits within a step.

Right-clicking a step button provides options:
- **Chance:** Adjust hit probability.
- **Group:** Set the edit group for shared parameter control.
- **Group Settings:** Copy or paste settings (e.g., volume, pitch) between groups.
- **Roll:** Configure repeated hits.

## Bar and Song Management

- **Total Bars:** Use the "+" and "−" buttons next to "Total Bars" to set the song length (minimum 1 bar).
- **Current Bar:** Navigate between bars using the "+" and "−" buttons next to "Bar X".
- **Copy/Paste Bar:** 
  - Click "Copy" to save the current bar's settings.
  - Click "Paste" to apply the copied settings to another bar.
  - Right-click a track for track-specific copy/paste options.

## Effects and Processing

Effects and processing options are organized into tabs per track:

- **Mix Tab:**
  - **Volume:** Adjust track volume (-60 dB to +12 dB).
  - **Pan:** Set stereo position (-1 to +1).
  - **Swing:** Apply swing timing (50% to 75%) to the even steps, similar to your classic Roland Drumcomputers
  - **Phase Invert:** Toggle to invert the audio phase. Try what sounds best.

- **ADSR Tab:**
  - **Attack:** Set onset time (0 to 0.02 seconds). Turn op for smoother hits.
  - **Decay:** Control fade-out time (0.01 to 1000 ms). Make those hits shorter, in case you need to tame those long 808 samples, cut of reverb etc.
  - **Sustain:** Adjust sustain level (0 to 1). Decay won't do anything when this is up.
  - **Release:** Set release time (1 to 2000 ms). How fast the sample stops playing when the next hit comes, if this is high, you'll get overlaps. 4 voices are used per track.

- **FX Tab:**
  - **Pitch Shift:** Adjust pitch (-12 to +12 semitones).
  - **Distortion:** Increase distortion drive (0 to 30 dB); right-click for type (Soft, Hard, Foldback, Hardcore). Make Drums Dirty Again.
  - **FX Send:** Control send level to FX bus (-112 dB to +12 dB). to sent to an external processor, or throw in an IR for internal reverb.
  - **Reverse:** Toggle reverse playback. for those swells
  - **Trim:** Set reverse trim steps (0 to 16). If you set trim to 2 for example, program the reversed step two steps before where you want the peak to come.
  - **Microtiming:** Adjust timing offset (-50 to +50 ms).
  - **BitCrush:** Reduce bit depth (2 to 16 bits; 16 = Off).For those old videogame sound, welcome to pacman zone.

- **EQ Tab:**
  - **High-Pass Filter:** Toggle and set cutoff (20 Hz to 20 kHz).
  - **Low-Pass Filter:** Toggle and set cutoff (20 Hz to 20 kHz).
  very basic untill now, just to tame excessive highs or lows. I recommend using separate outputs if you need to fine tune the sounds more.

- **LFO Tab:**
  - Three LFOs per track with:
    - **Enable:** Toggle LFO on/off.
    - **Frequency:** Set rate (0.1 to 20 Hz or 0.1 to 10 per beat; right-click to switch mode).
    - **Amplitude:** Adjust depth (0% to 100%).
    - Right-click for options: Mode (Hz or Per Beat), Type (Sine, Square, Sawtooth, Triangle, White Noise), Targets (e.g., Volume, Pitch).
    this can make some really weird sound, release your inner Aphex Twin with these, experiment. Make it play melodies by targeting the pitch shift. Combine with hitchances, random samples and every bar can sound completely different.

## MIDI and Output Settings

- **MIDI Note:** Right-click a track to set a MIDI note (0-127 or None) for triggering or output.
- **MIDI Channel:** Select a MIDI channel (1-16 or None) for input/output.
- **Direction:** Choose MIDI Input or Output mode via the context menu.
- **Output Channel:** Assign the track to an audio output pair (e.g., Main 1-2, Aux 3-4).
- **Synth Roll Mode:** When enabled, holding the assigned MIDI note triggers a continuous roll of the sample until the note is released.

Global MIDI and FX settings:
- **FX Mode:** Choose "External Output" or "Internal Reverb" via the dropdown.
  - **External Output:** Select output pair (e.g., Main 1-2).
  - **Internal Reverb:** Load an impulse response (IR) file and adjust reverb return level (0 to 1).

## Song Saving and Loading

- **Save Song:** Click the "Song" button and select "Save" (overwrites current file) or "Save As" (choose new file).
- **Load Song:** Select "Load Song" to open a `.drsong` file, or use the song dropdown to switch between files in the same directory.

## Tips and Tricks

- **Random Samples:** Enable "Random Sample Mode" to cycle through samples in a folder automatically.
- **Dynamic Patterns:** Use hit chances and rolls to create evolving rhythms.
- **LFO Modulation:** Assign LFOs to parameters like pitch or volume for movement in your patterns.
- **Mute Groups:** Group tracks (e.g., hi-hats) to cut off overlapping sounds naturally.
- **FX Bus:** Send multiple tracks to the FX bus for unified reverb or external processing.
- **Synth Roll Mode:** Use this mode for creating dynamic fills or textures by holding MIDI notes.

This manual provides everything you need to start using BeatForge effectively. Enjoy creating your beats!


