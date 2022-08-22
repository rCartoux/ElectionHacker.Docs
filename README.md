# ElectionHacker.Docs

Shield: [![CC BY 4.0][cc-by-shield]][cc-by]

This work is licensed under a
[Creative Commons Attribution 4.0 International License][cc-by].

[![CC BY 4.0][cc-by-image]][cc-by]

[cc-by]: http://creativecommons.org/licenses/by/4.0/
[cc-by-image]: https://i.creativecommons.org/l/by/4.0/88x31.png
[cc-by-shield]: https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg

## Definitions

| Notation | Meaning|
|-|-|
| $V = \lbrace v_1, v_2,..., v_n \rbrace$ | Set of voters|
| $C = \lbrace c_1, c_2,..., c_m \rbrace$ | Set of candidates|
|$c_i \geqslant_v c_j$ | Voter $v$ prefers $c_i$ over $c_j$. Non-strict preferences|
|$C_v \subset C$| Subset of candidates which are approved by voter $v$|


We describe the voter opinions about candidates by a score function $s_v : C \rightarrow  [0, 1]$
Each voter has its own approval threshold $a_v$. All candidates whose score is larger or equal to the voter approval threshold are approved by voter $v$.

## Ballots

### Ordinal

Candidates are ranked in descending order of preferrence. The candidate with the highest score should be first on ranked ballot (if the voter is sincere) 

Variants:
- Ties allowed / forbidden.
- Number of ranks limited to a fix number / unlimited (equal to the number of candidates)
- Approval threshold fixed to a given rank / freely defined by the voter.

### Cardinal

Voter give directly their score for each candidate in the ballot, on a $[0,10]$ or $[0,100]$ range for example.

Variants:
- Approval threshold fixed to a given score / freely defined by the voter.

Score ballot with free approval threshold would allow a direct transposition of the voter score function $s_v$ and approval threshold $a_v$


## Approval and majority pairwise sorting

Let us consider a ranked ballot with fixed approval threshold (candidate with rank 2 or higher is considered approved) and with limited maximal rank (5).

Approval and majority pairwise sorting (AMPS) algorithm.






