# PIP-CO Startup Systems

A custom startup selector for The Wand Company Pip-Boy 3000.

This public modular build preserves the hardware-tested V84 startup, menu, audio, and playback behavior while using the normal pip-boy.com metadata installation path for MISC registration.

## Startup Choices

### Special Bootups

- Mister Handy
- Vault Girl
- Deathclaw Vault Experiment
- Enclave PIP-BOY

### Faction Bootups

- The Enclave
- The Brotherhood of Steel
- The Minutemen
- Mothman

### NPC Bootups

- YES MAN

### Default Bootup

Restores the normal stock Pip-Boy startup sequence.

## Controls

- **Left wheel:** Move through the menu
- **Left wheel press:** Select
- **< Back:** Return to the previous menu

## Startup Selection

The selected startup is stored in:

`HOLO/STARTUP_ANIMATIONS/SELECT.JSON`

The selected startup remains active after leaving the holotape and is used on subsequent Pip-Boy startup/wake sequences.

Selecting **Default Bootup** restores the stock startup behavior.

## Modular Startup Packs

For a custom startup to appear in the menu, both its AVI and WAV files must be installed.

If either file is missing, that startup is automatically hidden from the menu.

This allows users to install only the startup packs they want instead of installing every available animation and audio file.

## Compatibility and Stability

The current runtime is based on the V84 hardware-tested startup implementation.

The cleanup removes legacy `global.__SA*` / `global.__startupAnimations*` state while preserving the startup timing, audio suppression, menu behavior, and repeated-boot stability verified on The Wand Company Pip-Boy 3000.

## Version

Current public feature update:

**v1.1.0**
