# ROS-Based Autonomous Rescue Support Robot with Custom Parallel Gripper

## Overview
This project showcases an autonomous mobile robot platform developed using the Robot Operating System (ROS) for rescue support operations. The robot is equipped with a custom-designed parallel gripper mechanism, enabling it to autonomously pick up, transport, and place material boxes. Wireless communication via Wi-Fi facilitates remote command execution and status updates, while collision avoidance and location identification ensure the robot navigates safely within the defined operational field.

## Features
- **Autonomous Operation**: The robot autonomously performs tasks such as material handling based on remote commands.
- **Parallel Gripper**: Custom 3D-printed gripper mechanism designed to pick and place material boxes.
- **Collision Avoidance**: Integrated sensors and IR beacons for real-time collision detection and avoidance.
- **Remote Control**: Bidirectional communication via Wi-Fi for sending commands and receiving status updates.
- **ROS Integration**: Utilizes ROS for managing robot control, sensor data, and task coordination.

## Workflow
1. **Robot Platform**:
    - Developed using an Intel-based mobile robot platform, with motors and sensors integrated for navigation and task execution.
2. **3D-Printed Gripper**:
    - Designed and printed a parallel gripper that can open and close to handle different box sizes.
    - Integrated the gripper with the robot's control system using ROS, ensuring precise handling.
3. **Navigation & Control**:
    - Implemented collision avoidance using infrared (IR) sensors and beacons for safe movement.
    - Developed location identification systems to navigate through the predefined field setup.
4. **Wireless Communication**:
    - Enabled bidirectional Wi-Fi communication, allowing remote operators to send commands and receive live status updates.
    - ROS topics and nodes were used for task coordination and robot behavior management.

## Technologies Used
- **ROS (Robot Operating System)**: ROS nodes were employed for sensor integration, robot control, and task scheduling.
- **Intel Mobile Robot Platform**: The robot base was built using an Intel platform, equipped with motors, sensors, and wireless communication modules.
- **Wi-Fi Communication**: Wireless communication allowed for remote control and monitoring of robot tasks.
- **3D Printing**: A custom-designed parallel gripper was fabricated using 3D printing technology.
- **Sensors**: IR beacons and sensors were used for collision avoidance and navigation.

## How to Run the Project
1. **Set Up ROS**:
    - Install ROS on your system by following the [ROS Installation Guide](http://wiki.ros.org/ROS/Installation).
2. **Clone the Repository**:
    ```bash
    git clone https://github.com/TheMechanicHulk/ROS-Autonomous-Rescue-Robot.git
    cd ROS-Autonomous-Rescue-Robot
    ```
3. **Launch ROS Nodes**:
    - Run the ROS nodes to manage robot control, sensor input, and task execution.
    ```bash
    roslaunch rescue_robot robot_control.launch
    ```
4. **Establish Wi-Fi Communication**:
    - Ensure Wi-Fi is set up on both the robot and the control system for bidirectional communication.
5. **Test the Gripper**:
    - Test the custom-designed parallel gripper using ROS commands to ensure proper opening, closing, and handling of material boxes.

## File Structure
- `src/`: Contains ROS node code for controlling the robot and sensors.
- `models/`: 3D models of the parallel gripper, including STL files for 3D printing.
- `scripts/`: Python and Bash scripts for launching and controlling the robot in ROS.
- `docs/`: Detailed documentation on setup, hardware requirements, and operational instructions.

## 3D-Printed Gripper Design
- The gripper was designed using CAD software and printed with a standard 3D printer.
- The **STL files** for printing the gripper can be found in the `models/` directory.
- The gripper mechanism is controlled using ROS nodes to execute open/close actions.

## Sensor & Navigation System
- **IR Sensors**: Used for real-time collision detection, ensuring the robot can navigate safely in its environment.
- **Location Identification**: The robot uses IR beacons and triangulation to identify its location and follow predefined paths.
- **Collision Avoidance**: Implemented a simple algorithm using sensor input to avoid obstacles in real time.

## Future Improvements
- **Enhanced Gripper Functionality**: Add more precision to the gripper's control for handling delicate or irregular objects.
- **Advanced Navigation**: Integrate LiDAR or camera-based SLAM for more complex navigation tasks.
- **Autonomous Task Scheduling**: Develop advanced task scheduling algorithms to handle multiple tasks in dynamic environments.

## Acknowledgements
This project was developed using open-source resources from the ROS community and Intel's mobile robot platform.
