Introduction

 This project aims to provide a flexible and portable environment for simulating the behavior of a mobile robot in various scenarios. Gazebo, a powerful robotics simulation tool, is employed to create realistic environments, while Docker ensures easy setup and reproducibility across different systems.

Key Features:

Gazebo Simulation: Utilize the capabilities of Gazebo to simulate a mobile robot in diverse environments.

Docker Containerization: Achieve a consistent and isolated simulation environment through Docker containers.

Purpose:

This repository serves as a foundation for developing and testing mobile robot algorithms in a controlled and virtual environment. 

Simulation Models: Explore different robot models and simulated worlds.

Docker Configuration: Easily set up the simulation environment using Docker containers.


Docker simplifies the setup process by encapsulating the simulation environment and its dependencies. This ensures a consistent experience across different platforms without the need to worry about software conflicts.

Getting Started:

Follow the documentation to set up the simulation environment, run the simulation, and explore the possibilities of mobile robot development in a virtual space.

2. Prerequisites
   
Before diving into the mobile robot simulation, ensure that your system meets the following prerequisites.

Software Requirements:
Docker: Install Docker on your machine by following the instructions for your operating system. Visit Docker Installation for detailed guidance.

Docker Compose: If not included with your Docker installation, install Docker Compose to manage multi-container Docker applications. Refer to Docker Compose Installation for the installation steps.

XLAUCH - If you are using Windows machine the GAZEBO and other GUI based applications will need a screen output so you need X lauch.

3. Installation

Create a folder on your machine then copy the file from this repo to your folder

then build the dacker image from within the folder using the command < docker build -t <image_name> .

this will build the image nessesary to build the image for the simulation consisting of all nessesay dependacies

4. setup

Once the image is built, setup a container to run the image using the command, docker run -it <imagename> 

At this stage you are insde a container to run all the simulation where all nessesay files are available.

5. Go to the root folder and excute the command catkin_make

6. Once you are here, excute git branch to see three branches, each branch represent different world where the mobile robot is spawned.

7. Openup a terminal and source to the ros directory /catkin_ws/devel/setup.bash

8. run ros core

9. then open up another terminal and run -  roslaunch robot_model_pkg robot_xacro.launch

10. make sure you installed Xlaunch and open the xlauch window

11. You shoulbe able to see the simulation at this point

12. To move between the enviroments, use -- git branch --command and see between the list and then hit git checkout <branch_name> then use the same step to run the simlation.

This project presents a mobile robot simulation environment utilizing Gazebo and Docker for easy setup and reproducibility. The simulation, designed as a foundation for developing and testing mobile robot algorithms, offers diverse robot models and simulated worlds. Prerequisites include installing Docker and Docker Compose, with additional considerations for XLaunch on Windows. After creating a folder, users can build the Docker image, set up a container, and run the simulation. The provided branches represent different worlds, and by switching between them, users can explore and test the robot's behavior in various environments.
