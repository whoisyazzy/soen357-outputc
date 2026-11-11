# Meal Planning Assistant – Output C interactive prototype

Sample prototype for learning and educational purposes only. Not for commercial use or commercial testing.
SOEN 357 Phase 2, The Vth Division. Version: Output C (snapshot of 11 Nov 2026).

## Open it locally
1. Download `index.html`.
2. Double-click it, or drag it into Chrome, Edge, Firefox or Safari. No installation or internet connection is needed (the font is embedded).
3. On a computer, the app is shown at phone width (375 px). For other widths, open the browser's developer tools and use responsive mode (320–430 px).

## Publish it on GitHub Pages
1. Create a public repository, e.g. `soen357-meal-planner-c`.
2. Upload `index.html` (and this README) to the root of the `main` branch.
3. Go to Settings → Pages → Source: "Deploy from a branch", Branch: `main`, folder `/ (root)` → Save.
4. After about a minute the link is `https://<github-username>.github.io/soen357-meal-planner-c/`.
5. Open the link in a private window on a phone and a computer to check it works before submitting.

## Essential tasks
- T1 Manage pantry: Pantry → Add ingredient → add Zucchini (2 units, Fridge, Reminder 7 Nov 2026) → Save. Then open Zucchini, change the quantity, Save.
- T2 Select a suitable meal: Meals → Zucchini and tomato rice skillet → Select this meal.
- T3 Prepare grocery list: Meals → Vegetable pasta → Select this meal → Add 1 missing item to grocery list → View grocery list → edit the quantity.

## Simulated behaviour and limitations
- All names, foods, recipes and dates are fictional sample data (Section 2.4, plus two extra fictional recipes: one containing peanuts, to show the allergy filter, and one longer than 30 minutes, to show search beyond the time filter).
- "Today" is fixed at 5 Nov 2026 so that the zucchini reminder shows as "Use soon".
- Suggestions come from a fixed rule set (Use soon items first, then fewer missing items, then shorter time). There is no AI model and no server.
- Ingredients are matched to the pantry by name only; quantities are not compared.
- Changes are kept in memory for the session. Reloading the page (or Profile → Reset sample data) restores the sample data.
- Dietary preferences are stored but do not filter the sample recipes.
- There are no loading states because nothing is fetched.

## Credits
Font: Atkinson Hyperlegible, Braille Institute of America, SIL Open Font License 1.1 (embedded via @fontsource/atkinson-hyperlegible).
