# Terraria Server with tModLoader binaries
This playbook creates a Terraria server with tModLoader binaries. Be aware that the tModLoader server version is set as a variable in the playbook and must be changed if a new version of the binaries are published.

To import mods on the server, the .tmod files must be placed in the `mods` folder and edit `mods/enabled.json` to enable them on start.

Feel free to edit the server configuration file (`serverconfig.txt`) to change the autocreation or set a specific world to load. Per default, the world will be a Medium sized map with Normal difficulty named "Terraria".
