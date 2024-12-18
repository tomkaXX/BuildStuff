# BuildStuff
Workshop for a BuildStuff 2024

**Participant Level**: All Levels  
**Date and Time**: 14:00 PM – 16:00 PM  
**Location**: Opsillon Room (2nd Floor)  

**Presentation**: [link ](https://prezi.com/view/2jS6FFfvmolAuBgeuKmN/)

**Workshop notebook**: [link to colab](https://colab.research.google.com/github/tomkaXX/BuildStuff/blob/main/BuildStuff.ipynb)  




## Agenda

**Main Topics**
The main topics to be covered in this workshop include:
- General Presentation

**Practical Part**
- Visualize Drone Imagery from D2S
- Visualize Google Earth Engine Data and Create Interactive Maps

**Optional**
- Explore Earth Engine Data Catalogs
- Analyze Earth Engine Data
- Create Time-Lapse Animations


---

## Workshop Overview

Recent advancements in drone and satellite technology have made high-resolution geospatial data more accessible and affordable. This workshop provides hands-on training on an open-source platform for processing and analyzing drone data, covering both the basics and advanced techniques in drone and satellite data integration. Participants will work with powerful Python tools, including `Geemap` and `Leafmap`, to search, visualize, and analyze geospatial data in a Jupyter Notebook environment.

### Data Description
The workshop includes sample data collected over several flights using various sensors and overlapping parameters. Attendees will learn how to process data from RGB, LiDAR, and multispectral sensors to create orthomosaics, point clouds, and DSM products. The data below provides key details for each flight conducted.

---


## Step 1: Prerequisites
✨ Create a free account at D2S to start uploading, managing, and visualizing your drone imagery! 
Register here: https://ps2.d2s.org/auth/register

🌐 Access maps and satellite data 
Register an account here: https://code.earthengine.google.com/

📝 Download sample data:
Flight sample data: [Link to Google Drive files](https://drive.google.com/drive/folders/1fjakT4R7E1o1wTQA_FMNjdt41Y7BixxU?usp=sharing)  

✨ Follow this parameter for creating a project at the D2S platform. 

Flight data parameters for D2S Platform:[parameters](https://github.com/tomkaXX/BuildStuff/tree/main/sample%20data)

Currently, ipywidgets does not work well with Colab dark theme. Some of the geemap widgets may not display properly in Colab dark theme. It is recommended that you change Colab to the light theme.

**DS2 Platform Registration**: [Register your account here](https://ps2.d2s.org/projects)  

**Flight sample data**: [Link to Google Drive files](https://drive.google.com/drive/folders/1fjakT4R7E1o1wTQA_FMNjdt41Y7BixxU?usp=sharing)  

## Colab 

Every participant will be working with Google Colab as their own copy.

**Workshop notebook**: [link to colab](https://colab.research.google.com/github/tomkaXX/BuildStuff/blob/main/BuildStuff.ipynb)  
If you are using Google Colab, you can open the notebook in Google Colab directly from the GitHub link. This will allow you to work with the notebook in your own Colab environment without modifying the original file.

### You’re Ready to go!

---

## Additional and Useful Resources

- [Geemap Book](https://book.geemap.org/)  
  A comprehensive guide to using Geemap for geospatial analysis with Google Earth Engine.

- [Geemap - Map Visualization Chapter](https://book.geemap.org/chapters/02_maps.html)  
  Focuses on map visualization techniques in Geemap, including interactive mapping features.

- [Google Earth Engine - Image Visualization Guide](https://developers.google.com/earth-engine/guides/image_visualization#colab-python)  
  Official guide for visualizing images in Google Earth Engine using Python in Colab.

- [Leafmap Tutorials Playlist](https://gishub.org/youtube-leafmap)  
  A YouTube playlist offering tutorials on Leafmap, a Python package for interactive maps.

- [Geographic Software Design Playlist](https://gishub.org/gsd)  
  Video series on design principles for geographic software, focusing on geospatial tools.

- [Spatial Data Management Playlist](https://gishub.org/sdm)  
  A playlist covering techniques and best practices in spatial data management.

- [Leafmap Homepage](https://leafmap.org)  
  The official homepage for Leafmap, a tool for creating interactive maps in Python.

- [Geemap Homepage](https://geemap.org)  
  The official homepage for Geemap, a Python package for Google Earth Engine applications.

- [Google Earth Engine Code platform](https://code.earthengine.google.com/)  
  Google Earth Engine account to access powerful geospatial data processing tools.

- [Data to Science (D2S)](https://ps2.d2s.org)  
  A platform for managing and visualizing data with a focus on drone imagery and other geospatial data.

- [Google Earth Engine Developers Guide](https://developers.google.com/earth-engine/)  
  Documentation and guides for using the Google Earth Engine API.

- [PX4 Documentation](https://docs.px4.io/main/en/robotics/)  
  A resource for PX4, an open-source flight control software for drones, with information on robotics integration.
---

Here’s a guide for testing drones and other vehicles in simulation:

| **Simulator**              | **Platform**             | **Control Options**                    | **Hardware Requirements**                          | **Special Features**                                    | **Ideal For**                                         | **Link**                                                |
|----------------------------|--------------------------|----------------------------------------|----------------------------------------------------|---------------------------------------------------------|---------------------------------------------------------|----------------------------------------------------------|
| **AirSim**                 | Windows, Linux           | Game controllers, keyboard, custom remotes | GPU with DirectX 11; moderately powerful CPU       | APIs for Python and C++, Unreal Engine, realistic physics | Researchers and developers focused on AI and data analysis | [AirSim GitHub](https://github.com/microsoft/AirSim)    |
| **FlightGear**             | Windows, macOS, Linux    | Keyboard, mouse, joystick, USB controllers | Moderate GPU, mid-range CPU                        | Open-source with real-world mapping, customizable       | Enthusiasts seeking realistic flight for fixed-wing drones | [FlightGear Official Site](https://www.flightgear.org/)  |
| **DRL Simulator**          | Windows, macOS           | Game controllers, custom drone controllers | Dedicated GPU, moderately powerful CPU             | Realistic racing environments, multiplayer mode         | Drone racing enthusiasts and competitive pilots          | [DRL Simulator](https://thedroneracingleague.com/simulator/) |
| **Gazebo with ROS**        | Linux (Ubuntu preferred) | Custom controllers, ROS-compatible hardware | Moderately powerful CPU, dedicated GPU for graphics | Integrates with ROS, supports realistic physics         | Researchers needing open-source robotics testing         | [Gazebo](http://gazebosim.org/)                           |
| **RealFlight (Free Demo)** | Windows                  | Joystick, custom USB RC controllers    | Mid- to high-range GPU, powerful CPU               | High-quality graphics, realistic physics                | Drone enthusiasts and RC pilots for realistic practice   | [RealFlight](https://www.realflight.com/)                |
| **VelociDrone (Free Demo)**| Windows, macOS           | Game controllers, USB or RC transmitter | Moderate GPU, mid-range CPU                        | FPV physics, multiplayer, custom track building         | FPV racing enthusiasts and freestyle pilots              | [VelociDrone](https://www.velocidrone.com/)              |



## ✈️ My Drones Video
Sri Lanka 2018. Press on the image to watch the video
[![Scenic filming Video](https://img.youtube.com/vi/YBrenZHu31g/maxresdefault.jpg)](https://www.youtube.com/watch?v=YBrenZHu31g&ab_channel=TamaraKoliada)


Racing drone in Mallorca (30 October 2024)
[![Racing drone Video](https://img.youtube.com/vi/kJVjDiOpkrc/0.jpg)](https://www.youtube.com/watch?v=kJVjDiOpkrc&feature=youtu.be)


## ✈️ Drones
- **5” Bind n Fly FPV Drone:** [Link](https://tinyurl.com/mrxnw5nv)
- **Travel-Friendly FPV Drone:** [Link](https://amzn.to/42OikQx)

## 🏎️  Racing Drone Parts
- **Five33 Frame (SFG):** [Link](https://tinyurl.com/mryuhchy)
- **Side Force Generators:** [Link](https://tinyurl.com/2jm3nzms)
- **Champions 2207 Motor:** [Link](https://tinyurl.com/2phpkyau)
- **RunCam Racer Nano 2:** [Link](https://amzn.to/3ZAO4qU)
- **Foxeer Reaper Mini (ESC):** [Link](https://amzn.to/449riby)
- **Foxeer F722 V4 Mini (FC):** [Link](https://amzn.to/44h6COY)
- **TBS Crossfire Sixty9 (VTx & Rx):** [Link](https://amzn.to/42Zeuoq)
- **Smooth As Props:** [Link](https://amzn.to/3PxTIIx)

## 🎮 Controller Setup
- **TX16S Controller:** [Link](https://amzn.to/3YpdkPu)
- **Battery:** [Link](https://amzn.to/3SSWd7M)
- **Crossfire Module:** [Link](https://amzn.to/3MjPIJn)

## 🧰 Essential Tools
- **Smoke Stopper:** [Link](https://amzn.to/3PvluFk)
- **TS101 Soldering Iron:** [Link](https://amzn.to/3kJ9gw1)
- **4-in-1 Hex Driver:** [Link](https://amzn.to/3nIrIWq)
- **Ratcheting Prop Tool:** [Link](https://amzn.to/3yk2DmI)
- **Solder:** [Link](https://amzn.to/3ZHgNdp)







