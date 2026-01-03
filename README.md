# PG3DToolkit

English / [日本語](README_ja.md)

```
Due to burnout, there is no guarantee that issues will be fixed or improvements made. I have lost enthusiasm for this game.
```

**A web-based tool to convert Minecraft skins into PG3D-compatible skins and bulk-import them into the game.**

- _Currently Windows only._

## Usage

1. Obtain a skin commonly used in Minecraft.
   - 64x64 skins are recommended. 64x32 skins have not been verified.
2. Accsess to https://mofixy.github.io/PG3DToolkit/
3. Select all skins obtained via the file input.
4. Click the `generate` button to download a .reg file.
5. Adjust options as needed.
6. Double-click the .reg file and follow the instructions to modify the registry.
7. Verify the result in the game.

## Options

_All options can be previewed using the `preview` button to see what changes will be made._

- `Automatic skin processing`
  - Enables automatic skin processing. When turned off, only conversion from 64x64 to 64x32 and arm width adjustment from 3px to 4px are performed.
- `Flip the top face of the arms on the X-axis`
  - Flips the image for the shoulder area of the skin.
  - Because PG3D's UVs are unusual, turning this off may make shadows face outward.
- `Remove dots that overwrite the eyeliner in the layer`
  - Removes some dots that overwrite the eyeliner on the layer side.
  - For typical avatar-style skins, enabling this improves the appearance; for some avatar or special skins, disabling is recommended.
- `Skip overwriting all layer textures`
- `Skip overwriting the *** layer`
  - Skip overwriting all or part of the layer textures.
  - Generally leaving these off produces a better appearance, but they may be unsuitable for some skins.

## Known Issues

- Importing currently overwrites existing skins rather than adding new entries.
  - ⚠ If you already have non-server-stored skins in the game, they will be overwritten. No support will be provided for overwritten skins! ⚠
- Per-skin option settings are not supported.
- Naming skins is not supported.
- The `Automatic skin processing` option does not fully disable processing.
- Left/right texture usage settings are not functioning.

If you encounter other issues, please report them via issues.

## Improvements

```
There is no guarantee these will be implemented. Consider them ideas only.
I hope someone will take over this project.
```

- UI improvements
- Skin preview within the UI
- Per-skin individual options
- Per-skin naming
- Implement left/right texture usage settings for arms and legs
- Import from registry data
- Export imported data as images
- Add various exception handling
- Improve skin ID (snowflake)
- Support for 64x32 skins
