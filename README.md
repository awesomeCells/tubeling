<img src="logo.svg" alt="Tubeling logo" width="96" align="right">

# Tubeling

A little lab helper. Just a collection of small tools I often need when doing benchwork, vibe-coded with Claude, no guarantees. 
It has small tools for everyday bench work: timers, a counter, and calculators for units, concentrations, dilutions, centrifugation, nucleic acids, master mixes, sequences, text clean-up, time zones and experiment timepoints.
I tried to keep it all-in-one, with no dependencies.

## Usage

Open it online at https://awesomecells.github.io/tubeling/, or download `tubeling.html` and open it in a web browser. 
Settings are stored in the browser and should survive reloading the page, but probably not a restart. 
## Tools

Left column:

- **Pomodoro**: focus / short break / long break cycle with optional auto-start, sound and desktop notifications.
- **Countdown timers**: several at once, with labels; durations like `10`, `1:30`, `90s`, `2h`. Finished timers keep beeping until dismissed and keep running across reloads.
- **Stopwatch** with laps.
- **Counter**: one or more categories, counted with the keyboard; includes a hemocytometer calculator (cells/mL, viability).
- **Hydra tank**: a small easter egg. 

Tabs:
- **Units**: mass, volume, length, temperature, time, pressure, amount, radioactivity, energy, area, wavelength/energy.
- **Concentration**: molar ↔ mass concentrations, mass to weigh for a solution, concentration from mass and volume; list of common reagents with formula weights.
- **Dilution**: C₁V₁ = C₂V₂ (leave one field empty) and serial dilutions.
- **Centrifuge**: rpm ↔ × g for a given rotor radius.
- **DNA / RNA**: molecular weight, mass ↔ moles ↔ copies, concentration units, concentration from A260, ligation insert amount.
- **Master mix**: per-reaction and total volumes with overage, presets for common PCR/qPCR set-ups, copyable table.
- **Sequence**: paste raw, FASTA or GenBank text; DNA/RNA/protein is detected. Shows GC content, reverse complement, translation, ORFs, common restriction sites, motif search (IUPAC codes or regular expressions); for proteins mass, pI, ε280 and GRAVY.
- **Text**: character/word/line counts and clean-up operations (join lines, remove whitespace or numbers, FASTA reformatting, sort, unique).
- **Time zones**: compare zones for any date and time, with daylight-saving changes and an hour-by-hour planner.
- **Timepoints**: clock times of sampling points after a cut/amputation, flagged when they fall at night, on a weekend or outside working hours, plus suggested cut times for the next 7 days.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| Space | +1 to the selected counter |
| 1–9 | +1 to that counter row |
| ↑ / ↓ | select counter row |
| - | −1 to the selected counter |
| Backspace | undo last count |
| P | start / pause the pomodoro |

Enter adds a timer from the timer fields and adds a zone from the time-zone field.
## Notes

- The calculations are aids, no guarantees. Check results against your kit protocol, the reagent bottle (formula weights differ between salt and hydrate forms) and your rotor manual.
- The melting temperature shown for short DNA is a rough estimate (Wallace rule or a basic GC formula, no salt correction). Use a dedicated tool for primer design.
- Browsers only play sound after the page has been clicked or a key pressed once. Click anywhere on the page after opening it if you rely on timer alarms.
- Timer and pomodoro alarms are scheduled on the browser's audio clock, so they ring on time even in a background tab. This won't work on a computer on standby; use *Keep awake* in the header to keep the screen awake while the page is visible.
- Time-zone calculations use the browser's built-in time-zone database.

## License

MIT
