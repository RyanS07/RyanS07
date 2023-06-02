# Ryan Seto

## Contact  
Resume: [Resume - Ryan Seto.pdf](https://github.com/RyanS07/RyanS07/blob/main/resume_ryanseto.pdf) \
LinkedIn: https://www.linkedin.com/in/ryan-shi-an-seto/ \
Email: [ryan.seto@mail.utoronto.ca](ryan.seto@mail.utoronto.ca)

## Projects  

### Disclaimer
A majority of my projects are from internships/research terms or school. As such, unfortunately I can't share much code here because their source codes cannot be shared publically.  

### Microbot For Line-Tracking (Arduino, AutoCAD), *For Research Term*
Designed and built a miniature robot that can follow a black line to a destination using IR sensors and an Arduino. Currently still in development.

### OSM ArcGIS Map (C++, GTK), *For School*
Created an ArcGIS application by processing *OpenStreetMap (OSM)* geolocational data into an object oriented database and displayed the user interface using GTK. Additionally, data was called from the *OpenWeatherAPI* to have live weather display. The A* path finding algorithm was also used to form routes between two selected locations (ex: your home and a grocery store). The OSM data was parsed into the following inheritance hierarchy:
- MapElement 
  - StreetSegment
  - Intersection
  - Street
  - PointOfInterest (ex: Tim Hortons, T&T Supermarket, etc.)
  - Feature (ex: building, lakes, parks, etc.) 


### Boo Hunter (C, Arm), *For School*
Created a Luigi's Mansion themed aim-labs game where the player needs to hit ghosts/boos that appear randomly around the screen. The app was written in C and could be played on a DE1-SoC board or CPUlator. User input was through PS2 keyboard interrupts and the switches and pushbuttons present on the board. The game state was managed using A9 timer interrupts.

### Music Genre Classifier (Python, TensorFlow)
Trained a convolutional neural network to predict the genre of a sample of music to 70% accuracy using TensorFlow and Keras. \
Repo Link: https://github.com/RyanS07/music-genre-classifier 

### Authentication Middleware (Python, FASTAPI), **For Work**
Designed a middleware to handle user authentication requests from the front-end by redirecting them to a central authentication server away from the back-end. By using FASTAPI dependencies, I was able to attach permissions to a back-end endpoint through decorators and a list of all the permissions a request needs. This streamlined API development and was implemented in 10+ services. 
```
@requires(["admin_permission", "this_workspace_permission"])
def some_api_endpoint(...):
    print("This is a secure endpoint!")
```
 
### Chemistry Database and Calculator (Java, JavaFX)
Created a JavaFX application that imitated my high school chemistry data sheet with some additional ideal gas law calculators. \
Repo Link: https://github.com/RyanS07/Chemistry-Database-and-Calculator

### Infrared Photobooth (Python, Flask, OpenCV), **For Work**
In this project, I built a full-stack trade show demo using Flask that could take an infrared photo of the user in exchange for their contact information. After extracting the IR camera's footage using its SDK, I processed it using OpenCV to blend with another visible light camera and create 50/50 IR/VL footage. This footage was then streamed to the front end using multithreading. 

### 1v1 Shooter Game (Java, JavaFX)
Created a JavaFX game where two players can move vertically similarly to pong but instead of bouncing a ball they try to shoot each other. \
Repo Link: https://github.com/RyanS07/JavaFX-Shooter-Game
