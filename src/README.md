# How to generate/update the patch.

When applying the patch in PAZ folder, "Meta Injector.exe" may reports that patching to some .pac files have failed.
This is an indicator that the patch in PAZ folder is not compatible with the the game binaries any more due to game
content update. Usually, these errors/fails can be fixed by regenerate the patch using the latest game client:

  1. Run [setupenv.cmd](../setupenv.cmd) to open the dev console.
  2. Run the following commands in the dev console:

    run.cmd -i <full_path_to_the_PAZ_folder_of_your_bdo_game> -o .\PAZ\midnight_xyzw -m all

If you still see patch failures after this, then it is probably due to incompatibilities of my mod collection to the
latest game. Try delete mods in [PAZ/midnight_xyzw/_01_xyzw_collections](../PAZ/midnight_xyzw/_01_xyzw_collections) one
by oen to find out which one causes issue.
