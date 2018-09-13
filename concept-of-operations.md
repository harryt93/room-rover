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

