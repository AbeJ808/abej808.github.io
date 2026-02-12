---
layout: page
title: Retro Game Device 
description: Arm processor based RPG game written in C
img: assets/img/2035Game.jpg
importance: 2
category: academic projects
giscus_comments: false
---



# Overview

This project was the culminating final assignment for ECE 2035, where I designed and implemented a fully functional top-down roguelike RPG on an ARM-based MBED microcontroller. The game was written entirely in C and consists of over 3,700 lines of code.

The system integrates an LCD display, hardware switches, and an SD card reader to create a standalone embedded gaming platform. All logic, rendering, and data structures were implemented manually with a focus on low-level memory management and efficient system design.

# Project Demo

<div style="text-align: center;">
  <iframe width="560" height="315"
    src="https://www.youtube.com/embed/-ByK3FcCoNQ"
    title="Demo Video"
    frameborder="0"
    allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
    allowfullscreen>
  </iframe>
</div>


# Hardware Platform

The game runs on an ARM MBED processor and interfaces with:

- LCD display for real-time rendering

- Physical switches for player input

- SD card reader for persistent storage

- On-board memory for dynamic game state management

# Game Features

- Two unique playable maps

- Collectible items

- Two enemy types with distinct behaviors and drop maps

- Final boss encounter

- Scoreboard system

- Persistent save/load functionality

The codebase was modularized into rendering, entity management, game logic, and storage subsystems to maintain clarity and scalability.

# Custom Data Structures & Memory Management

A primary challenge was efficiently managing large game-world data within limited embedded memory.

To support over 3,500 map items, I implemented:

- A custom hash table using linked-list chaining

- Custom hash, insert, lookup, and collision-resolution functions

- Dynamic memory allocation and deallocation

This allowed constant-time average lookup performance while operating under strict RAM constraints.

# Persistent Save/Load System

The save/load system writes the complete game state to an SD card, enabling power-off persistence.

The system:

- Serializes player stats, inventory, and quest progression into a txt file format

- Stores map state and enemy conditions

- Restores the full game state on reboot with the option of creating a new save at any point

This required careful struct organization and file handling in C to ensure reliability and data integrity.

# Technical Challenges

Debugging memory leaks

Designing efficient data structures without standard containers

Optimizing display updates for limited processing power

Ensuring reliable SD card read/write operations

# What This Project Demonstrates

Embedded systems programming

Low-level C development

Custom data structure implementation

Hardware–software integration

Ownership of a large, single-developer codebase

System design under resource constraints

