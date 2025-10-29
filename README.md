# wordlist_2048.txt

## Overview
`wordlist_2048.txt` contains 2,048 lowercase English words copied from the [EFF large word list](https://www.eff.org/files/2016/07/18/eff_large_wordlist.txt). The intent is to have a mnemonic-friendly corpus for general purposes that is unrelated to Bitcoin or BIP39 wallets. Using this independent list avoids any overlap with bitcoin seed phrases and removes even the minimum probability of collision or accidental reuse.

## Selection Rationale
- Exactly 2,048 entries, matching the size of common mnemonic sets but sourced exclusively from the EFF list.
- No edits or replacements beyond lowercasing and deduplicating; the words are purely extracted from the EFF data.
- Suitable for puzzles, gamified learning, or any mnemonic use case that should not reference Bitcoin infrastructure.

## File Structure
Each line uses the following format:

```
<binary_index> <word>
```

- `binary_index` is an 11-bit, zero-padded binary number (`00000000000` through `11111111111`).
- `word` is the corresponding alphabetic entry drawn from the source list.

Example:

```
00000000000 abide
00000000001 abiding
```

