# Rock Band Blitz Stage 1 Last Ditch

> One final theoretical Rock Band Blitz Stage 1 patch hack shenanigan that needs to be confirmed impossible.

This repository is a small research/workbench project for one very specific question:

**Can the existing Rock Band Blitz BadUpdate Stage 1 binary be patched for a different Xbox 360 dashboard without having the original tools/source used to build it?**

Probably not.

But "probably not" has been bothering me enough that I'm giving it one final attempt.

## Progress:

* [x] Extract Stage 1 from `songs.dta`
* [ ] Document its offset, size, and alignment inside `songs.dta`
* [x] Compare its structure against Stage 1 implementations with available source
* [x] Identify any dashboard-specific values
* [x] Determine whether those values can be patched for 17526
* [x] Reinsert the patched binary and perform an initial test
* [x] See whether Rock Band Blitz reaches the “Running Exploit” screen


# current ramblings:

value should be: str(hex_address as signed int32)  ?

0x817247c8 -> str(0x817247c8 - 0x100000000) = '-2126659640'
