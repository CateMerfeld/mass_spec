# README

This CSV file contains contains data for 572 chemical samples. Each sample has a unique mass spectrum, the Chemception embedding for that chemical, and condition information for the sample/chemical.

## File Structure

- **data_for_randy.csv**: Main CSV file containing chemical data.


## Columns

| Column Name    | Description                          |
|----------------|--------------------------------------|
| 0 - 914        | Mass Spectrum                        |
| 915 - 1426     | Chemception embedding                |
| 1427 - 1431    | Condition - Number of carbon rings   |
| 1432           | Condition - Contains a chain         |

## Data Format

- "Number of carbon rings" is one-hot-encoded: zero carbon rings is [0,0,0,0,0], three carbon rings is [0,0,0,1,0], etc.
- "Contains a chain" [0] indicates no chain, [1] indicates a chain. 