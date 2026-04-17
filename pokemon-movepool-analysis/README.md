# Pokemon Move Pool Analysis

A data-driven analysis of move pool features across 847 Pokemon in 
Scarlet and Violet, examining how access to key competitive moves 
influences Smogon tier placement. Data was collected from PokeAPI 
and Smogon, building on the previous two projects in this series.

## Tools Used
- Python, pandas, matplotlib, seaborn
- Requests for API and web scraping
- Jupyter Notebook

## Data Sources
- PokeAPI (https://pokeapi.co/) for move pool data per Pokemon
- Smogon Strategy Pokedex (https://www.smogon.com/dex/sv/pokemon/) 
  for tier placements and move details

## Key Findings
- Recovery and setup moves are broadly available across all tiers 
  and are not reliable predictors of competitive viability
- Priority, pivot, and hazard moves are the key differentiators 
  in mid tier competitive play
- Coverage type diversity does not predict tier placement — Normal 
  types have the broadest move pools yet rank among the worst types
  competitively due to poor STAB utility
- Move pool features show surprisingly little correlation with 
  power score, suggesting stats and abilities outweigh move access 
  in determining raw competitive potential

## Limitations
- The 4 move slot constraint cannot be captured analytically — 
  a Pokemon may have access to every key move category but can 
  only use 4 moves per battle
- Move pool changes between generations mean historical data may 
  not reflect current competitive viability accurately
- Team synergy, matchup knowledge, and opponent prediction are 
  irreducible human factors that data cannot measure

## Conclusions

This analysis completes a three project series examining competitive 
Pokemon viability through progressively deeper lenses — base stats, 
Smogon tier placement, and now move pools.

The most surprising finding is how little move pool access alone 
predicts competitive success. After 30 years and 9 generations, moves 
that were once exclusive to certain Pokemon have been distributed 
broadly across the roster through TMs, TRs, and move tutors. The 
exclusivity that once made certain Pokemon irreplaceable has been 
largely removed — making team building more flexible and accessible 
than ever before.

This democratization of move pools has shifted the competitive 
meta toward stats, abilities, and typing as the primary determinants 
of viability. A Pokemon with a powerful ability and strong offensive 
stats will outperform a Pokemon with a diverse move pool but mediocre 
stats in almost every matchup.

The 4 move slot constraint remains the hidden variable that no data 
analysis can fully capture. A Pokemon may have access to recovery, 
setup, priority, hazards, and pivot moves simultaneously — but must 
choose only 4. The art of competitive Pokemon lies in making those 4 
choices correctly for every situation, something that requires 30 years 
of accumulated human knowledge that no dataset can replicate.

## Future Work
Future analysis could incorporate generational move history to track 
how specific move additions and removals have impacted tier placement 
over time, quantifying the competitive impact of game freak's 
balancing decisions across generations.

## Previous Projects
- Project 1: Pokemon Competitive Viability Analysis — Base stat analysis
- Project 2: Pokemon Competitive Viability — Smogon Tier Analysis
