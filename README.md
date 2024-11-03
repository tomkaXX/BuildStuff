# BuildStuff
Workshop for a BuildStuff


Here’s a guide to setting up Project AirSim  for testing drones and other vehicles in simulation:

# Step 1: Prerequisites
MacOS
Ensure macOS compatibility:
AirSim works best on macOS Mojave or later, and requires a powerful machine for smooth simulation, ideally with a dedicated GPU.
Install Xcode:
Install Xcode from the App Store, as you’ll need some of its command-line tools for Unreal Engine and AirSim setup.
Install Homebrew:
Homebrew is a package manager for macOS and will simplify the installation of required dependencies.
bash
```
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

# Install dependencies:
Using Homebrew, install Python3 and other essential dependencies:
bash
```
brew install python3 cmake clang
```

# Step 2: Install Unreal Engine
AirSim uses Unreal Engine to render the simulation environment, so you’ll need to install it.
Download the Epic Games Launcher:
Visit Unreal Engine’s website and download the Epic Games Launcher.
Install Unreal Engine:
Open the Epic Games Launcher, sign in, and install Unreal Engine (ideally version 4.27, as it's more stable with AirSim).
Open Unreal Engine and Create a Project:
Launch Unreal Engine and create a new project (preferably in “Blank” or “Flying” mode).
Choose Blueprint for ease of setup, and make sure the project is set to No Starter Content for faster loading.
Name and save the project somewhere accessible.
Step 3: Clone and Build AirSim
Clone the AirSim Repository:
Open a terminal and clone the AirSim GitHub repository.


```
bash
git clone https://github.com/microsoft/AirSim.git
cd AirSim
```

Build AirSim:
Run the build.sh script to compile AirSim for macOS.
```
./build.sh
```

This process may take a few minutes and will create a Plugins folder in the AirSim directory with the AirSim plugin.
Step 4: Add AirSim Plugin to Unreal Project
Copy AirSim Plugin:
Navigate to your newly created Unreal project directory.
Create a Plugins folder inside it if it doesn’t exist, and copy the AirSim Plugins folder you just built into this new directory:
```
cp -r ~/path_to_AirSim_repo/AirSim/Plugins ~/path_to_Unreal_project/Plugins
```

Launch Unreal Engine with AirSim:
Open your Unreal Engine project in Unreal Editor. It may prompt you to rebuild AirSim for compatibility; allow it to proceed.
Once loaded, you should see AirSim options under Simulation.
Step 5: Test and Run AirSim
Configure AirSim Settings:
In your Unreal project’s root folder, create a file called settings.json with basic configurations for a drone:
json
```
{
    "SettingsVersion": 1.2,
    "SimMode": "Multirotor",
    "Vehicles": {
        "Drone1": {
            "VehicleType": "SimpleFlight",
            "X": 0, "Y": 0, "Z": 0
        }
    }
}
```

Save settings.json in the root of your Unreal project folder.

# Run the Simulation:
Press the Play button in Unreal Engine to start the simulation. You should see a drone model in the Unreal environment.
If the drone appears stationary, you can control it using AirSim's APIs or an Xbox controller.
Test with Python APIs:
AirSim provides Python APIs for controlling the drone. To use them, navigate to the AirSim/PythonClient directory and run a sample script:

```
cd ~/path_to_AirSim_repo/PythonClient
python3 hello_drone.py
```

This script will connect to the simulated drone and execute some basic commands, like takeoff and landing.
# Troubleshoot:
If the drone doesn’t respond, check the settings.json configuration or ensure your project is in Play mode in Unreal.
You can also test other scripts in the PythonClient folder, such as moveOnPath.py or camera.py for more advanced control and testing.

# Optional: Configure Additional Settings
You can add more configurations in settings.json to fine-tune the simulation environment, such as camera settings, weather conditions, and additional drones.

# You’re Ready to Simulate!
This setup will allow you to test AirSim on your MacBook using Unreal Engine. You can now use Python scripts to control the drone in real-time and explore AirSim’s additional APIs for navigation, data collection, and machine learning experimentation.


