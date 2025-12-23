# Overview

This folder contains scripts to generate and update the patch.

When applying the patch in PAZ folder, "Meta Injector.exe" may reports that patching to some .pac files have failed.
This is an indicator that the patch in PAZ folder is not compatible with the the game binaries any more due to game
content update. Usually, these errors/fails can be fixed by regenerate the patch using the latest game client:

  1. Run [setupenv.cmd](../setupenv.cmd) to open the dev console.
  2. Run the following commands in the dev console:

    run.cmd -i <full_path_to_the_PAZ_folder_of_your_bdo_game> -o .\PAZ\midnight_xyzw -m all

If you still see patch failures after this, then it is probably due to incompatibilities of my mod collection to the
latest game. Try delete mods in [PAZ/midnight_xyzw/_01_xyzw_collections](../PAZ/midnight_xyzw/_01_xyzw_collections) one
by oen to find out which one causes issue.

# Class ID

## Female

| Class | IDs |
| - | - |
| 2_PHW | Sorceress |
| 3_PEW | Ranger |
| 5_PBW | Tamer |
| 7_PVW | Valkyrie |
| 8_PWW | Witch |
| 11_PGW | Guardian |
| 12_PKW | Old Maehwa (Some early Maewha outfits/underwear use this) |
| 13_PNW | Kunoichi |
| 14_PLW | Shai |
| 15_PDW | Dark Knight |
| 16_PCW | Mystic |
| 17_PSW | Lahn |
| 21_PPW | Nova |
| 22_PKWW | Maehwa |
| 24_PFW | Corsair |
| 25_PQW | Drakania |
| 27_PKOW | Maegu |
| 28_PMYF | Woosa |
| 29_PNYW | Scholar |
| 32_PWGE | Deadeye |
| 33_PDKL | Seraph | 

## Male

| Class | IDs |
| - | - |
| 1_PHM | Warrior |
| 4_PGB | Berzerker (Beast Form) |
| 4_PGM | Berzerker |
| 6_PKM | Musa |
| 7_PVM | Valkyrie |
| 8_PWM | Old Wizard |
| 8_PWMM | Revamped Wizard |
| 9_PEM | Archer |
| 13_PNM | Ninja |
| 16_PCM | Striker |
| 18_PAM | Hashashin |
| 23_PPM | Sage |

# Outfit Types 

| ID | Desc |
| - | - |
| _00 | class specific pearl shop outfits |
| _02 and 03 | armors/Honor outfits |
| _10 | outfits shared by many/all classes |
| _50 | craftable outfits (Serendia Soldier,etc) |
| _bw /_kw, etc | usualy cosplay or outfits from a diff class (they use class IDs without P) |
