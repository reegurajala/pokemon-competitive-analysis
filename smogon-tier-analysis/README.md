# Smogon Tier Analysis

A data-driven analysis of 848 Pokemon across all Smogon competitive 
tiers, combining PokeAPI stat data with live Smogon tier placements. 
Built a custom web scraper to collect and merge data from two sources, 
exploring how base stats, abilities, and typing influence competitive 
tier placement.

## Tools Used
- Python, pandas, matplotlib, seaborn
- Requests, BeautifulSoup for web scraping
- Jupyter Notebook

## Data Sources
- PokeAPI (https://pokeapi.co/) for base stats and legendary flags
- Smogon Strategy Pokedex (https://www.smogon.com/dex/sv/pokemon/) 
  for tier placements and ability data

## Key Findings
- Power score generally decreases from AG down to LC, confirming 
  stats correlate with tier placement at the extremes
- Between OU and NUBL the relationship becomes inconsistent, 
  suggesting abilities and typing play a larger role in mid tiers
- Water dominates regular competitive play due to defensive utility
- Protosynthesis and Quark Drive emerge as the most common abilities 
  in top tiers among regular Pokemon, highlighting Generation 9's 
  impact on the competitive landscape
- Bug, Ice, and Normal are the weakest types in top tier play despite 
  having strong offensive moves

## Limitations
- Move pool data was not included and remains a significant factor 
  in competitive viability
- 10 Pokemon could not be matched between datasets due to naming 
  inconsistencies between PokeAPI and Smogon
- Tier placements reflect a snapshot in time and shift regularly 
  as the meta evolves
- Team synergy and matchup specific factors cannot be captured 
  through individual Pokemon data alone

## Conclusions

This analysis builds directly on the findings of the previous Pokemon 
Competitive Viability project, and broadly confirms that base stats 
are a reliable indicator of competitive strength at the extremes, 
but the story becomes far more complex in the middle tiers.

Typing proved to be a critical factor in determining viability. Types 
are only as good as what they resist, not just what they hit. Water 
dominates regular competitive play due to its defensive utility, while 
types like Ice and Electric, despite having excellent offensive moves, 
are held back by the fragility of the Pokemon that carry them.

Abilities emerged as perhaps the most decisive factor separating tiers 
in the mid range. Generation 9's Paradox Pokemon demonstrate this most 
clearly, with Protosynthesis and Quark Drive directly amplifying already 
strong stats, creating a class of Regular Pokemon that rival Legendaries 
in competitive viability. Conversely, abilities like Truant and Defeatist 
can render elite base stats completely useless.

Finally this analysis surfaces a broader competitive truth, powercreep 
is real. Older Pokemon that were once considered elite are increasingly 
being pushed down tiers as newer generations introduce stronger entries 
with better stat spreads, superior typing combinations, and more powerful 
abilities. Competitive viability is not static, it evolves with every 
new generation.

## Future Work
A third project will focus specifically on move pool analysis, examining 
how access to certain moves influences tier placement independent of base 
stats and abilities. This will complete the picture of what truly makes 
a Pokemon competitively viable.
