[README.md](https://github.com/user-attachments/files/34038089/README.md)
# Factor-Label Workbench

An interactive dimensional analysis (factor-label) tool for general chemistry students.

**Use it:** https://lufox2021.github.io/factor-label-workbench/

## What students can do

- **Solve & Check** – Enter a starting quantity and target units, build the conversion chain with units only, and check that they cancel. The number fields unlock once the units work out. Each numeric factor is checked against true values, and the answer appears on the right.
- **Tutor** – Work built-in problems one factor at a time, with feedback after every step, hints, a "show next step" option, and a running score.
- **FL Calculator** – Work your own problem step by step. Enter the start and target, plus any given data from the problem (a density or concentration, for example), and each step is checked.

## What it checks

- Unit cancellation, including squared and cubed units (raise a factor to a power only when the units need it)
- Metric prefixes, English↔metric, time, volume, pressure and energy conversions
- Molar masses (computed from the formula, hydrates included), Avogadro's number, and mole ratios from a balanced equation
- Relationships given in the problem (density, molarity, percent)

Significant figures are not enforced. Answers are shown to 4 figures.

## Typing units

- Powers: `cm^3`, `cm3` or `cm³`. Rates: `mi/h`, `m/s^2`, `g/mL`
- Substances go after the unit: `g NaCl`, `mol H2O`, `molecules CO2`, `L solution`
- Large and small numbers: `6.022e23` or `6.022x10^23`

## Note

This GitHub version includes the 12 built-in starter problems. The instructor problem bank (saving new problems and uploading spreadsheets) is available only in the Claude-hosted version.

The whole tool is a single self-contained `index.html` file.
