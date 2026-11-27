<img src="logo.svg" alt="Tubeling logo" width="96" align="right">

# Tubeling

A little lab helper, built with Claude, no guarantees. 
It offers a bunch of small tools for everyday bench work: timers, a counter, and calculators for concentrations, centrifugation, master mixes, text clean-up, time zones and experiment timepoints.

## Usage

Open it online at https://awesomecells.github.io/tubeling/, or download `tubeling.html` and open it in a web browser. 
Settings are stored in the browser and should survive reloading the page. 
## Tools

Left column:

- **Timers**: one card with tabs; they run in parallel.
  - **Pomodoro**: focus / short break / long break cycle with optional auto-start, sound and desktop notifications.
  - **Countdown timers**: several at once, with labels; durations like `10`, `1:30`, `90s`, `2h`; click a name to rename it. Finished timers keep beeping until dismissed and keep running across reloads.
  - **Stopwatch** with laps.
- **Hydra tank**: a small easter egg. 

Tabs:
- **Text**: character/word/line counts and clean-up operations (join lines, remove whitespace or empty lines, unique lines, upper/lower case, FASTA reformatting).
- **Counter**: one or more categories, counted with the keyboard. Can also count cells square by square in a Neubauer improved or Fuchs-Rosenthal chamber (cells/mL, viability).
- **Time zones**: compare zones for any date and time, with daylight-saving changes and an hour-by-hour planner.
- **Timepoints**: clock times of sampling points after a cut/amputation, flagged when they fall at night, on a weekend or outside working hours, plus suggested cut times for the next 7 days.
- **Concentration**: molar ↔ mass concentration, mass to weigh for a solution (never less than 10 mg; suggests a stock to dilute instead), concentration from mass and volume; list of common reagents with formula weights.
- **Centrifuge**: rpm ↔ × g for a given rotor radius.
- **Master mix**: per-reaction and total volumes with overage, presets for common PCR/qPCR set-ups, copyable table.

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| Space | +1 to the selected counter |
| 1–9 | +1 to that counter row |
| ↑ / ↓ | select counter row |
| - | −1 to the selected counter |
| Backspace | undo last count |
| P | start / pause the pomodoro |
| Enter | next square (cell counting) |

Counter keys work while the Counter tab is open. Enter adds a timer from the timer fields and adds a zone from the time-zone field.
## Notes

- The calculations are aids, no guarantees. Check results against your kit protocol, the reagent bottle (formula weights differ between salt and hydrate forms) and your rotor manual.
- Browsers only play sound after the page has been clicked or a key pressed once. Click anywhere on the page after opening it if you rely on timer alarms.
- Timer and pomodoro alarms are scheduled on the browser's audio clock, so they ring on time even in a background tab. This won't work on a computer on standby; use *Keep awake* in the header to keep the screen awake while the page is visible.
- Time-zone calculations use the browser's built-in time-zone database.

## License

MIT
