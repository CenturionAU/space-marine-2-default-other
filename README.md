# README.md
## Client-side SSL Modification of Space Marine 2 PVE
All rights to Space Marine 2's developer, Saber Interactive. I am simply modifying the .sso files 
according to my preferences.

Modification of local files is not supported by Saber Interactive and doing so comes at one's own risk.

---

### Initial Repo Creation
This repo was created from the base files within default_other.pak of Space Marine 2's local files. 
An initial modification of ~ssl/main/user/progressiona/weapons_mastery/perks/weapon_perks_progression_library.sso
by @RumpleForskin is included which removes the perk exclusivity lockouts, allowing the selection of all perks 
within a weapon's perk tree assuming there are enough perk points.

***

### Health Restoration
~ssl/damage/damagable/damage_points_restoring/damagable_health_restoring_library_pve.sso

#### Changelogs
- Stim Injectors fully restore health regardless of player's health value which also cures any mortal wounds.  
- Executions restore a small amount of player health, regardless of contested health state.
    - Common enemies restore 5% health.
    - Elite enemies restore 10% health.
    - Special enemies restore 10% health.
    - Miniboss enemies restore 15% health.
    - Boss enemies restore 20% health.

#### Changelog Table
| Line | Variable | Original Value | Previous Modified Value | Modified Value |
|------|----------|----------------|-------------------------|----------------|
| 399 | healthRestoringPercent | 35 |   | 100 |
| 291 | healthRegenPercentByKill | 0 |   | 5 |
| 298 | healthRegenPercentByKill | 0 |   | 10 |
| 308 | healthRegenPercentByKill | 0 |   | 10 |
| 318 | healthRegenPercentByKill | 0 |   | 15 |
| 325 | healthRegenPercentByKill | 0 |   | 20 |

___

### Ranged Weapons
~ssl/weapons/creator/fire_library_pve.sso

#### Changelogs
- All ranged weapons have had their spread reduced to 0.

### Changelog Table
| Line | Variable | Original Value | Previous Modified Value | Modified Value |
|------|----------|----------------|-------------------------|----------------|
| 153 | minBulletSpread | 0.22 |   | 0.00 |
| 154 | maxBulletSpread | 2.1 |   | 0.0 |
| 168 | spline | 0, 1, 30, 25, 60, 28, 100, 22 |   | 0, 0, 00, 00, 00, 00, 000, 00 |