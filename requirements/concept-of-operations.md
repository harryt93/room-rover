# Room Rover Concept of Operations

## Scenario 1: Box in the Way

### Scenario
The rover is exploring the room. There is a large box in the way, right in the middle of the floor. As the rover approaches the box, it detects it, and moves around it. The box is reflected in the map that the rover creates.

### Derived Requirements:
The system shall mark what it thinks are temporary obstacles on the map.<br>
<i>It would be nice for the system to know what is permanently part of the environment, and what is only temporarily so. It should identify when it finds a temporary object like a box on the floor.</i>

## Scenario 2: Trodden on in the Dark

### Scenario
The rover is trundling around on the floor in the middle of the night. Person gets out of bed, and stands on the rover, breaking it.

### Derived Requirements:
The system shall not operate in darkness.<br>
<i>If it's dark, assume that the person can't see either, it's probably night. Not operating at night is the easiest way to avoid being trodden on. </i>

## Scenario 3: Starting System Operation

### Scenario
The rover is currently stopped and in hibernation mode under a desk. The user comes into the room, bends down, and pushes a button on top of the rover. The rover turns on and immediately begins to explore the room.

### Derived Requirements:
The system shall have a low power standby mode where it monitors for user commands to start.<br>
<i>Turning the rover on should be as easy as commanding it to start exploring. It should be waiting, ready to start exploring as soon as the user requests it to. </i>

## Scenario 4: Trapped in a Room

### Scenario
The rover is exploring a room. The door is shut, trapping the rover in the room. It continues to explore the room, and simply updates the map to show the door is closed. It doesn't specifically recognise that it is trapped.

## Scenario 5: Stuck

### Scenario
The rover is exploring a room, and travels over a pile of clothes on the floor. It tips up slightly and it's wheels no longer touch the floor, and it gets stuck. It recognises that it's spinning it's wheels, but that there is no change in location, so it assumes it is stuck. It attempts to escape by reversing and moving forward a few times, but it doesn't escape. It stops, and signals that it is stuck.

### Derived Requirements:
The system shall detect when it gets stuck.<br>
<i>The system should recognise when it gets stuck so that it can make some attempt to get loose.</i><br><br>
  
The system shall attempt to free itself when stuck.<br>
<i>The system should attempt to free itself so that it can continue to explore the room autonomously. </i><br><br>

The system shall signal if it is truly stuck.<br>
<i>If the system is truly stuck and can't escape, it should let the user know so that it can be freed.</i><br><br>
  