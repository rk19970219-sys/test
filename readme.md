# MIDI Sawtooth Synth

Name: Havirbhavi Pothugunta

## Description

This project is a personal MIDI soft synthesizer written in Python. It listens for MIDI note events from a MIDI input device and generates audio through the computer's default audio output.

The synth is monophonic and uses a sawtooth waveform. It includes a fixed attack-release envelope: notes ramp up over 10 milliseconds when started and ramp down over 10 milliseconds when released. A `note_on` message with velocity 0 is treated as a `note_off` message.

I also added two extra features: selecting a MIDI input device using `--midi-device`, and using MIDI KEY ON velocity to control note volume.

## Files

- `synth.py` - main MIDI synthesizer program
- `play_notes.py` - small MIDI note sender used for testing with loopMIDI
- `requirements.txt` - Python package dependencies
- `SYNTH.mp4` - short demo video showing the synth working

## Requirements

Install dependencies with:

```bash
pip install -r requirements.txt
