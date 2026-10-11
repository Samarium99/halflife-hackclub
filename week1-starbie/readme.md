# Starbie

adapted from https://github.com/SharKingStudios/Starbie/tree/main

## Notes/Progress
#### Set up new venv `~/hack_club_venv`
```
python3 -m venv ~/hack_club_venv
```
#### Installed hackatime
Hackatime is the open-source Wakatime to track how long you spend productively on text editors VSCodium, XCode, Terminal, etc.
Also installed [add on](https://github.com/hackclub/kicad-wakatime) to track KiCad changes. 
```
curl -fsSL https://raw.githubusercontent.com/hackclub/hackatime-setup/refs/heads/main/install.sh | bash -s -- 18b4fb88-612a-4661-9f48-94d667e80b66
```
- Quick setup

#### Install care package materials
- `.sym` files = symbol libraries = collection of premade graphical components, assets
- `.pretty` folder = footprint libraries = collection of 3d models + schematic assets... for PCB design

#### Lapse
- create [new session](https://lapse.hackclub.com/timelapse/create) on Lapse
- install [lookout](https://lookout.hackclub.com/) to record desktop

## 10-11-26 Bugs with kicad-wakatime.app on MacOS
#### Screen & System Audio Recording prompt
Even after toggling on and off the Privacy & Security permissions for the application, the following popup would show:
<img width="459" height="176" alt="Screenshot 2026-10-11 at 6 57 11 PM" src="https://github.com/user-attachments/assets/3bb2d06b-5dbe-43a0-b975-78d13cf078a9" />
#### multiple .sch file error
Use the below command to identify additional .kicad_sch files:
```
find ~/path/to/kicad/files -name "*.kicad_sch"
```
kicad-wakatime returned error due to the file `.history/file.kicad_sch`
