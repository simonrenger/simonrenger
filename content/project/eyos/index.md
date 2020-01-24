---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Eyos (In Development)"
subtitle: "A multiplayer RTS game written in C++ with data oriented design in mind. A learning project to deppen my C++ knowlegde and my network programming skills."
summary: "A multiplayer RTS game written in C++ with data oriented design in mind. A learning project to  challange my network programming skills. [more information](/project/eyos/)"
authors: ["admin"]
tags: ["windows","cpp","linux","networking"]
icons: ["logo logo-cpp svg-black","logo logo-cmake svg-black","fab fa-github text-black","fab fa-windows text-black","fab fa-linux text-black"]
categories: ["portfolio"]
date: 2019-12-01T15:10:00+01:00
lastmod: 2019-12-14T21:19:00+01:00
featured: false
draft: false

links: 
  - icon_pack: "fab"
    icon: "github"
    url: "https://github.com/Eothaun/Eyos"
    name: "Eyos"

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: "Smart"
  preview_only: true

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Eyos is a cross platform (Windows and Linux) targeting 2D multiplayer RTS focused on managing a massive amount of units. I see this project as a chance to enhance and challenge my network programming skills as well as my software engineering skills. The development of this project is open and can be found on github. ([GitHub](https://github.com/Eothaun/Eyos)).

## My main responsibilities

**The network architecture**

I am in charge for the network architecture which supports the synchronization of millions of entities via the network. The chosen architecture is an *peer to peerish* server-client approach, with deterministic lock step. As descripted in this article [Age of Empire](https://www.gamasutra.com/view/feature/131503/1500_archers_on_a_288_network_.php) and in this book *Architecting Networked Games by Joshua L. Glazer and Sanjay Madhav*. The host starts up a dedicated server on their machine and that one confirms the gameplay.



**QA Pipeline**

I am working with GitHub Actions. It verifies that our game can be build on Windows (`msvc`) and Linux (our test environment is Ubuntu) with GCC9 and Clang9 tool chain. Our code gets also tested and verified with clang-tidy and clang format every time someone pushes. Besides this `ctest` runs our unit tests (Catch2)




| Project Information |                                                       |
| ------------------- | ----------------------------------------------------- |
| Type:           | Networking RTS                 |
| Duration:           | Decemeber 2019 - Ongoing Development                  |
| Teamsize:           | 3 Programmers                                         |
| Roles:              | QA Engineer, Engine & Network programmer     |
| Engine:             | Eyos Custom Game Framework                            |
| Platform:           | Windows & Linux                                               |
| Languages:          | C++                                                    |
| Technologies:       | cmake, clang & msvc, git, bgfx, GitHub Actions, hack'n plan |


<div class="github-card" data-github="Eothaun/Eyos" data-width="400" data-height="153" data-theme="default"></div>
<script src="//cdn.jsdelivr.net/github-cards/latest/widget.js"></script>
