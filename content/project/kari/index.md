---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "Kari (In Development)"
subtitle: "Kari is a single player, adventure game in which you are stuck on the island of the Nordic gods."
summary: "Kari is a single player, adventure game in which you are stuck on the island of the Nordic gods. [more information](/project/kari/)"
authors: ["admin"]
tags: ["windows","ue4"]
icons: ["logo logo-cpp svg-black","logo logo-csharp svg-black","logo logo-ue4 svg-black","fab fa-windows text-black","fab fa-jenkins"]
duration: "	January 2020 - July 2020"
Focus: "Build & Test pipeline as well as Commit Testing tool (C# WPF)"
team: "6 programmers, 10 designers, 12 artists, 1 producer"
roles: "QA & Tools engineer"
Engine: "Unreal engine"
categories: ["portfolio"]
date: 2020-04-16T00:10:00+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: "Kari is a single player, adventure game in which you are stuck on the island of the Nordic gods."
  focal_point: "Smart"
  preview_only: true

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

Kari is a single player, adventure game in which you are stuck on the island of the Nordic gods. It is your job to complete quests given by the gods and the islands inhabitants in order to rebuild your boat. 

{{< youtube lthr3OE43MI >}}
> Game teaser, basic game overview

## My main responsibilities

I am mainly responsible for the QA pipeline and the Jenkins set up. I created a [Jenkins Utility library](https://github.com/simonrenger/jenkinsUtils).  This Jenkins groovy script collection helps us create the QA pipeline we want on the school's Jenkins server. The library contains a collection of functions to communicate with Helix Swarm, Mantis and Discord. It supports the automated testing pipeline in Unreal Engine. Furthermore, it can pack and build UE4 projects.

Besides, I have created a prototype of a Commit Testing Tool in WPF (Windows Presentation Foundation) and [Material Design for WPF](http://materialdesigninxaml.net/).

## P4CommitTester - prototype

 The purpose of this tool is it to test local or online Perforce changelists before they can be submitted or turned into a Swarm review. The tool has a simple `toml` configuration file in which the automated tests can be specified (e.g. unit tests, map tests/ funcionality tests). 
 
 One can also define pre/post steps. They will be executed before the actual tests run e.g. shelve all other changelists. This set up makes it possible for the tool to work with any kind of engine or software. When tests are finished, the tool will check the return code of the application and react appropriately (most test applications return `EXIT_FAILURE` on failure).

 Currently, the tool can only communicate with the Jenkins API to run online tests / builds.


### Images

| Changelist Overview |
| ------------------- |   
|![commit selection](/img/commits.png)|
|List of all possible changelists. The default changelist is excluded because it is not really a changelist.|

| Selected Changelist Details |
| ------------------- |   
|![commit selection](/img/commitview.png)|
|You can shelve (if it is a shelved changelist), unshelve and test the current changelist.|

| Test configuration |
| ------------------- |   
|![configure tests](/img/tests.png)|
|Toml file to configure the tool to run tests.|

| Test Results |
| ------------------- |   
|![configure tests](/img/tests_ok.png)|
|In case the tests were ok the user can create a review or commit directly. If they were not successful the user would find the log here.|


## Project Overview

| Project Information |                                                       |
| ------------------- | ----------------------------------------------------- |
| Type:               | Single player, adventure game                 |
| Duration:           | September 2019 - Ongoing Development                  |
| Teamsize:           | 6 programmers, 10 designers, 12 artists, 1 producer |
| Roles:              | QA & Tools engineer                                     |
| Engine:             | Unreal Engine                                                  |
| Platform:           | Windows                                             |
| Languages:          | C++, Jenkins Groovy, C#                                                    |
| Technologies:       | Jenkins, Visual Studio, C# UWP, C# WPF          |
