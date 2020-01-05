# PokemonGen8IVCalculator
 IV Calculation library from Pokemon Gen 8.

## Adapted from
[LegendaryPKMN/ivcalc](https://github.com/LegendaryPKMN/ivcalc)

## Example Use

```cs
decimal pokemonID = IVCalculator.PokemonDictionary["Charmeleon"];
string nature = "Bashful";
string character = "Likes to thrash about";
List<int> knownStats = new List<int>() { 236, 164, 130, 175, 143, 196 };
List<int> EVs = new List<int>() { 0, 0, 0, 0, 0, 0 };
int dexID = IVCalculator.getPokemonIndex(pokemonID);
int level = 100;

IVCalculator.getIVs(dexID, level, nature, character, knownStats, EVs)
```