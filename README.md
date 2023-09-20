# Ryan Seto

## Contact  
Resume: [Resume - Ryan Seto.pdf](https://github.com/RyanS07/RyanS07/blob/main/Software_Resume___Ryan_Seto.pdf) \
LinkedIn: https://www.linkedin.com/in/ryan-shi-an-seto/ \
Email: [ryan.seto@mail.utoronto.ca](ryan.seto@mail.utoronto.ca)

## Projects  

### Disclaimer
A majority of my projects are from internships/research terms or school. As such, I cannot share any of their source code publically and I can only share samples of the projects.  

### Raspberry Pi Cluster For Solving Linear Systems in Parallel (Docker, Python, Flask, Linux), *For Research Term*
Provisioned a Raspberry Pi cluster using Docker Swarm to solve linear systems in parallel by deploying a Flask server to take requests to solve linear systems. The request would be processed into multiple tasks which would be published to a Redis Pub/Sub pipeline (message queue) for worker containers to consume. Workers would then solve and return determinants back to the Flask server for individual variables to be solved via Cramer's Rule. 

RPI Cluster Pipeline





to solve linear systems in parallel by deploying a Flask server that published tasks to a message queue with Docker Compose, and distributed asynchronous jobs across workers in a Docker Swarm

### Line-Tracking Arduino Robot Workshop (Arduino, AutoDesk Fusino 360), *For Research Term*
Designed and taught an 8-day workshop teaching first year electrical and computer engineering (ECE) students at UofT how to CAD, wire, and program an Arduino-controlled robot to follow a black line. ***The workshop was such a success that the Chair of the ECE Department at UofT offered to support the workshop in future with a dedicated facility and full funding.***

The workshop started with 3 days of involved lessons teaching the students:
- How to use Fusion 360 to design their own robot body
- How a microcontroller (MCU) works and the available communication protocols (UART, SPI, I2C)
- How to program their MCU with Arduino to read input from sensors and control motors (Analog, Digital, and PWM Pins)

Students were then given 5 days to design and implement their own robot designs with the teaching team's help where necessary to compete on a circuit-themed course. Their CAD designs where passed to a 3D printing lab at UofT to manufacture their robot bodies. The final track and each team's robots can be seen below:

Final Competition Field
![alt text](https://github.com/RyanS07/RyanS07/blob/main/images/MicRobotics%20Field.jpg) 

Student Designs
![alt text](https://github.com/RyanS07/RyanS07/blob/main/images/MicRobotics%20Teams.jpg)

### HomeCook+ (C++, GTK), *For School*
Created an ArcGIS application by processing *OpenStreetMap (OSM)* geolocational data into an object oriented database and displayed the user interface using GTK. The OSM data was parsed into the following inheritance hierarchy:
- MapElement 
  - StreetSegment
  - Intersection
  - Street
  - PointOfInterest (ex: Tim Hortons, T&T Supermarket, etc.)
  - Feature (ex: building, lakes, parks, etc.) 

Additionally, data was requested from the *OpenWeatherAPI* to have live weather display. The A* path finding algorithm was also used to form routes between two selected locations (ex: your home and a grocery store). 

HomeCook+ GUI
![alt text](https://github.com/RyanS07/RyanS07/blob/main/images/HomeCook%2B%20Sample.png) 

### Boo Hunter (C, Arm), *For School*
Created a Luigi's Mansion themed aim-labs game where the player needs to hit ghosts/boos that appear randomly around the screen. The app was written in C and could be played on a DE1-SoC board or CPUlator. User input was through PS2 keyboard interrupts and the switches and pushbuttons present on the board. The game state was managed using A9 timer interrupts.

Boo Hunter Title Screen
![alt text](https://github.com/RyanS07/RyanS07/blob/main/images/Boo%20Hunter%20Title%20Screen.png) 

Boo Hunter In Game Screen
![alt text](https://github.com/RyanS07/RyanS07/blob/main/images/Boo%20Hunter%20In%20Game.png) 

### Music Genre Classifier (Python, TensorFlow)
Trained a convolutional neural network to predict the genre of a sample of music to 70% accuracy using TensorFlow and Keras. \
Repo Link: https://github.com/RyanS07/music-genre-classifier 

### Authentication Middleware (Python, FASTAPI), *For Work*
Designed a middleware to handle user authentication requests from the front-end by redirecting them to a central authentication server away from the back-end. By using FASTAPI dependencies, I was able to attach permissions to a back-end endpoint through decorators and a list of all the permissions a request needs. This streamlined API development and was implemented in 10+ services. 
```
@requires(["admin_permission", "this_workspace_permission"])
def some_api_endpoint(...):
    print("This is a secure endpoint!")
```
 
### Chemistry Database and Calculator (Java, JavaFX)
Created a JavaFX application that imitated my high school chemistry data sheet with some additional ideal gas law calculators. \
Repo Link: https://github.com/RyanS07/Chemistry-Database-and-Calculator

### Infrared Photobooth (Python, Flask, OpenCV), *For Work*
In this project, I built a full-stack trade show demo using Flask that could take an infrared photo of the user in exchange for their contact information. After extracting the IR camera's footage using its SDK, I processed it using OpenCV to blend with another visible light camera and create 50/50 IR/VL footage. This footage was then streamed to the front end using multithreading. 

### 1v1 Shooter Game (Java, JavaFX)
Created a JavaFX game where two players can move vertically similarly to pong but instead of bouncing a ball they try to shoot each other. \
Repo Link: https://github.com/RyanS07/JavaFX-Shooter-Game
