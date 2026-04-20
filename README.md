# Into The Breach — Turn-Based Strategy Game

A Python implementation of a turn-based tactical strategy game inspired by *Into The Breach*, built with tkinter for the Introduction to Software Engineering course at UQ.

## Gameplay

Players control mechs on a grid-based map to defend buildings from enemy units. Each turn, move your mechs and attack enemies before they destroy the city's buildings.

## Features

- Grid-based tactical map with tiles (Ground, Mountain, Buildings)
- Player-controlled mechs with unique abilities:
  - **TankMech** — long-range horizontal attacks
  - **HealMech** — heals adjacent friendly units and buildings
- Enemy units with AI behaviour:
  - **Scorpion** — melee attacker
  - **Firefly** — ranged attacker
- Buildings with health that can be damaged or destroyed
- Undo move functionality
- Save and load game state
- Full tkinter GUI with sidebar showing entity stats and a control bar
- 3 levels included

## Architecture

The project follows an MVC structure within a single file:

- **Model** — `Tile`, `Board`, `Entity`, `Mech`, `Enemy`, `BreachModel` classes managing all game state and logic
- **View** — `BreachView`, `GameGrid`, `SideBar`, `ControlBar` classes handling all tkinter rendering
- **Controller** — `BreachController` wiring model and view together, handling all user input

## Project Structure

```
a2_solution.py    # Main game code (model, view, controller)
a2_support.py     # Constants and support code
levels/
├── level1.txt
├── level2.txt
└── level3.txt
```

## Running

```bash
python a2_solution.py
```
