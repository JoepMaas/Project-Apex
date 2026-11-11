# Functional design document 
## Project-Apex

### Rc Car
* The vehicle must have an F1-inspired design.
* The vehicle must be controlled by an ESP32.
* The vehicle must receive wireless commands from the controller.
* Steering must be controlled using a servo motor.
* Propulsion must be provided by a brushless motor.
* Motor speed must be controlled through an ESC.
* The vehicle must support controlled acceleration and braking.
* The vehicle must have four wheels.
* The chassis and bodywork must be custom-designed.
* Loss of communication must trigger a defined safe state.

### Controler
* The controller must have a custom-designed enclosure.
*	The controller must use an ESP32.
*	The controller must communicate wirelessly with the RC car.
*	The controller must provide steering input.
*	The controller must provide acceleration input.
*	The controller must provide braking input.
*	Driver inputs must be processed and transmitted in real time.
*	The controller must indicate whether a connection is established.
*	The controller must have its own power supply.
*	The controller must support a safe response when communication is lost.

### Track
*	The track must have a custom-designed circuit layout.
*	The track must contain electronic sensors.
*	Sensors must detect the RC car at designated positions.
*	Sensor measurements must provide information about racing-line accuracy.
*	The track must detect start/finish line crossings.
*	Lap times must be measured accurately.
*	Track data must be transmitted to the scoring system.
*	The track must support multiple laps per race.
*	The system must distinguish valid detections from duplicate or invalid readings.

### Scoring System
*	The system must receive data from the track.
*	The system must calculate racing-line precision scores.
*	The system must reward measurements closer to the preferred racing line.
*	The system must calculate individual lap times.
*	The system must calculate total race time.
*	The system must calculate the total driver score.
*	The system must maintain a leaderboard.
*	The leaderboard must be displayed on an external monitor.
*	The leaderboard must update during a race.
*	The system must store completed race results.
*	The system must associate results with the correct driver.
*	The system must handle missing or invalid sensor measurements.