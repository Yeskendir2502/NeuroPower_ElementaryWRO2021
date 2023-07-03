# NeuroPower: Wireless Charging System for Electric Vehicles Mentoring Elementary team (8-12 years)
## Introduction
Nowadays, one of the global problems is CO2 emissions, and therefore people are looking for different solutions, one of which is the use of electric cars. However, not every city has a sufficient charging infrastructure. For example, in Britain, the government plans to ban the sale of new cars with gasoline and diesel engines from 2030, but the demand for electric vehicles is limited by a lack of charging infrastructure.

Unlike conventional cars that can be refueled in a matter of minutes, electric cars take a significantly longer time to charge. For example, the famous Tesla Model S takes as much as 24 hours to fully charge. This charging time inconvenience hinders the widespread adoption of electric vehicles. However, with our NeuroPower system, we can charge electric cars on the go, eliminating the need for long charging times. This is a groundbreaking solution!

To encourage people to transition to green energy and protect the environment, we present the NeuroPower system, a wireless charging system for electric vehicles.

## Solution
NeuroPower is an autonomous and automatic charging system for electric cars on the go. It consists of two main components:

Camera-based Charging: We install solar panels on the roof of electric cars, which are monitored by a camera system. The camera uses lasers to accurately guide the charging beams onto the solar panels, enabling charging while the vehicles are in motion.

Inductor-based Charging: We deploy inductors on the road, which utilize electromagnetic induction to wirelessly charge electric cars. The inductors act as transmitters on the road, while the electric cars are equipped with receivers on their bottom side. Electricity is transferred from the inductors to the cars through electromagnetic induction, providing continuous wireless charging capabilities.

Our project's mechanism involves the simultaneous use of inductors for wireless charging from the road and a camera system with lasers for charging from the air. The camera system utilizes a yolov4 convolutional neural network to monitor the position of electric cars and ensure accurate charging.

## Code
### EV3 Loop Code:
The EV3 loop code runs an infinite loop in which the brightness of two color sensors is continuously compared, and the corresponding motors are controlled accordingly.

### Arduino Loop Code:
The Arduino loop code continuously receives data via the COM port from the laptop and adjusts the brightness of the LED correspondingly.

### Python Code:
The Python code is responsible for image processing using the OpenCV library. It loads the yolov4-tiny-custom model, which has been trained on a dataset of 1000 photos. The code takes a frame from the video stream, detects the object of interest (electric car roof), and calculates its coordinates. Based on the coordinates, the camera is adjusted to keep the object in the center. The code communicates with the Arduino microcontroller to control the EV3 camera's rotation using LEDs.

## Conclusion
The NeuroPower system offers a revolutionary solution for charging electric vehicles on the go. By combining camera-based charging with inductor-based charging, we provide a seamless and efficient charging experience. With our system, electric cars can be charged wirelessly while in motion, eliminating the need for long charging times and expanding the usage of electric vehicles. By implementing NeuroPower, we aim to promote the adoption of electric cars and contribute to a greener future.

Thank you for your attention!

Team Members:

Aruzhan Kuanyshbai
Yelzhan Tama
