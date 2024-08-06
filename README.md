Motion Planning and Decision Making for Autonomous Vehicles
This project showcases my implementation of key components in a hierarchical planner for autonomous vehicles, as part of the Udacity Self-Driving Cars Nanodegree. It demonstrates the practical application of behavioral and motion planning techniques, and is intended to serve as a portfolio piece for potential recruiters.

Project Overview
In this project, I implemented two crucial components of a traditional hierarchical planner: the Behavior Planner and the Motion Planner. These components work together to achieve the following objectives:

Avoid Static Objects: The vehicle is capable of avoiding static objects (e.g., parked cars, bicycles, trucks) that may invade the lane. The vehicle can execute maneuvers such as “nudges” or “lane changes” to prevent collisions.

Handle Intersections: The vehicle can navigate various types of intersections (3-way, 4-way intersections, and roundabouts) by stopping at all of them by default.

Track Lane Centerline: The vehicle accurately tracks the centerline of the traveling lane.

Key Implementations
Behavioral Planning: Implemented using Finite State Machines (FSM).
Static Objects Collision Checking: Developed logic to detect and avoid collisions with static objects.
Path and Trajectory Generation: Utilized cubic spirals to generate paths and trajectories.
Trajectory Selection: Evaluated trajectories using a cost function that balances collision avoidance and lane centerline adherence.
Dependencies
The project was developed using the Udacity VM workspace. For a local setup, ensure the following tools are installed:

CARLA simulator 0.9.9.4
NICE DCV Server
C++ (GCC 9.4.0 or above)
Git
OpenCV
CMake and Make
VSCode
Eigen Library for C++
Point Cloud Library
Python3 and Pip v20.xx or above
ROS
Project-specific dependencies (details provided in the original instructions)
Instructions
Step 1: Log into VM Workspace
Open the VM workspace and log in to practice the current project.

Step 2: Clone the Repository
Fork the repository to your GitHub account and clone it:

bash
Copy code
git clone https://github.com/udacity/nd013-c5-planning-starter.git
Change to the project directory:

bash
Copy code
cd nd013-c5-planning-starter/project
Step 3: Review the Starter Files
Review the files in the project directory, including:

behavior_planner_FSM.cpp
cost_functions.cpp
motion_planner.cpp
velocity_profile_generator.cpp
planning_params.h
Step 4: Start the Carla Server
Start the Carla server:

bash
Copy code
./run_carla.sh
Step 5: Install Dependencies
Open another Terminal tab, navigate to the project directory, and install dependencies:

bash
Copy code
./install-ubuntu.sh
Step 6: Update the Project Code
Navigate to the starter_files/ directory and update the necessary files. Ensure your changes align with the rubric criteria.

Step 7: Build and Execute the Project
Build the project:

bash
Copy code
cd starter_files
cmake .
make
Run the project:

bash
Copy code
cd ..
./run_main.sh
Handle any errors as described in the original instructions.

Step 8: Portfolio Project
This project is now a completed portfolio piece, showcasing skills in motion planning and decision-making for autonomous vehicles. It is part of the Udacity Self-Driving Cars Nanodegree.

Ensure that the project meets all rubric criteria before submitting it to your portfolio or showcasing it to potential recruiters.
