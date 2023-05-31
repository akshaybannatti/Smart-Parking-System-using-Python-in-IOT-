# Smart-Parking-System-using-Python-in-IOT-

**This code assumes the use of a Raspberry Pi and ultrasonic sensors to detect the presence of vehicles in parking spaces. It uses Python programming language and the RPi.GPIO library for GPIO (General Purpose Input/Output) control.**

This code uses an ultrasonic sensor connected to the Raspberry Pi to measure the distance between the sensor and an object (e.g., a vehicle). The measure_distance() function sends a pulse and measures the time it takes for the pulse to return, which is then converted into distance.

The is_parking_space_available() function compares the measured distance with a threshold value to determine if a parking space is available. If the distance is greater than the threshold, it considers the space as available; otherwise, it assumes the space is occupied.

The main() function continuously checks the availability of the parking space using the ultrasonic sensor and prints the corresponding message. It repeats this process every 5 seconds until the program is interrupted.

Remember to connect the ultrasonic sensor correctly to the Raspberry Pi and adjust the TRIGGER_PIN, ECHO_PIN, and threshold_distance values based on your specific setup. Additionally, make sure to install the RPi.GPIO library if it's not already installed using the command pip install RPi.GPIO.


# Smart Parking System using IoT

This project implements a basic smart parking system using IoT. The system utilizes ultrasonic sensors connected to a Raspberry Pi to detect the presence of vehicles in parking spaces. The availability of parking spaces is monitored and displayed in real-time.

## Hardware Requirements

- Raspberry Pi (any model)
- Ultrasonic sensors (HC-SR04 or similar)
- Jumper wires
- Breadboard (if necessary)
- Power supply for the Raspberry Pi
- Computer or device with internet access

## Software Requirements

- Python 3.x
- RPi.GPIO library

## Installation

1. Connect the ultrasonic sensors to the Raspberry Pi's GPIO pins according to the wiring diagram provided.
2. Install the RPi.GPIO library by running the following command:

   ```shell
   pip install RPi.GPIO

**Usage**
1. Clone or download the code from this GitHub repository.

2. Open a terminal or command prompt and navigate to the project directory.

3. Run the following command to start the smart parking system:

**Shell Command**
python smart_parking_system.py

4. The system will continuously monitor the availability of parking spaces and display the status in the terminal.

**Customization**
If your ultrasonic sensors are connected to different GPIO pins, modify the TRIGGER_PIN and ECHO_PIN constants in the code accordingly.
Adjust the threshold_distance value in the code to set the desired distance threshold for considering a parking space available or occupied.
You can customize the code to integrate it with other IoT platforms or add additional features as per your requirements.

**Contributing**
Contributions to this project are welcome! If you find any issues or have ideas for improvements, please submit an issue or a pull request.

**License**
This project is licensed under the MIT License.
