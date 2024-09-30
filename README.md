# space-marine-2-default-other

## Client-side SSL Modification of Space Marine 2 PVE
All rights to Space Marine 2's developer, Saber Interactive, I am simply modifying the .sso files 
according to my preferences.

Modification of local files is not supported by Saber Interactive and doing so comes at one's own risk.


### Initial Repo Creation
This repo was created from the base files within default_other.pak of Space Marine 2's local files. 
An initial modification of ~ssl/main/user/progressiona/weapons_mastery/perks/weapon_perks_progression_library.sso
by @RumpleForskin is included which removes the perk exclusivity lockouts, allowing the selection of all perks 
within a weapon's perk tree assuming there are enough perk points.


### Health Restoration
~ssl/damage/damagable/damage_points_restoring/damagable_health_restoring_library_pve.sso

#### Changelogs
Stim Injectors fully restore health regardless of player's health value which also cures any mortal wounds.  
Executions restore a small amount of player health, regardless of contested health state.

| Line | Variable | Original Value | Modified Value |
|------|----------|----------------|----------------|
