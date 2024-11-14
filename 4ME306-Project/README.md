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

# AR Marker Interaction and Scaling System

## Functionality

The primary functionality is handled by the `ImageTargetDistanceScaleManager` class, which manages the interaction between multiple AR markers and dynamically adjusts the virtual content based on their relative positions. This is achieved through the following core features:

### 1. **Distance Calculation**
The system calculates the distance between the **Content** and **Plus** AR markers using their positions in 3D space. This distance is essential for scaling the virtual object in relation to the markers.

### 2. **Distance-Based Scaling**
Once the distance is calculated, the `ImageTargetDistanceScaleManager` adjusts the scale of the virtual object associated with the **Content** marker. The scaling factor is dynamically determined based on how close or far apart the **Content** and **Plus** markers are. As the distance changes, the virtual object will either scale up or down accordingly.

### 3. **Position Realignment**
The virtual object is repositioned above the **Content** marker to maintain a floating effect. After each scaling adjustment, the position of the object is updated to keep it aligned correctly with the **Content** marker, ensuring the virtual object stays in place visually relative to the marker.

---

## `ImageTargetTracker` Class

In addition to the `ImageTargetDistanceScaleManager`, the **`ImageTargetTracker`** class is used to detect whether an AR marker (such as **Content** or **Plus**) is being tracked by the camera. This class doesn't perform any calculations or transformations but rather provides the tracking status. The `ImageTargetDistanceScaleManager` uses this status to determine whether the markers are present, and whether scaling and realignment need to occur.

- **Tracking States**: The `ImageTargetTracker` class uses events like **OnTargetFound** and **OnTargetLost** to update whether the marker is being tracked, which is essential for deciding when to apply changes to the virtual object's scale and position.

---

## Conclusion

The system efficiently handles real-time scaling and positioning of AR content based on the distance between markers. As the user moves the markers closer or further apart, the content will adjust its size accordingly, while always staying aligned above the respective markers.


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



