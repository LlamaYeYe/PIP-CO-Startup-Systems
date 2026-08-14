PIP-CO Startup Systems v1.1.0 - Full Modular Installer Package

Core files:
- app.min.js -> HOLO/STARTUP_ANIMATIONS/APP.JS
- assets/SELECT.JSON -> HOLO/STARTUP_ANIMATIONS/SELECT.JSON
- assets/TITLE.BIN -> HOLO/STARTUP_ANIMATIONS/TITLE.BIN

Optional startup packs (install any combination):
- Mister Handy
- Vault Girl
- Deathclaw Vault Experiment
- YES MAN
- Mr. House
- The Enclave
- The Brotherhood of Steel
- Mothman
- The Minutemen
- Enclave PIP-BOY

Playback baseline:
- Mister Handy, Vault Girl, Deathclaw, YES MAN, and Minutemen use videoStopped as normal completion.
- Natural completion does not redundantly call Pip.videoStop()/Pip.audioStop().
- A generous hard failsafe remains for stuck playback.
- Mr. House preserves its existing working timed behavior.
- No AudioSafe wrappers or runtime APPINFO self-registration.

This bundle is installer-focused and self-contained; repository-only preview/icon/readme references are intentionally omitted from metadata.json.
