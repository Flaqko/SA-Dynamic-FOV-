# Dynamic FOV Redux v1.0

CLEO Redux port/remaster of **Dynamic FOV v1.1** by **Junior_Djjr** for **Grand Theft Auto: San Andreas Classic PC 1.0**.

Redux port/remaster by **Flaqko**.

## What it does

Dynamically adjusts the gameplay field of view based on the camera's vertical angle. Looking up/down changes the FOV smoothly while preserving the original mod's camera-mode restrictions and native weapon zoom behavior.

This v1.0 release is based directly on the user-confirmed working v0.1 TEST build. Gameplay logic is unchanged.

## Installation

Copy the included `CLEO` folder into your GTA San Andreas installation folder and merge when prompted.

The installed path should be:

`CLEO/DynamicFOV[fs][mem]/`

CLEO Redux uses the `[fs][mem]` suffix to grant the script the permissions it needs for INI access and the small camera-state memory reads used by the original behavior.

## Configuration

Edit `DynamicFOV.ini`:

```ini
[Module]
Enabled = 1
Debug = 0

[Settings]
FOV = 70.0
Speed = 0.1
DynamicIntensity = 0.8
DynamicIntensityDown = 1.0
```

- `Enabled` — enables/disables the mod.
- `Debug` — enables extra CLEO Redux log output.
- `FOV` — base/default FOV.
- `Speed` — smoothing speed.
- `DynamicIntensity` — main dynamic FOV strength.
- `DynamicIntensityDown` — additional response while looking downward.

## Compatibility behavior

The script intentionally avoids unsupported camera modes, loaded cutscenes, and native weapon/camera zoom interpolation so it does not fight GTA SA's own zoom behavior.

## Requirements

- Grand Theft Auto: San Andreas Classic PC 1.0
- CLEO Redux

## Credits

- Original Dynamic FOV v1.1: **Junior_Djjr**
- CLEO Redux port/remaster: **Flaqko**
