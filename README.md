# io_import_collada_normals
An import script to apply custom mesh normals from a COLLADA 1.4.1 file to objects in Blender.

## Install
This script is installed the same as any other Blender addon. For those that aren't fimiliar with this process:
1. Download the code and unzip the file.
2. In Blender, go to Edit > Preferences. This will open a new window.
3. In the preferences window, head to the "Addons" tab and click the button that says "Install"
4. Navigate to the unzipped code, and select the `.py` file.
5. Click the checkbox next to the addon in the when it pops up in the preferences window.

## Use
1. Import a Collada file using `File > Import > Collada (Default) (.dae)`.
2. Select all of the objects in your scene (default binding is `A`).
3. Go to File > Import > Import Collada Normals (.dae).
4. Import **the same Collada file you imported earlier.**
5. Objects will now use normals from the Collada file instead of auto-generated geometry normals

## Notes
* This addon relies on objects having the same name in your scene as in the Collada file. Objects that have been renamed (manually or by Blender because there was already an object with that name) won't have their normals imported.
* This addon was thrown together in just a couple hours and with very little testing, so it may be buggy. If it doesn't work properly, let me know and I'll try to fix the issue.
