# pokemon-competitive-analysis
An exploratory data analysis of all 1,025 Pokémon across Generations 1-9, investigating what base stats best predict competitive viability. Data was collected from the PokeAPI and analyzed using Python and pandas, featuring a custom Power Score metric to rank Pokémon by raw competitive potential.

## Tools Used
- Python, pandas, matplotlib, seaborn
- PokeAPI for data collection
- Jupyter Notebook

## Key Findings
- Offensive stats correlate most strongly with competitive viability
- Dragon types lead all types in average power score
- Power score reliably identifies competitive archetypes
- Stats are a ceiling not a guarantee

# Conclusions: What Makes a Pokemon Competitively Viable?

## Key Findings

**1. Offensive stats are the strongest predictor of viability**
Special Attack and Attack correlate most strongly with power score, 
followed closely by Speed. Defense correlates least, confirming that 
competitive Pokemon favor hitting fast and hard over absorbing damage.

**2. Dragon types lead all types in average power score**
However this is heavily influenced by the high concentration of 
Legendary and Pseudo-Legendary Pokemon within the type. Type alone 
is not a pure indicator of strength — sample composition matters.

**3. Power score reliably identifies competitive archetypes**
Every Pokemon in the top 20 outside of Slaking and Archeops has a 
legitimate competitive reputation, Pseudo-Legendaries, Ultra Beasts, 
and Paradox Pokemon all appear exactly where expected.

**4. Stats are a ceiling, not a guarantee**
Slaking and Archeops demonstrate that restrictive abilities can 
completely nullify elite base stats. Power score should be interpreted 
as a measure of raw potential, not guaranteed performance.

## Limitations & Future Work
- Abilities, move pools, and type matchups were not factored into 
  this analysis and are equally critical to competitive viability
- A future iteration could incorporate Smogon tier data to validate 
  power score against real competitive usage
- Team synergy and meta trends are impossible to capture through 
  base stats alone

## Final Takeaway
Base stats are the foundation of competitive viability but not the 
whole story. A Pokemon needs strong offensive stats and speed to 
compete, but without a functional ability and viable move pool, 
even the highest power score means nothing. Slaking proves that 
better than any chart could.

## Data Source
Data collected via [PokeAPI](https://pokeapi.co/)
