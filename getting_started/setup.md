# Setup

Armory bundle comes with everything you need.

- [Download SDK](http://armory3d.org/download.html).
- Unpack `Armory_version.zip` to your preferred location. *(On Windows, prefer a short path like `C:\Dev` or unpack with [7-zip](http://www.7-zip.org) to prevent long path errors and speed-up the extraction.)*
- Run Blender located in the unpacked SDK. *(On Windows, you may need to enable it for the first time by clicking **More info** - **Run anyway**. On Linux, open terminal in the extracted folder and type `./blender`. On macOS, see `instructions.txt` file.)*

<img src="./getting_started/img/winrun.png" width="50%">

- To verify everything is working correctly, save your .blend file, switch to `Cycles Render` or `Eevee` engine (using a drop down located in the info header) and hit `Play` (F5) button, located in the `Properties - Render - Armory Player` panel.

- Continue to the [Playground tutorial](./getting_started/playground.md) to learn more.

<iframe width="560" height="315" src="https://www.youtube.com/embed/4FPKCUYjpP0?rel=0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Troubleshooting

- For old graphics cards, select `Low` preset in `Blender - Properties - Render - Armory Render Path`.
- If you have any trouble setting things up, [let us know](http://armory3d.org/community.html)!
- When naming things, prefer unaccented alphabetical letters `A-Z`.

### Windows

- To see error messages, start Blender from console or press `Blender - Window - Toggle System Console`.
- `Type not found : Main` error - save your .blend in a safe path like `C:\Users\user_name\Documents\test`, otherwise Windows may prevent writing the files.
- If `MSVCP140.dll` is missing, install [Visual C++ Redistributable for Visual Studio 2015](https://www.microsoft.com/en-us/download/details.aspx?id=48145).

### Linux

- To see error messages, start Blender from console.

### macOS

- To see error messages, start Blender from terminal using `/path/to/Armory/blender.app/Contents/MacOS/blender`.
- Due to security elements of macOS, you may get a `file corrupted` error. Try starting Blender from terminal like described above.


## Using Armory as add-on

If you do not require the built-in player, Armory can be used as add-on only in standard Blender installation. The player will then launch in a separate window.

- [Download](http://armory3d.org/download.html) and unpack appropriate SDK for your platform.
- In Blender, Select **File** - **User Preferences...** and navigate to **Add-ons** tab.
- Click **Install from File...**
- Select `armory.py` located in `my_unpacked_sdk/Armory/armsdk/armory/blender/addon` (on MacOS the location is `my_unpacked_sdk/Armory/Blender.app/armsdk/armory/blender/addon`).
- **Enable** Armory add-on.
- Set **SDK Path** property to `my_unpacked_sdk/Armory/armsdk`.
- Hit **Save User Settings** at the bottom and restart Blender. That's it!
