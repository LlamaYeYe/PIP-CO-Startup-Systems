Description


* Updates PIP-CO Startup Systems to v1.1.0 with modular optional startup-pack installation support.

* Users can install only the startup animations they want. Each startup AVI contains its matching audio, and the holotape automatically shows only the startup options whose AVI is installed.

* The latest update also improves completion handling for the remade startup animations. Mister Handy, Vault Girl, Deathclaw, YES MAN, and The Minutemen now use videoStopped as their normal completion event, preventing unnecessary stop calls after playback has already completed. A generous hard failsafe remains for genuinely stuck playback.

* Update Checklist

* Added modular optional startup media support
* Embedded matching startup audio directly into each AVI
* Removed separate startup WAV dependencies
* Added YES MAN
* Added Mr. House
* Added The Enclave
* Added Enclave PIP-BOY startup
* Added The Brotherhood of Steel
* Added Mothman
* Added The Minutemen
* Preserved Mister Handy, Vault Girl, and Deathclaw
* Added TITLE.BIN
* Updated startup menu/core files
* Updated metadata to use AVI-only storageOptional startup packs
* Preserved the existing holotape ID and preview
* Tested on the Wand Company Pip-Boy 3000

Cleanup Check

* App exits without requiring a reboot
* App reopens normally after use
* Startup media is only loaded when needed
* Installed startup AVIs are detected dynamically
* Missing optional startup packs are hidden from the startup menu
* No separate startup WAV files are required
* Startup audio plays from the installed AVI itself
* Memory-conscious startup behavior is preserved
* Existing startup selections remain compatible
* No runtime APPINFO self-registration is used
* No audioStop wrapper
* No audioStartVar wrapper
* No playSound wrapper
* No protected-startup wrapper state
* No heavy crash/memory logging
* No re-open wrapper cleanup experiment
