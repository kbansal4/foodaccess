# Food Access Program Analysis

**Where should a food access program go?**

A side project built with public data (CDC 500 Cities + USDA Food Environment Atlas) that scores U.S. counties on food-access need and recommends where a county-level program would reach the most people.

### Live page

**[kbansal4.github.io/foodaccess](https://kbansal4.github.io/foodaccess)** - full write-up with interactive results.

### How it works

1. **Data** - CDC 500 Cities tract-level health data joined to USDA Food Environment Atlas county data on FIPS codes.
2. **Scoring model** - 15 variables weighted by priority: food-access demographics (12% each), population change (10%), health prevalence (5% each).
3. **County ranking** - tract-level health data aggregated up to counties, rescored, and ranked.
4. **Results** - Harris TX, Los Angeles CA, and Maricopa AZ top the list, with 750k+ people projected to benefit at a 45% engagement assumption.

### Files

- `index.html` - the project page
- `FoodAccessProgramAnalysis.ipynb` - the analysis notebook

Note: the notebook reads from `challenge.db` (SQLite), which isn't included here. It can be rebuilt from the two public sources linked above.

### Credits

By Kush Bansal - Side project, Spring 2025.
