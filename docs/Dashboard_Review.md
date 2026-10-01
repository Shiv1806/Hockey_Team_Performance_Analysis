# Final Power BI Dashboard Review

## Final dashboard components

The supplied final PBIX contains:

- 8 KPI cards
- 2 interactive slicers
- 1 Performance Category pie chart
- 1 Average Win % by Team bar chart
- 1 Goal Differential vs Average Win % scatter chart
- 1 Goals For vs Goals Against combination chart
- 1 Total Goals Scored vs Average Win % combination chart

## Aggregation choices reviewed

### Correct analytical choices

- Win % comparisons use **Average**
- Goals For / Goals Against KPI cards use **Average**
- Goal Differential KPI uses **Average**
- Maximum Win % uses **Maximum**
- Wins and Losses use **Sum**
- Performance Category uses team count

### Small final polish recommendation

The KPI currently labelled **"Goals Differential"** is calculated using an average aggregation. For clarity, rename the displayed label to:

**Average Goal Differential**

This makes the card's label match its aggregation and avoids ambiguity.

### Future-proofing recommendation

The current dataset contains 25 records and 25 unique team names, so the current Team count is appropriate for this dataset.

If the project is later expanded to multiple rows per team across many seasons, use **Distinct Count of Team Name** for the Total Teams KPI so that teams are not counted repeatedly.

These are presentation/future-proofing points rather than evidence that the current dashboard is incorrect.
