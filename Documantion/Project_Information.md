# PROJECT APEX

## Document information	
- Project 	| Project Apex
- Version |	 1.0
- Status |	 Beta
- Main controller |	 ESP32
- CAD software | Autodesk Fusion 360
- Programming |	 Arduino
- Planning | [My Planning App](https://github.com/JoepMaas/Planning-Website)
- Manufacturing | 3D printing

## About
This project consists of four main subsystems: the RC car, a custom wireless controller, a interactive racing track, and a scoring system with a live leaderboard.

The vehicle and its supporting infrastructure will be custom-designed, with 3D printed components and ESP32 microcontrollers handling the electronic control and communication.

The objective is to create a complete miniature motorsport experience where drivers are evaluated on both their racing speed and racing line precision.

## Main objectives
- Design and manufacture a custom F1 inspired RC car.
- Develop a custom wireless controller.
- Build a racing track equipped with sensors.
- Implement accurate lap time measurement.
- Develop a scoring system that rewards racing-line precision.
- Display race results on an external monitor.
- Integrate all subsystems into one connected platform.

# DESCRIPTIONS OF THE MAIN PROJECTS
## RC car
The RC car will be a custom designed, F1 inspired vehicle. Its chassis, bodywork and mechanical components will be designed in Autodesk Fusion 360 and manufactured using 3D printing.

An ESP32 microcontroller will act as the main control unit, receiving commands from the custom controller and translating them into steering, acceleration and braking inputs.

The vehicle will be equipped with four wheels, a battery, a steering mechanism, a propulsion system and wireless communication hardware.

## Controller
The custom controller will be designed to provide the driver with complete control over the RC car.

It will feature an ESP32 microcontroller responsible for interacting with the rc car and transmitting control commands wirelessly to the vehicle, via joysticks and buttons.

The controller will have dedicated inputs for steering, acceleration and braking. Its enclosure will be custom-designed in Fusion 360 and manufactured using 3D printing

## RC track
The RC track will be a custom designed racing circuit equipped with electronic sensors.

The track will be responsible for detecting the RC car's position at designated locations, measuring its lap times and collecting information about its racing line.

Sensors will be positioned at selected points around the circuit. Their measurements will be used by the scoring system to evaluate how closely the vehicle follows the intended racing line.

The track infrastructure will communicate with the scoring system to provide the necessary race data.

## Scoring System
The scoring system will be responsible for evaluating driver performance throughout a race.

Unlike a traditional RC racing system that focuses exclusively on lap times, Project Apex will introduce an additional scoring mechanic based on racing line precision.

The track sensors will measure how closely the vehicle follows the preferred racing line. Drivers will receive points based on these measurements.

Lap times will also be recorded and incorporated into the race results.

All results will be processed and displayed on an external monitor through a leaderboard interface.

### Scoring algorithm prototype

#### total = score + time

- score = how close the car went to the sensor (the closer the higher)
- time = time will start when you go over the finish line and end on the second time.

This will be refined upon further testing.