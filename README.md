# README.md
## Client-side .sso Modification of Space Marine 2 PVE
All rights to Space Marine 2's developer, Saber Interactive. I am simply modifying the .sso files 
according to my preferences.

Modification of local files is not supported by Saber Interactive and doing so comes at one's own risk.

This repo serves as a means of storing and sharing my preferred modified values for Space Marine 2 and also to help me become more familiar with Git and GitHub.

---

### Specific Changes
- All player ranged weapons do 2x damage.
- All player ranged weapons have no spread.
- All player melee weapons do 2x damage.
- All player melee weapons have zero delay between each attack in their combo, resulting in master melee
  attacks.
- Executions restore a percentage of player health regardless of contested health.

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

You should then be able to launch your game with these modified values.