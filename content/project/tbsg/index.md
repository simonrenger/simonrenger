---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "“Tomorrow Engine“"
subtitle: "A Custom C++ crossplatform network card game engine"
summary: "A multiplayer crossplatfrom c++ determinstic linear card game engine developed in 16 weeks. Targeted for Playstation 4 and Windows 10 [more information](/project/tbsg/)"
authors: ["admin"]
tags: ["cpp","ps4","windows"]
icons: ["logo logo-cpp svg-black","logo logo-lua svg-black","fab fa-js text-black","fab fa-windows text-black","fab fa-playstation text-black"]
duration: "16 Weeks - February to July 2019"
team: "1 Programmers, 5 Designers, 8 Artists and 1 Producer"
roles: "Tech Lead, Tools programmer, Scrum Master"
Engine: "Custom cross-platform C++ Engine (Windows and PS4) with Electron Tooling (Tomorrow Engine) "
categories: ["portfolio"]
date: 2019-05-01T20:19:00+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "A multiplayer crossplatfrom c++ card game engine developed in 16 weeks."
  focal_point: "Smart"
  preview_only: true

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

The tomorrow engine is a cross platform C++ game framework which allows the creation of deterministic linear card games. The player had to fight the opponent and the 3 monsters in the game. The game we created with this was called Raptoads. The Framework supported Playstation 4 and Windows 10.

## Gameplay trailer

{{< youtube KfBd1vJM9wI >}}

## My main responsibilities

Besides being the Tech lead / Team lead of the 11 programmers, I have been in charge for the core architecture. Besides this I have been responsible for implementing and designing the extensive tooling and pipeline for content creation, content management. The tooling was created in web technologies (electron & SQL Database), this allowed us for quick and rapid iterations.

### Core Architecture

The application were split into four different modules. The Framework (TBSG) which served the Client as well as the Server with the basic utilities. Besides this we have the Network layers as its own lib. 

When designing the modules I kept the guideline that the architecture shall be for our game type specific: _determinstic linear card games_. That is why I chose for a "data oriented" approche with packing related data closely together.

### Tooling - The Hub

The framework came with its own tooling which was written in JavaScript and Electron. It served as the main content creation tool for Designers. The tool offered the following functions:

- AI Optimization for the QA Test games
- Modifiying the underlaying content database (SQL)
- source contol of our Lua card scripts
- UI Editor
- Lua Script validation


| Project Information |                                                              |
| ------------------- | ------------------------------------------------------------ |
| Duration:           | 16 Weeks - February to July 2019                                                   |
| Team size:          | 11 Programmers, 5 Designers, 8 Artists and 1 Producer        |
| Roles:              | Tech Lead, Tools programmer, Scrum Master                    |
| Engine:             | Custom cross-platform C++ Engine with Electron Tooling (Tomorrow Engine) |
| Platform:           | Windows, Playstation 4                                       |
| Languages:          | C++, JavaScript, Lua, SQL                                    |
| Technologies:       | Lua Scripting, Online Crossplay Multiplayer, Event/HTTP/UI handling with PS4 Support. |

| Project Highlights                                           |
| ------------------------------------------------------------ |
| Scripting Pipeline: A Lua dialect which allowed designers to quickly develop with our tooling the card behaviour. |
| Scripting source control integration - via the tooling |
| Google Drive integration & Sheets |
| Utility AI - custimizeble via the tooling |
| Custom Tooling written with Web technologies for quick iterations, tool of choice: Electron & MariaDB |
| Playstation 4 Support: The engine supported Playstation 4    |

