# My Trainyard

This README file is for a significant school project that I have worked on. While the project's full codebase isn't included here due to specific requirements, this README serves as an essential guide to understanding the project's objectives, methodology, and outcomes.

## Description:
The Trainyard project is a program developed in C++ that simulates a trainyard management system. It provides functionalities for managing trains and tracks within the trainyard. The program includes classes for Train and RailTrack, representing trains and tracks, respectively.

The Train class represents a train in the trainyard. Each train has a unique identifier, cargo name, engine, caboose, and a variable number of train cars. The Train class provides methods for adding and removing train cars, as well as unloading cargo. The RailTrack class represents a track in the trainyard. Each track has a queue of trains waiting to be processed. It also provides a method for adding trains to the queue and a method for processing trains.

## Requirments: 
1. Train System Enhancement Objective:
    - Develop advanced control and monitoring capabilities for the train yard's basic train system to provide detailed information about each train car's cargo content and occupancy.

2. Current System Limitations:
    - Improve the existing train system, which lacks comprehensive details about train cars, such as passenger count or material quantity. Currently, only limited information, like unloading time, cargo content, and fullness level, is available.

3. Detailed Information Extraction:
    - Modify the code to print the quantity of passengers or the amount of material in each train car upon unloading cargo. The information should be displayed individually for each train car.

4. Final Processing Output:
    - Implement code to print the total number of train cars processed once all cargo has been unloaded from the train. This final count should accurately represent the number of train cars involved in cargo unloading.

5. Linked-List Redefinition:
    - Redefine the existing train class as a linked-list structure to accommodate advanced control and monitoring features.
    - Create a custom linked list implementation to represent each train car as a node in the list.

6. Engine and Caboose Consideration:
    - Recognize that the engine and caboose are standard components in every train, but they don't impact the linked list structure or train car count.

7. Random Train Generation:
 - During train creation:
    a. Generate a random number of cars in each train.
    b. Assign a random quantity of cargo/passengers to each train car.
    c. Randomly determine whether each car holds cargo or passengers.

8. Test Case Development:
    - Create test cases exclusively for the implemented linked-list structure to ensure its functionality and accuracy. These tests should validate the train car representation using the linked-list approach.

## Challenges Faced:
During the development of this program, the following challenges were encountered:
* One challenge faced during the development of the Trainyard program was the discrepancy in the number of cars processed between the Trainyard and Train classes. The Trainyard's carCount variable always printed as 0, while the Train class correctly tracked the number of processed cars within the unloadCargo() function. 

## How to Run the Program:
To run the Trainyard program, follow these steps:
1. Ensure you have a C++ compiler installed on your system.
2. Download the program source code files (Trainyard.h, Train.h, TrainYard.cpp, Train.cpp) as well as the other files (main.cpp, test.h, test.cpp) and place them in the same directory.
3. Compile the program using the makefile: ```make trainyard```
4. Run the compiled executable: ```./trainyard```
5. The program will execute various tests to verify its functionality. The test results will be displayed in the console, indicating whether each test passed or failed.

## Overview/Workflow of the Code and its Functionality:
The workflow of the Trainyard program is as follows:
1. The trainyard and tracks are created, and trains are added to the tracks queues.
2. The trainyard starts processing the trains on each track.
3. For each track, the trainyard dequeues a train and begins processing it.
4. The train's cargo is unloaded by iterating through each train car and printing their details.
5. After unloading the cargo, the train is marked as unloaded, and its details, including the total number of train cars processed and the total number of train cars, are printed.
6. The trainyard moves on to the next train in the track's queue and repeats the process until all trains have been processed.
7. Once all trains have been processed on all tracks, the trainyard waits for the trains to clear the platforms.
8. Finally, the trainyard prints the total number of trains processed and the total number of trains scheduled.
