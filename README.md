# Moje Wykresy Piłkarzy / My Player Charts

Project overview  
This repository contains visual analyses of football players: radar charts, shotmaps and pass/position maps created from match and season data. Each image is accompanied by a short description explaining what the chart shows and how to interpret it.

How to reproduce (if source data &amp; scripts are present)  
1. Clone the repository:  
   git clone https://github.com/kowalczyk350/Moje-wykresy-pilkarzy.git  
2. Install dependencies (if scripts are provided):  
   - Python: `pip install -r requirements.txt`  
   - Node: `npm install`  
3. Run the chart generation script (example): `python generate_charts.py` or open the provided .html files in a browser.

Chart descriptions (English)
- Doku i Wittz.jpeg  
  This radar chart compares a selected set of normalized performance metrics for Jeremy Doku and Wittz during the analysed match/period. Each axis represents a different metric (for example: successful dribbles, pass accuracy, key passes, shots on target), and values are scaled so metrics with different ranges can be compared directly. The visualization highlights contrasting strengths and tactical roles, making it easy to see where one player outperforms the other. Use the corresponding data file to reproduce the chart or to change which metrics are shown.

- Erling Haaland.jpeg  
  A shotmap showing Erling Haaland's shot locations and outcomes across the analysed match/season. Markers show the exact pitch positions for each attempt and are color-coded by result (goal, on-target, off-target), which gives a quick view of his most productive shooting zones. This plot helps identify preferred finishing areas and trends in positioning or shot selection. Re-run the generation script with filters (opponent, home/away) to explore situational patterns.

- Imaz i Pozo.jpeg  
  A comparative visualization (radar or bar chart) contrasting Imaz and Pozo on a set of offensive and defensive metrics. The chart includes normalized values for actions such as successful tackles, progressive carries, key passes and expected assists, allowing direct visual comparison despite differing raw scales. It is useful for assessing differences in style and contribution during the analysed period. To adapt the comparison, update the metric list in the data preprocessing step.

- Moder i Kairinen.jpeg  
  This chart focuses on creative and transitional metrics for Moder and Kairinen, showing attributes like key passes, progressive passes, successful dribbles and interceptions. The visualization emphasizes how each player contributes to build-up and chance creation rather than pure finishing. Comparing these metrics highlights differences in playmaking roles and defensive involvement. Use per-90 normalization to compare players with different minutes played.

- Pietuszewski and Bengtsson.jpeg  
  A comparative radar/heatmap that demonstrates role-specific performance between Pietuszewski and Bengtsson in the selected match or period. Metrics include positional involvement, passing accuracy in different thirds, duel success and chance creation. The chart helps reveal tactical responsibilities and where each player has most influence on the game. Consult the underlying event data to inspect individual actions behind peaks in the visualization.

- Pieńko and Fornalczyk.jpeg  
  A visualization centring on offensive involvement for Pieńko and Fornalczyk: passes into the final third, shot-creating actions, shots and assists. The chart shows volume and efficiency metrics so you can judge not only how often players attempt certain actions but also how successful they are. This is useful for comparing direct attacking impact and chance creation tendencies. Filter the dataset by match context to see changes under different tactical setups.

- radar 1  
  A general radar chart template used as a baseline for comparing two players across a configurable set of normalized statistics. Values are scaled between a common minimum and maximum so metrics with different natural ranges can be plotted together. This template is intended for quick visual comparisons and can be reused by swapping the data source or metric list. For reproducibility, include the normalization method and raw columns used in the README or nearby data docs.

Repository structure (example)
- images/ — visualization files (jpeg/png)  
- data/ — raw and processed data files (.csv, .json)  
- src/ — scripts that generate the charts and prepare data  
- docs/ — additional documentation and notes

Contact / Author  
Mirosław Kowalczyk  
GitHub: https://github.com/kowalczyk350

License  
Please add a LICENSE file (e.g., MIT) if you want to specify reuse terms.

Notes for the maintainer: replace `REPO-NAME` in the README clone URL with the actual repository name. Do not modify existing image/chart files. Add README only if README.md is missing or update/replace the existing README.md with this content if present.
