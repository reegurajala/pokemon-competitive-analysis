# Pokemon Competitive Viability — A Three-Part Analysis

A three-part data-driven series examining what makes a Pokemon competitively viable, 
progressing from raw base stats through Smogon tier placement to move pool access. 
Data collected from PokeAPI and Smogon, analyzed using Python and pandas across 
848-1,025 Pokemon depending on the project scope.

## The Series

| Project | Focus | Pokemon Analyzed |
|---|---|---|
| [Part 1 — Base Stat Analysis](#) | Custom Power Score metric, stat correlations | 1,025 (Gen 1-9) |
| [Part 2 — Smogon Tier Analysis](#) | Tier placement, abilities, typing | 848 |
| [Part 3 — Move Pool Analysis](#) | Move access, competitive move categories | 847 |

## Tools Used
- Python, pandas, matplotlib, seaborn
- Requests, BeautifulSoup for web scraping
- Jupyter Notebook

## Data Sources
- [PokeAPI](https://pokeapi.co/) — base stats, move pools, legendary flags
- [Smogon Strategy Pokedex](https://www.smogon.com/dex/sv/pokemon/) — tier placements, 
  ability data, move details

---

## Key Findings Across the Series

**Stats are a ceiling, not a guarantee**
Base stats correlate strongly with competitive viability at the extremes — 
the top and bottom tiers align closely with Power Score. But between OU and 
NUBL the relationship breaks down, and Slaking and Archeops demonstrate that 
a restrictive ability can completely nullify elite stats.

**Abilities are the decisive factor in the mid tiers**
Generation 9's Paradox Pokemon make this clearest. Protosynthesis and Quark 
Drive directly amplify already strong stats, producing Regular Pokemon that 
rival Legendaries. Conversely, Truant and Defeatist render top-tier stat 
spreads competitively useless.

**Move pool access is no longer a differentiator**
After 30 years of TMs, TRs, and move tutors, most competitive moves are 
broadly distributed. Recovery and setup are available across all tiers. 
Priority, pivot, and hazard moves are the remaining differentiators, but 
even these are far less exclusive than they once were. Stats and abilities 
now outweigh move access in determining viability.

**Typing is about what you resist, not just what you hit**
Water dominates regular competitive play due to defensive utility. Bug, Ice, 
and Normal have strong offensive moves but rank among the weakest types 
competitively — held back by poor STAB utility or the fragility of the 
Pokemon that carry them.

**Powercreep is real and measurable**
Older Pokemon once considered elite are being pushed down tiers as newer 
generations introduce stronger entries with better stat spreads, superior 
typing, and more powerful abilities. Competitive viability is not static.

---

## Overarching Conclusion

Across all three projects, a consistent picture emerges: **the formula for 
competitive viability is strong offensive stats + speed + a functional ability 
+ access to at least one of priority, pivot, or hazard moves**. No single 
factor is sufficient alone.

The hidden variable that no dataset can fully capture is the 4 move slot 
constraint. A Pokemon may have access to every key move category simultaneously 
but can only bring 4 moves into battle. The art of competitive Pokemon — 
predicting opponents, building for synergy, adapting to the meta — is 30 years 
of accumulated human knowledge that sits entirely outside the data.

---

## Limitations Across the Series
- Team synergy, matchup prediction, and meta trends cannot be captured 
  through individual Pokemon data alone
- Tier placements reflect a snapshot in time and shift with every new generation
- The 4 move slot constraint is analytically irreducible
- 10 Pokemon could not be matched between datasets due to naming inconsistencies 
  between PokeAPI and Smogon

## Future Work
Future analysis could incorporate generational move history to track how 
specific move additions and removals have impacted tier placement over time, 
quantifying the competitive impact of Game Freak's balancing decisions across 
generations. A natural extension would also be validating Power Score directly 
against Smogon usage statistics rather than tier placement alone.
