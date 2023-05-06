
# Drogon
Drogon is an IoT-Based Quadcopter for Toxic Gas Detection and Sampling

### Introduction:
Drogon is a multipurpose quadcopter designed for industrial applications, particularly for detecting toxic gases and environmental conditions. The project aims to prevent industrial accidents by routinely surveying areas and indicating if there are any toxic or harmful substances present. The quadcopter is also equipped with a robotic claw for taking soil and water samples for further inspection. The usage of a drone reduces the need for human interaction with the toxic substances, making the process much safer.

### Hardware Build:
Drogon is built using lightweight material, a brushless DC motor, 30A Electronics Speed Controller, Pixhawk flight controller, RF remote control and receiver, Li-ion battery module, and an action camera for live video streaming. It also has a Raspberry Pi 4, GPS module, GSM module, and sensors for detecting toxic gases and environmental conditions. The drone communicates with the remote cloud storage and sends data through an IoT protocol.

### Methodology:
The Pixhawk flight controller enables the quadcopter to run its motors and take off. The RF remote controller communicates with the RF receiver connected with the flight controller, allowing manual control of the drone. The GPS module allows the drone to be sent to a destination using a pre-defined route, lock the altitude at any level, and return to the source location.

The sensors attached to the drone collect samples from the air around it, detecting toxic gases and environmental conditions. A mobile netv2 model was trained using Pytorch framework in toxic gas datasets. The model is loaded inside the Raspberry Pi, which analyzes the collected samples and gives a verdict if the area is toxic or harmful to humans. The results are sent to a remote cloud storage accessible from any place in the world. The data is serialized and posted to an endpoint using the GSM module, which is then stored in a database. The database is accessible through a simple user interface, allowing authorized personnel to view the toxicity levels in different areas.

Drogon is also equipped with a robotic claw that can take soil and water samples for further inspection. This feature adds to the drone's multipurpose nature, making it useful for various applications.

### Conclusion:
Drogon is an innovative solution that helps prevent industrial accidents by detecting toxic gases and environmental conditions. It is designed to minimize human interaction with toxic substances, making the process safer. The quadcopter's robotic claw is a valuable addition that makes it useful for various applications. The remote cloud storage and simple user interface allow authorized personnel to view the toxicity levels in different areas, making it a valuable tool for industrial applications.
