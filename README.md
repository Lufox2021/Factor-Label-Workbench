# Factor-Label Workbench

An interactive dimensional analysis (factor-label) tool for general chemistry students.

## What students can do

- **Solve & Check** – Enter a starting quantity and target units, build the conversion chain with units only, and check that they cancel. The number fields unlock once the units work out. Each numeric factor is checked against true values, and the answer appears on the right.
- **Tutor** – Work problems one factor at a time, with feedback after every step, hints, a "show next step" option, and a running score.
- **FL Calculator** – Work your own problem step by step. Enter the start and target, plus any given data from the problem (a density or concentration, for example), and each step is checked.
- **Units & notation** – A reference panel, open from any tab, listing every unit the tool accepts (metric and English, grouped by quantity) with their relationships, the metric prefixes, and how to type scientific notation. Tap a unit to add it to the box you're typing in.

## What it checks

- Unit cancellation, including squared and cubed units (raise a factor to a power only when the units need it)
- Metric prefixes, English↔metric, time, volume, pressure, energy and force conversions, and molarity (M, mM)
- Molar masses (computed from the formula, hydrates included), Avogadro's number, and mole ratios from a balanced equation
- Relationships given in the problem (density, molarity, percent)

Significant figures are not enforced. Answers are shown to 4 figures. Temperature conversions are not included.

## Typing units and numbers

- Powers: `cm^3`, `cm3` or `cm³`. Rates: `mi/h`, `m/s^2`, `g/mL`
- Substances go after the unit: `g NaCl`, `mol H2O`, `molecules CO2`, `L solution`
- Scientific notation: `6.022e23` (also `6.022x10^23` or `10^-3`). A line under the chain shows how each number was read.

## Problems

The page loads 12 built-in starter problems plus every row of `problems.csv` (currently 100 problems with worked solutions). Each row is checked when the page loads; rows with errors are skipped and listed at the bottom of the page.

To add or change problems, edit `problems.csv` in Excel and upload it here to replace the old file. Columns: `prompt`, `topic`, `start`, `target`, `solution`, and optionally `given`, `equation`, `hint`. Separate solution factors with semicolons (`1609 m / 1 mi; 1 h / 3600 s`) and write powers as `(2.54 cm / 1 in)^3`.

The whole tool is a single self-contained `index.html` file.
