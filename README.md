# Wings of Freedom

A third-person action game inspired by *wayang kulit*, the Javanese shadow puppet theatre.
Made by a team of four in 3 days.

> **Winner** of the international game marathon **"CyberSmena: Moscow — Indonesia"**, Skolkovo, October 2026.

![Wings of Freedom](images/landscape.jpg)

## Play

Download the Windows build from [Releases](https://github.com/DaniilBaranov-UNVS/wings-of-freedom/releases/latest): unzip it and run `Wings of Freedom.exe`.

Requirements: Windows 10/11 64-bit. A DirectX 12 GPU is recommended (ray tracing and DLSS need it).

## About

<img src="images/hero.jpg" align="right" width="260" alt="The Garuda hero">

The challenge of the marathon was to make a game that shows the culture of Indonesia.
We built the whole game around wayang kulit: the main menu is a shadow puppet show, the puppets
are menu buttons, and the music is a procedural gamelan.

You play as a young Garuda. The Lord of Scales, a lizard-man warrior, has kidnapped your mother.
To reach him, you travel through jungle villages, train in the village yard, and collect the pieces
of a sacred seal. Each piece is guarded by a guardian bound by an oath to the gods, and each one
has to be defeated in a boss fight. Then you cross the water by boat to the mountain for the final battle.

## Features

- **Combat system**: light attack combos, heavy attack, dodge roll with counter-attack, jump and dive attacks, stamina.
- **Three bosses** with phases and a rage mode: Raja Buta, the Demon Lord with a hammer, and the Lord of Scales.
  The final boss falls from the sky in a cutscene, and the game ends with a cinematic of his fall.
- **Enemy AI** on NavMesh: sight and hearing, alerting nearby enemies, attack queue, flanking, dodging.
- **Shadow theatre main menu**: the lamp lights up, the *gunungan* opens the show, and puppets act as buttons.
- **Tutorial**: a training yard with dummies that teaches movement and every main attack.
- **Legends**: an in-game encyclopedia about wayang characters, the puppeteer (*dalang*) and gamelan.
- **Side quests**: *Surakarta* (traditional Indonesian checkers) against a bot, wooden puzzles, and a 2D shadow play mini-game.
- **Procedural nature**: tropical trees with vines and roots, grass that bends under the player, wind.
- **English, Russian and Indonesian** localization.

## Screenshots

| | |
|---|---|
| ![Village](images/village.jpg) | ![Path to the mountain](images/gate.jpg) |
| Jungle village with the training yard | The path to the mountain |

<img src="images/menu.jpg" width="447" alt="Main menu">

Main menu: a shadow puppet show where the puppets are the menu buttons.

## Controls

| Action | Keyboard and mouse |
|---|---|
| Move | WASD |
| Sprint / slow walk | Shift / Alt |
| Jump, double jump | Space |
| Crouch | Ctrl |
| Dodge roll | C |
| Light attack (combo) | Left mouse button |
| Heavy attack | Right mouse button |
| Counter-attack | C, then left mouse button |
| Pause | Esc |

## Team

| | Role |
|---|---|
| [D.Baranov-UNVS](https://github.com/DaniilBaranov-UNVS) | Full-stack game developer, UI |
| [Leelik12](https://github.com/Leelik12) | Full-stack game developer |
| [Taizer124](https://github.com/Taizer124) | Level designer, developer |
| [TAllex](https://github.com/TAlleks) | 3D artist, sound designer, UI |

## Tech

- Unity 6 (6000.2), HDRP, Cinemachine 3, new Input System
- Code split into independent modules (core, player, combat, AI, UI, audio, animations) with their own assemblies.
  Modules talk through an event bus, so each one can be reused in another project.
- Object pooling, timers and game-time scaling for pause and slow-motion.
- PlayMode tests for core mechanics.

## Source code

The source code is private. This repository only shows the game.
If you want to see the code (for example, for a job application), contact me and I can give access.

© 2026 Wings of Freedom team. All rights reserved.
