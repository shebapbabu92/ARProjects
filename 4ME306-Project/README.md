# 4ME306 - Cross Media Design and Production

## Overview

The **4ME306** project, created for AR Workshop 2 in the *Cross Media Design and Production* course, demonstrates advanced multi-target functionality using the Vuforia engine in Unity. Users can interact with multiple AR image targets (or markers), enabling a dynamic resizing effect where AR content scales based on the proximity of two markers. This provides a responsive and immersive AR experience, ideal for interactive media and educational applications.

## Project Details

- **Project Name**: 4ME306 - Cross Media Design and Production
- **Supported Unity Version**: 2021.2.7f1 Personal
- **AR Engine**: Vuforia
- **Scripts**: `ImageTargetDistanceScaleManager`, `plus`, `minus`
- **GitHub**: [https://github.com/nicoversity](https://github.com/nicoversity)
- **Author**: Nico Reski, with modifications by Sheba Ponmelil Babu

## Key Features

1. **Multi-Image Target Tracking**: Utilizes Vuforia’s image target capabilities to track and respond to multiple AR markers.
2. **Proximity-Based Scaling**: Implements dynamic scaling of AR content based on the distance between two markers ("Content" and "Plus").
3. **Controlled Scaling Limits**: Prevents AR content from exceeding a defined maximum scale, maintaining visual clarity and consistency.

## Functionality

The main functionality is handled by the `ImageTargetDistanceScaleManager` class, which performs the following tasks:

- **Distance Calculation**: Determines the distance between the Content and Plus markers to adjust scaling dynamically.
- **Distance-Based Scaling**: Adjusts the scale of AR content based on the relative positions of the two markers.
- **Position Realignment**: Repositions the virtual object to float above the physical marker, maintaining alignment during scaling adjustments.


## Getting Started

### Prerequisites

Make sure the following tools and versions are installed before running **4ME306**:

- **Unity**: Version 2021.2.7f1 or compatible
- **Vuforia**: Installed and configured within Unity for AR tracking support

### Installation

1. Clone or download the **4ME306 - Cross Media Design and Production** project folder.
2. Open the project in Unity.
3. Import and configure Vuforia as needed.
4. Load the AR scene and test the functionality by interacting with the Content and Plus markers.

### Usage

The scaling effect is managed by two main scripts:

- **plus.cs**: Increases the size of the AR content based on proximity.
- **minus.cs**: (If implemented) Decreases the AR content size.

These scripts enable interactive resizing for a dynamic AR experience.

---



