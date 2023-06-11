# Gamebox-Product-Firmware-Updates
Repository of firmware update binaries for FPGA based Gamebox projects

## Directories
### GGHD
- FWUPD_GGHD_v1.3.2.mcs *to be released imminently - needs additional testing*
	> GGHD v1.3.2 Changelog
	> - Added 3 second delay to boot to allow time for Game Gear CPU boot strap process to finish.
	> 	this fixes boot issues on some problematic units in initial testing such as rainbow screen
	> 	of death, everdrive boot issues, and forced power cycle (unplug and plug back in)
	> - Backported most recent pixel filters

### 64HD
- FWUPD_64HD_v2.0.1.mcs - **11/06/2023**
	> 64HD v2.0.1 Changelog
	> - Codebase heavily refactored to drastically improve image stability and screen compatibility, especially for PAL region consoles
	> - 1080i flickering fixed (for screens that accept the 1080i signal)
	> - Toggling "Alt Audio" no longer resets HDMI stream
	> - N64 sound volume normalized before getting to HDMI output 
	> - OSD menu restructured
	> - New resolution 1024x768 added
	> - Filters removed due instability and timing issues causing unstable image output

- FWUPD_64HD_v1.7.3.mcs - **18/05/2023**
	> 64HD v1.7.3 Changelog
	> - Scaling option bugs in 240p and 480p reported by users have been addressed
	> - Filter options tweaked and now vertical bar issue on left and right of image have __actually__ been fixed/
		> __*IMPORTANT NOTE:*__ Due to a change in valid pixel ranges in the image filter core, those who have filter options on and saved in their current firmware version will see incorrect colors upon first boot of the updated firmware. Simply toggle the image brightness up or down to correct the colors in the image and save. This issue will not persist after this adjustment is done.

- FWUPD_64HD_v1.7.0.mcs - **16/05/2023**
	> 64HD v1.7.0 Changelog
	> - 1080i half screen bug fixed
	> - L/R Audio swap bug fixed
	> - 1280x800p video mode added
	> - Bilinear pixel filtering update - No more "cloudy" look. Bars on side of image when using filters reduced drasitcly
	> - Audio resampling core updated to reduce higher frequency and shrill sounding audio (more testers needed)

