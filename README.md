# Sound Source Localization Using Coincident Microphone Pair

## Overview
This project focuses on the development and simulation of an advanced sound source localization system, utilizing a pair of coincident microphones. It aims to simulate a realistic environment where users can estimate the direction and distance of various sound sources, providing a tool that is particularly useful in acoustics research and audio engineering.

## Key Features
- **Dynamic Angle Adjustment**: Microphones dynamically adjust their angles to optimize the detection of sound sources.
- **Handling Multiple Sound Sources**: Capable of distinguishing and localizing multiple sound sources in a simulated environment.
- **Accuracy Metrics**: Includes measurement of localization accuracy, signal-to-noise ratio, and system response time.
- **Interactive Simulation Environment**: A user-friendly interface for placing sound sources and microphones, and visualizing their interactions.

## Installation
To set up this project, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/your-repository/sound-localization.git
   ```
2. Navigate to the project directory:
   ```bash
   cd sound-localization
   ```
3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Usage
To use the simulation environment, you need to initialize the microphones and sound sources, and then run the simulation. Here is a basic example:

```python
from sound_localization import Mic, simulate_environment

# Initialize microphones at specified positions and angles
mic1 = Mic('Mic1', 0, 0, np.pi/2)
mic2 = Mic('Mic2', 5, 0, np.pi/2)

# Define positions of sound sources
sources = [(3, 4), (-2, 6)]

# Run the simulation
simulate_environment([mic1, mic2], sources)
```

This code will simulate an environment with two microphones and multiple sound sources, showcasing how the microphones adjust their orientation to optimize sound source localization.
