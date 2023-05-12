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
- FWUPD_64HD_v1.7.0.mcs *to be released imminently - needs additional testing*
	> 64HD v1.7.0 Changelog
	> - 1080i half screen bug fixed
	> - L/R Audio swap bug fixed
	> - 1280x800 video mode added
	> - Audio resampling core updated to reduce higher frequency and shrill sounding audio (needs testing) 

