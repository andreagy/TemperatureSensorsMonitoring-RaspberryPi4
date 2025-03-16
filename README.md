# Application Description

The application is a temperature measurement system using a Raspberry Pi 4. The program includes a graphical user interface, allowing users to control the measurement process and get statistical information about the sensor readings.
The project is part of the "Data Structures and Algorithms Project" course.

The system consists of three 1-wire, waterproof Shelly DS18B20 temperature sensors connected directly to the Raspberry Pi 4 through the GPIO4 pin. The Raspberry Pi reads temperature data from the sensors at set intervals, stores the data in a JSON file, and displays the GUI for user interaction. Through the GUI, users can start and stop measurements, as well as visualize the temperature data in the form of graphs. The system performs basic data analysis, including calculations of the maximum, minimum, and average temperatures. To further enhance the system, a linear regression model is implemented to predict future temperature trends based on the latest historical data.

# Package Dependencies

This project requires the following dependencies to be installed. Follow the instructions below for your operating system.

## nlohmann/json
A JSON library for C++.

- **GitHub:** [nlohmann/json](https://github.com/nlohmann/json)
- **MacOS Installation:**
  ```sh
  brew install nlohmann-json
- **Ubuntu/Debian Installation:**
```sh
sudo apt install nlohmann-json3-dev
```

## imgui 
Prerequisites: to run imgui on raspbian, install the packages below:
```sh
sudo apt-get update
sudo apt install libglfw3-dev libgles2-mesa-dev
sudo apt install libsdl2-image-dev libsdl2-mixer-dev libsdl2-ttf-dev
sudo apt install libglew-dev
```
## Compiling on Raspbian
```sh
mkdir build
cd build
cmake ..
make 
./DataStructureAlgorithmsProject
```
