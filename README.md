# README.md
## Client-side SSL Modification of Space Marine 2 PVE
All rights to Space Marine 2's developer, Saber Interactive. I am simply modifying the .sso files 
according to my preferences.

Modification of local files is not supported by Saber Interactive and doing so comes at one's own risk.

---

### Changelogs
#### 30-Sep-2024
~ssl/damage/damagable/damage_points_restoring/damagable_health_restoring_library_pve.sso
- Health injectors now fully restore the player's health.
- Executions now restore a small amount of player health, regardless of player contested health.
    - Common enemies restore 5% of health.
    - Elite and special enemies restore 10% of health.
    - Miniboss enemies restore 15% of health.
    - Boss enemies restore 20% of health.

~ssl/weapons/creator/firearm_library_pve.sso
- All player ranged weapons have had their spread reduced to 0.

~ssl/weapons/melee/weapon_descriptions/melee_weapon_descs/
- All player melee weapons have had the delay between attack removed, meaning all player melee weapons 
now attack faster.
    - The speed of the individual attacks themselves remain the same but the player character no longer
    has a small delay in between each swing.