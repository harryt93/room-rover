# Room Rover Concept of Operations

## Scenario 1: Box in the Way

### Scenario
The rover is exploring a room autonomously. There is a large box in the way of it's path, right in the middle of the floor. As the rover approaches the box, it detects it, and moves around it. The box is reflected in the map that the rover creates as a temporary obstacle.

### Derived Requirements:
The system shall dectect and navigate around obstacles in it's path.<br>
<i>The Rover should automatically detect obstacles in it's path, and navigate around them.</i><br>

The system shall mark temporary obstacles on it's map.<br>
<i>It would be nice for the system to communicate what is permanently part of the environment, and what is only temporarily so. It should identify when it finds a temporary object like a box on the floor.</i>

## Scenario 2: Trodden on in the Dark

### Scenario
The rover is moving around on the floor in the middle of the night. A person moving around in the darkness stands on the rover, breaking it.

### Derived Requirements:
The system shall not operate in darkness.<br>
<i>If it's dark, assume that the person can't see either, it's probably night. Not operating at night is the easiest way to avoid being trodden on. </i>

## Scenario 3: Starting System Operation

### Scenario
The rover begins in a shutdown state. The user activates the rover. The rover turns on, does a system check, confirms that all it's systems are functioning, and begins to explore the room.

### Derived Requirements:
The Rover shall perform a start up check to confirm that it's functioning properly.
<i>Performing a start up check will allow the Rover to catch problems before it begins to move.</i>

## Scenario 4: Failed Start

### Scenario
The rover begins in a shutdown state. The user activates the rover. The rover turns on, does a system check, and detects a low battery. It communicates a failed start status to the user and then awaits shutdown.

### Derived Requirements:
The Rover shall communicate a failed start status to the user if a system check detects a problem.
<i>The Rover should alert the user to any problems it finds.</i>

## Scenario 5: Stuck

### Scenario
The rover is exploring a room autonomously, and travels over a pile of clothes on the floor. It tips up slightly and it's wheels no longer touch the floor, and it gets stuck. It recognises that it's spinning it's wheels, but that there is no change in location, so it assumes it is stuck. It attempts to escape by reversing and moving forward a few times, but it doesn't escape. It stops, signals that it is stuck, and awaits shutdown.

### Derived Requirements:
The system shall detect when it gets stuck.<br>
<i>The system should recognise when it gets stuck so that it can make some attempt to get loose.</i><br><br>
  
The system shall attempt to free itself when stuck.<br>
<i>The system should attempt to free itself so that it can continue to explore the room autonomously. </i><br><br>

The system shall signal if it is truly stuck.<br>
<i>If the system is truly stuck and can't escape, it should let the user know so that it can be freed.</i><br><br>

## Scenario 6: Communicating the Map

### Scenario
The Rover is exploring a room autonomously, at regular intervals when it detects a connection, it connects to a computer and transmits it's representation of the internal map.

### Derived Requirements:
The system shall transmit data when it detects a suitable connection.
<i>The system should automatically pick up a connection and send it's map data over that connection if it's strong enough.</i><br>

The system shall transmit it's internal map to a computer.
<i>The system itself does not need to display the map, but it must communicate it to a computer on the network.</i>
