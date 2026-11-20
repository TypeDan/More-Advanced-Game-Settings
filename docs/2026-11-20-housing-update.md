# Version 2026.11.20.1

Custom population limits now set the maximum without granting housing. The previous OnPlay fixed-cap override made a 250 limit immediately usable without houses. The code clears that override and retains the maximum-population modifier. Team population transfers also preserve housing. Restore callbacks clear the override without applying the maximum modifier twice. Mongols retain their civilization's housing exception, and an explicit minimum-population setting still applies.

Validation on 20 November 2026:

- Automated checks passed for all eight lobby slots in reversed internal player order, independent housing and ceiling values, global and individual limits, house gains/losses, maximum clamping, Mongols, repeated initialization/restore callbacks and team population transfers.
- Player settings and bonus-HUD regression checks passed in both repositories.
- A native Yuletide match used Knights Templar in host slot 1, Abbasids in slot 2 and HRE in slot 3, each configured for 250. All started with 10 housing capacity and a reported maximum of 250.
- A temporary diagnostic gave sufficient housing to all three players: usable capacity stopped at 250. Removing it restored their natural housing (10 for the idle host, 20 for the AIs which had built houses).
- Building a normal house as the host raised the native display from 7/10 to 7/20 while the maximum remained 250.
- The diagnostic overlay, temporary housing and test tokens are excluded from the production archive.

The native match validates the shared population code used in both mods. It is not a full multiplayer or saved-game compatibility test; start a new match with the updated mod.

Both final native Content Editor builds completed with zero errors and warnings. Archive inspection confirmed production source matches, mod metadata and all expected files; no housing diagnostic remains.

Published through the native AoE IV publisher as [More Advanced Game Settings 593850](https://www.ageofempires.com/mods/details/593850/). A fresh subscription download matched the production archive byte-for-byte: SHA256 `33b2b3f9277f43744486d0ef980f531795de203b25eea5b0da024239b8562459`. The superseded listing 593824 was deleted after that verification. Previous subscribers need the new listing.
