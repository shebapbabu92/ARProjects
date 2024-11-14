# 4ME306 - Cross Media Design and Production (AR Workshop 2)

## Project Overview

The **4ME306** project is developed as part of the Cross Media Design and Production course (specifically for AR Workshop 2). This project focuses on using augmented reality (AR) to create interactive media, with functionalities that align with workshop objectives, including image tracking and object interactions.

## Project Details

- **Project Name**: 4ME306 - AR Workshop 2
- **Course**: Cross Media Design and Production
- **Primary Script**: `ImageTargetTracker.cs`
- **Unity Version**: 2021.2.7f1 Personal (or compatible)
- **Platform**: Mobile AR (iOS and Android)

## Features

- **Image Target Tracking**: Tracks specific images to activate AR content.
- **Object Interaction**: Allows for interaction with virtual objects upon detection.
- **Customizable Tracking**: Adjusts for multiple image targets with tailored responses.

## Getting Started

### Prerequisites

Ensure the following are installed and set up before proceeding:

1. **Unity Editor**: Version 2021.2.7f1 Personal (or a compatible version)
2. **AR Foundation**: This project uses Unity's AR Foundation package for AR capabilities.
3. **ARCore/ARKit**: Install the AR SDK for Android (ARCore) or iOS (ARKit) as per your target device.

### Installation

1. Clone the repository or download it directly from GitHub.
2. Open the `4ME306` folder in Unity 2021.2.7f1 or later.
3. Allow Unity to load and compile all assets, scripts, and AR libraries.

### Project Structure

- **Scripts**: Contains the main AR functionality, including `ImageTargetTracker.cs`.
- **Assets**: All project assets, including images, models, and prefabs.
- **Scenes**: Unity scenes specific to the AR workshop requirements.

### Usage

1. Load the scene configured for AR tracking.
2. Build and deploy the project to an AR-compatible mobile device.
3. Aim your device camera at the specified image targets to trigger AR interactions.

## Scripts Overview

- **ImageTargetTracker.cs**: The primary script for image tracking functionality, which detects image targets and triggers corresponding AR content.
  - **Target Recognition**: The script initiates AR content upon recognizing specified image targets.
  - **Interaction Capabilities**: Provides options for user interaction with tracked objects.

## Contributing

If you wish to extend or improve this project, please consider:

- Adding additional image targets for AR experiences.
- Enhancing interaction mechanics or integrating new AR assets.

---

### License

This project is part of a course and may contain assets or code provided for educational purposes. Be sure to consult the course guidelines before distributing or modifying any part of the project.

