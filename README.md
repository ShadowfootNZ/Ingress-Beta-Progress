# Ingress +β Progress Tracker

A small, client-side progress tracker for the Ingress +β event.  Test it out: https://ShadowfootNZ.github.io/Ingress-Beta-Progress/
Enter your current score and the page will show days remaining, remaining bounty points, and how far you are from Bronze / Silver / Gold targets.

Features
- Shows days remaining until the event end date.
- Calculates remaining bounty points (60 pts/day).
- Displays how many points or days of bounties are needed for each tier.
- Uses custom tier icons (one image per tier) placed next to each target.

Usage
1. Enter your current score in the input and press Enter or click "Calculate".
2. The page updates:
   - Days remaining
   - Remaining bounty points available
   - Targets with tier icons and points/days needed

Assets
- Drop these image files into the same folder as `index.html`:
  - `beta bronze.png`
  - `beta silver.png`
  - `beta gold.png`
- Filenames must match the values in the `icons` map inside `index.html`. You can change those filenames in the script if desired.

Customization
- Event dates and tier thresholds are defined at the top of `index.html`:
  - `startDate` and `endDate`
  - `tiers` object (e.g. `{ bronze: 3000, silver: 6000, gold: 9000 }`)
- Daily bounty points assumed: 60 (6 × 10). Update the calculation in `index.html` if this changes.

Development notes
- The tracker is entirely client-side and requires only a modern browser.
- Styling and icon sizes live in the `<style>` block of `index.html`.

License
- Unlicensed / use as you like. If sharing, please include attribution.

Contact / Issues
- Open an issue in the repository or edit the files directly and submit a pull request.
