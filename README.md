# Adventure Quest - Unity 3D Gameplay Prototype

This project contains a complete Unity 3D game flow for:

- Main Menu
- Instructions panel
- Character Selection
- Level Selection
- Level 1 - Easy Mode
- Level 2 - Hard Mode
- Game Over
- Victory

Open the project in Unity `6000.3.15f1` or newer and start from `Assets/Scenes/MainMenu.unity`.

## Controls

- Move: `WASD` or arrow keys
- Jump: `Space`
- Look: mouse movement
- Attack: right mouse button

## Implemented Gameplay

- First-person movement with the Unity New Input System
- Mouse look, jumping, enclosed 3D arenas, lighting, and generated materials
- Three lives in Level 1, two lives in Level 2
- Respawn after life loss until lives reach zero
- Score, lives, timer, and objective HUD
- Gold coins and blue energy orbs
- Moving enemies that chase and attack the player
- Right-click attack mechanic with combat audio
- Enemies fall to the ground briefly, disappear, and increment the in-game kill counter
- Boss enemy in Level 2
- Victory condition: collect all collectibles and defeat all enemies before time runs out
- Lose conditions: timer reaches zero or lives reach zero
- Game Over and Victory screens with buttons and audio
- Level 2 is locked on the Level Selection screen until Level 1 is completed
- Boy/Girl character selection flow
- All scenes registered in Build Settings

## Imported Asset Store Packages

The project now includes locally imported free Asset Store packages found on this machine:

- `RPG Tiny Hero Duo PBR Polyart`
- `Stylized Medieval Ranger Outfit`
- `Flooded Grounds`

The character selection screen uses the imported boy and girl character prefabs. The non-gameplay UI screens use a Flooded Grounds background prefab.

## Asset Store Replacement Points

The current project uses procedural placeholder geometry, generated materials, and generated child-friendly audio so it can run without external downloads. Replace these objects with imported Unity Asset Store assets after signing into Unity:

- `Boy Character - Asset Store Replacement`: replace with the imported boy character model.
- `Girl Character - Asset Store Replacement`: replace with the imported girl character model.
- `First Person Player`: replace with boy/girl hero models or attach visible first-person arms.
- `Chaser Enemy`: replace with animated enemy models.
- `Boss Enemy`: replace with a larger boss model and animations.
- `Textured Stone Floor`, `Bright Castle Wall`, and `Crystal Column`: replace with environment prefabs/materials.
- Generated audio in `AudioManager`: replace the procedural clips with imported music and sound effects.

After replacing assets, rerun `Adventure Quest > Build Complete Game` from the Unity menu if you want to regenerate the scenes from the scripted builder.
