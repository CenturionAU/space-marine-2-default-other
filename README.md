# README.md
## Client-side .sso Modification of Space Marine 2 PVE
All rights to Space Marine 2's developer, Saber Interactive. I am simply modifying the .sso files 
according to my preferences.

Modification of local files is not supported by Saber Interactive and doing so comes at one's own risk.

This repo serves as a means of storing and sharing my preferred modified values for Space Marine 2 and also to help me become more familiar with Git and GitHub.

---

### Installation Instructions
Big thanks to MegaDux for sharing this method.  
You will need to source your own EAC bypass.
1. Download WinRAR, if you don't already have it.
2. Right click Space Marine 2 on Steam > Manage > Browse local files.
3. Navigate to client_pc/root/paks/client/default/
4. Open default_other.pak using WinRAR.
5. At the top of WinRAR, select Options > Settings > Compression > Create default...  
    a. Change 'Compression method' to 'Store' using the drop down.  
    b. Select OK > OK.
6. Download the latest release from this GitHub repo.
7. Open the zip file using WinRAR.
8. Drag the ssl folder from the downloaded .zip into default_other.pak.
9. Select OK.

Enjoy your new values.

---

### Changelogs
#### v1.0.0
~ssl/damage/damagable/damage_points_restoring/damagable_health_restoring_library_pve.sso
- [[BUG REPORT]](https://github.com/CenturionAU/space-marine-2-modded-values/issues/1)
  Health injectors now fully restore the player's health.
- Executions now restore a small amount of player health, regardless of player contested health.
    - Common enemies restore 5% of health.
    - Elite and special enemies restore 10% of health.
    - Miniboss enemies restore 15% of health.
    - Boss enemies restore 20% of health.

~ssl/weapons/creator/firearm_library_pve.sso
- All player ranged weapons have had their spread reduced to 0.
- All player ranged weapons have had their damage increased by 100%.

~ssl/weapons/melee/weapon_descriptions/melee_weapon_descs/
- All player melee weapons have had the delay between attacks removed, meaning all player melee weapons
  now attack faster.
    - The speed of the individual attacks themselves remain the same but the player character no longer
      has a small delay in between each swing.
- All player melee weapons have had their damage increased by 100%.