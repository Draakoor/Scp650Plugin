# Scp650plugin
A plugin for SCP: Secret Laboratory (based on the Exiled framework) that adds the eerie behavior of SCP-650, the “Startling Statue.”

When a player enters the same room as SCP-650, the statue will mysteriously move whenever it’s not being directly observed — often appearing closer each time you look away. Its only purpose is to unsettle and surprise players by suddenly appearing behind them or in unexpected positions, creating a creepy and tense atmosphere.

Inspired by SCP Foundation lore, this mod brings SCP-650 to life as a passive but terrifying entity that loves to make you jump.

![20251028011456_1](https://github.com/user-attachments/assets/4eed9e8c-5efc-4961-b032-2cfb593194a4)

Requirements:
0. Exiled framework. [https://github.com/ex-team/EXILED](https://github.com/ExMod-Team/EXILED)
1. MapEditorReborn plugin. [https://github.com/Michal78900/MapEditorReborn](https://github.com/rockysx27/MapEditorReborn)

Installation:
1. Export the dependency `Configs` File from the .zip to the EXILED folder in the %appdata%, and override.
2. Install scp650plugin.dll to %appdata%\Roaming\Exiled\Plugins.
3. **Run Local Admin. And Exit.**
5. Check out whether it operates normally.

**Edit Poses/Create Poses:**
1. Download SL-CustomObjects. https://github.com/Michal78900/MapEditorReborn/releases/tag/2.1.2
2. Load scp650 schematic folder. By using 'import schematic' of bar 'schematic'.
3. Add 'Pose Recorder'script to root object: SCP-650.
4. Edit property 'size' of 'Objects' of the script to 13.
5. Drag all mixamorig:{joint name} to each Elements of the property.
5-1. If you're going to add more joint to edit, you can add more mixamorig.
6. **A primitive object with mixamorig in its name means that it will position a joint with the same name on same position.**
7. Make your poses. **SCALE DOESN'T SUPPORTED.**
8. Press play button. Then there will be a log on console tab.
9. Press it to see all of log content. And copy it.
10. Open global.yml. And write following.

```
- pose_name: {pose_name_here}
  transform_per_joint:
{paste_console_content_here}
```
11. If you want to set the pos to default:standing, just select all mixamorig and set rotation to 0 0 0.
