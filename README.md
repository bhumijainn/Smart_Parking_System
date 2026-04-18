**IoT-Based Smart Parking System**

**Project Overview**

As urban populations grow, vehicular traffic and parking management have become issues of great concern. The Smart Parking System is an IoT-based automation project designed to eliminate the time wasted searching for parking slots and reduce the manual labor required for parking management. This fully automated system senses vehicles at entry and exit points, dynamically allocates parking slots based on vacancy, and provides real-time occupancy updates.

By integrating hardware sensors with a microcontroller and computer vision, this project serves as a comprehensive solution for modern, efficient, and user-friendly parking facilities.

**Key Features**

Automated Access Control: Uses ultrasonic sensors and servo motors to automatically open gates upon vehicle detection, removing the need for manual labor.

Real-Time Occupancy Tracking: IR sensors deployed at each parking slot monitor availability and instantly update the system.

Capacity Management: A built-in counter increments upon entry and decrements upon exit. If the system reaches its maximum capacity, the entry gate will remain closed.

Vehicle Categorization (Computer Vision): Utilizes a camera and image processing to categorize vehicles by size (cars, bikes, SUVs), allowing for optimized slot allocation (e.g., heavy vehicles on the ground floor).

Mobile App Integration: Users can pre-book parking slots and view availability remotely via a dedicated Android application.

Simultaneous Operations: Capable of handling multiple entry and exit points simultaneously across different parking floors.

 **Hardware Components**
 
STM32FC103 Microcontroller: The central processing unit of the system where the control logic is executed.

Ultrasonic Sensors: Placed at entry and exit gates to detect the presence and distance of approaching vehicles.

IR Sensors: Installed in individual parking slots to detect whether a space is empty or occupied.

Servo Motors: Act as the automated barrier shafts for the entry and exit gates.

Camera Module: Captures live feeds for size and weight detection using image processing.

LCD Display (Nokia 5110): Displays the current slot vacancies to the drivers on-site.

 **Software & Technologies**
 
Arduino IDE: Used for firmware development and programming the STM32 microcontroller.

Python (Anaconda & OpenCV): Powers the image processing algorithms for vehicle categorization.

Thunkable Classic: Used for the rapid development of the Android mobile companion app.

**System Architecture & Working**

Entry Protocol: When a vehicle arrives at the entrance, the Ultrasonic (UV) sensor detects it. If the parking lot has not reached its maximum capacity, the microcontroller signals the entry Servo Motor to rotate 90 degrees, opening the barrier.

Occupancy Detection: As the vehicle parks, an IR sensor at the specific slot registers the object (using a calibrated analog threshold). The system updates the localized LED indicators and the main LCD display.

Exit Protocol: When a vehicle approaches the exit, the exit Ultrasonic sensor detects it, opening the exit Servo Motor barrier.

Capacity Counter: The system simultaneously updates the internal capacity counter—incrementing upon entry and decrementing upon exit.

**Applications**

Corporate Offices & Business Parks

Shopping Malls & Retail Centers

Hospitals

Amusement Parks & Event Venues

Nikita Patel
