# light-arena
FiveM Arena Zone Script for QBCore with automatic respawn and weapon system
# Arena Zone Script

Arena Zone is a lightweight and optimized PvP arena script for FiveM QBCore servers. It allows players to join a combat arena, receive arena-only weapons from an NPC, and automatically respawn after death. The entire arena system is controlled using a single admin event command.

---

## Features

- Arena zone detection
- Automatic respawn system
- Weapon NPC system
- Arena-only weapon restriction
- Automatic weapon removal when leaving arena
- Single admin command to control arena event
- Random respawn points
- Optimized and lightweight
- Fully compatible with QBCore

---

## Event Control

The entire arena system is controlled using one event command.

Enable Arena Event:

```
/event 2
```

Disable Arena Event:

```
/event 0
```

The arena will only function when the correct event stage is active.

---

## How It Works

1. Admin enables the event using the event command  
2. Players enter the arena zone  
3. Weapon NPC becomes available  
4. Players receive arena weapons  
5. Players fight inside the arena  
6. When a player dies:
   - Player is revived automatically
   - Player is teleported to a random respawn point
7. When a player leaves the arena:
   - Arena weapons are removed automatically

---

## Installation

1. Download or clone the repository:

```
git clone https://github.com/Aswerking/light-arena.git
```

2. Place the script in your resources folder:

```
resources/[local]/arena-zone
```

3. Add this to your server.cfg:

```
ensure arena-zone
```

4. Restart your server

---

## Configuration

All settings can be configured in:

```
config.lua
```

You can change:

- Arena location
- Arena radius
- Respawn points
- Weapon settings
- NPC settings
- Event stage

---

## Dependencies

Required dependencies:

- qb-core
- qb-target or ox_target
- hospital script

---

## Author

Light Studio  
Independent FiveM Developer  

---

## Version

1.0.0

---

