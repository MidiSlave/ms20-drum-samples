# MS-20 Drum Samples

A collection of MS-20 drum samples for use with [Strudel](https://strudel.tidalcycles.org/) live coding environment.

## Categories

- **kicks**: 31 kick drum samples
- **snares**: 69 snare drum samples  
- **toms**: 32 tom samples
- **cymbals**: 56 cymbal and hi-hat samples
- **percs**: 61 percussion samples (including congas)

## Usage in Strudel

Load the samples in your Strudel session:

```javascript
await samples('github:MidiSlave/ms20-drum-samples')
```

Then use the samples by referencing the category and index:

```javascript
// Play different kicks
s("kicks:0 kicks:1 kicks:2 kicks:3")

// Play a simple beat
s("kicks:0 ~ snares:5 ~")

// Use different samples
s("kicks:10 [~ percs:5] snares:20 cymbals:2")

// Layer multiple samples
s("kicks:0, cymbals:8*4, ~ snares:5 ~ snares:5")
```

## Sample Naming

Samples maintain their original descriptive names in the filesystem, but are accessed by numerical index in Strudel (0-based):

- `kicks:0` = -distort-a_p.wav
- `kicks:1` = -distort-b_p.wav
- `snares:0` = acoustic1ap.wav
- etc.

## Credits

MS-20 drum samples processed and organized for Strudel.