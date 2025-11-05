# Solfege Trainer - Extended Range Pattern Display

A Python application for smartboards that displays extended range solfege patterns (low so to high do) on a five-line staff. Perfect for music education and solfege practice!

## Features

- **Five-line staff**: Extended staff with lines for ti, sol, mi, do, and low la
- **Extended range**: 10 different notes from low so (G3) to high do (C5)
- **4-note patterns**: Each pattern contains exactly 4 notes from the extended range
- **Random generation**: Click "New Pattern" to generate new random patterns
- **Play Pattern**: Click "Play Pattern" to hear the entire pattern at 75 BPM
- **Interactive notes**: Click any note to hear its pitch played on piano
- **Fullscreen mode**: Press F11 or click the Fullscreen button for smartboard display
- **Touch-friendly**: Large buttons designed for smartboard interaction
- **Color-coded notes**:
  - Do notes are red (on line and above ti)
  - Re notes are orange (space between mi and do)
  - Mi notes are yellow (on line)
  - Fa notes are light green (space between sol and mi)
  - Sol notes are dark green (on line and below low la)
  - La notes are purple (space between ti and sol, and on line)
  - Ti notes are light purple (on line)
- **Hide/Show controls**:
  - Hide Names button: Toggle visibility of note names below staff
  - Hide Labels button: Toggle visibility of all note labels on the left
  - Play Pattern button: Play the current pattern at 75 BPM

## Requirements

- Python 3.6 or higher
- tkinter (usually included with Python)
- pygame (for audio playback)

## Installation

Install pygame for audio support:

```bash
pip install pygame
```

## Usage

### Running the Application

```bash
python3 solfege_trainer.py
```

or make it executable:

```bash
chmod +x solfege_trainer.py
./solfege_trainer.py
```

### Controls

- **New Pattern button**: Generate a new random 4-note pattern
- **Fullscreen button** or **F11**: Toggle fullscreen mode
- **Hide Names button**: Toggle visibility of note names below the staff
- **Hide Labels button**: Toggle visibility of all note labels on the left side
- **Play Pattern button**: Play the entire pattern at 75 BPM
- **Click any note**: Play the note's pitch individually
- **Escape**: Exit fullscreen mode

## How It Works

1. The application displays a five-line staff with extended range notes:
   - **High Do** (red) - above the ti line
   - **Ti** (light purple) - on top line
   - **La** (purple) - in the space between ti and sol, touching both lines
   - **Sol** (dark green) - on second line
   - **Fa** (light green) - in the space between sol and mi, touching both lines
   - **Mi** (yellow) - on middle line
   - **Re** (orange) - in the space between mi and do, touching both lines
   - **Do** (red) - on fourth line
   - **Low La** (purple) - on bottom line
   - **Low So** (dark green) - below the bottom line

2. Each pattern contains 4 notes randomly chosen from the extended range (low so to high do)

3. Notes are displayed as simple note heads (circles) without stems

4. The pattern can be shown in text form below the staff (toggle with Hide Names button)

5. Click "Play Pattern" to hear the entire 4-note sequence at 75 BPM

6. Click any individual note to hear its piano pitch:
   - Low So = G3 (196.00 Hz)
   - Low La = A3 (220.00 Hz)
   - Do = C4 (261.63 Hz)
   - Re = D4 (293.66 Hz)
   - Mi = E4 (329.63 Hz)
   - Fa = F4 (349.23 Hz)
   - Sol = G4 (392.00 Hz)
   - La = A4 (440.00 Hz)
   - Ti = B4 (493.88 Hz)
   - High Do = C5 (523.25 Hz)

## Perfect For

- Elementary and intermediate music classrooms
- Extended range solfege practice
- Smartboard/interactive whiteboard lessons
- Teaching pitch recognition across octaves
- Interval training with wider range
- Ear training exercises
- Music theory fundamentals
- Melodic dictation practice

## Customization Ideas

You can modify the code to:
- Change the tempo (currently 75 BPM)
- Change the number of notes per pattern (currently 4)
- Include rhythm patterns with varying note durations
- Add difficulty levels (limit range for beginners)
- Change note durations or timbres
- Add major/minor mode selection
- Add chromatic notes (sharps/flats)
- Add option to restrict to pentatonic scale only
- Add visual feedback when notes are playing
