# GTU BME steam dryness fraction and enthalpy calculator

For GTU Basic Mechanical Engineering (3110006, BE01000081, BE01R00081). Unit 2, Properties of Gases and Steam, is 22% of the official BE01000081 syllabus, the biggest unit. GTU Hero's BME guide lists 'calculate dryness fraction of steam at given pressure' as a standard question type, and steam tables are permitted in the exam. Ye page wet steam ka h, x aur v nikalta hai. You type hf, hfg and vg from your own steam table row.

Live page: https://princeadvant.github.io/gtu-bme-steam-dryness-calculator/

## Formulas

- h = hf + x hfg (kJ/kg)
- x = (h - hf) / hfg
- v = x vg (liquid volume neglected)
- Separating calorimeter: xs = m / (m + M)
- Combined separating + throttling: x = xs x xt

## Test

`node test.js` checks the formulas against hand-worked values and prints `All checks passed`.

## Tips

- Default numbers are illustrative only. Read hf, hfg and vg from the exact pressure row of your steam table.
- Dryness fraction x is between 0 and 1. If you get more than 1, the steam is superheated or you used the wrong row.
- GTU Hero's guide warns that unofficial solutions often read dryness fraction values from the wrong steam table row.

Old papers and repeat counts: [GTU BME Paper: Old Papers and PYQs on GTU Hero](https://gtuhero.com/blogs/gtu-bme-paper-previous-year-papers-pyq) (GTU Hero is my project).
