
# TokenMaster-Launcher-FDL

This repository aims to contribute to the **TokenMaster Launcher Pro v5.x FDL Cheat Codes** database.
> **credits** : [TokenMaster's Random Ramblings](https://tokenmaster.blogspot.com)

## XML structure is quite simple:

    <?xml version="1.0" encoding="utf-8"?>
    <FDL\>
      <cafd id="00000794" name="FEM_BODY" series="F020,F030"\>
        <code description="Angel Eyes Parking Light Brightness 50%" series="F030"\>
          <group id="3062"\>
            <function start="68" end="68" mask="11111111b" comment="MAPPING_STANDL_V_L_PWM Level 1 - Left"\>32</function\>
            <function start="80" end="80" mask="11111111b" comment="This is a comment..."\>32</function\>
          </group\>
        </code\>
      </cafd\>
    </FDL\>

 - CAFD ID is visible into .NCD file name or into Header section of .ncd file into launcher FDL Editor :
[FDL-cheat-code-1.png](https://postimg.cc/xkjnM8dv)
 - **name** : what you want but prefer the ECU real name
 - **series** : useful for Launcher UI filtering capability (optional)
 - **description** : useful for Launcher UI Review function to ensure you are coding the right settings (optional)
 - **group id, start, end and mask** : you can find them into FDL Editor with "*Storage Info*" selected :
[FDL-cheat-code-2.png](https://postimg.cc/c6Tx1Q4s)

## Create your own file
If the XML file does not exist in the launcher UI, you need to copy it to this folder : `%ProgramFiles%\TokenMaster\LauncherPRO5\FDLCodes` and then restart the Launcher.

## Updating existing Cheat Codes files
When XML file already exists into the Launcher UI, you only have to update to the last online version directly into the **Launcher FDL Cheat Codes menu**
[FDL-updating.png](https://postimg.cc/nM911z8t)

## Testing your own file
Your XML Cheat Codes files will have to be in `%LocalAppData%\LauncherPRO5\FDLCodes` (launcher must be restarted to take into account the new file). When updating to last version directly from Launcher UI, files are overwriten from this repository (since Launcher PRO v5.0.5). Before this version, master repository is [packetpilot](https://github.com/packetpilot/bmw-f) but not but not maintained anymore.

