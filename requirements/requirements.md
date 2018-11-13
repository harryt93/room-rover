## System Attributes
<b>NFS_01: </b>Low Cost<br>
<i>I don't want to spend loads on this, it's only supposed to be a replacement for a Udacity course. 
Note that this is an attribute for trading off, not a specific constraint, hence no specific value. See NFS_9 for a constraint.</i><br><br>

<b>NFS_02: </b>Large Growth Capacity<br>
<i>I want to be able to add things to it later on when I learn new technologies or have other ideas.</i><br><br>

<b>NFS_03: </b>High Reliability<br>
<i>I don't want to have to be repairing it all the time.</i><br><br>

<b>NFS_04: </b>High Durability<br>
<i>I don't want to have to be super careful when I'm around it. Since it's autonomous, it should be fairly robust to accidents, drops, things falling on it etc.</i><br><br>

<b>NFS_05: </b>High Maintainability<br>
<i>If anything goes wrong, I want to be able to fix it fairly easily.</i><br><br>

<b>NFS_06: </b>Exciting<br>
<i>I want to be able to show it off to people at interviews, to friends, and at work.</i><br><br>

<b>NFS_07: </b>Provides Opportunities to Learn<br>
<i>It's important that this project stretches me and forces me to learn new things.</i><br><br>

<b>NFS_08: </b>High Performance<br>
<i>The rover should perform satisfactorily, at a reasonable speed, and generate good quality maps.</i><br><br>

## System Constraints
<b>NFS_09: </b>The total unit cost shall not exceed £2000.<br>
<i>The price of a Udacity nanodegree is about £2000, and is what I'm willing to spend.</i><br>
<i>Source: Me</i><br><br>

## Functional Requirements
### Sense Environment
<b>NFP_01:</b> The rover shall be able to sense an object of size 10cm^3.<br>
<i>I want the map to be of high quality and detail, which requires the sensing function be capable of detecting small objects. Small is arbitrary, but
intuitively, I want to be able to detect a coffee cup, which is about 10cm^3.</i><br>
<i>Source: Me</i><br><br>

<b>NFP_02:</b> The rover shall be able to sense objects up to 5m away..<br>
<i>The rover should be able to map a room of size 5m by 5m.</i><br>
<i>Source: Me</i><br><br>

### Traverse Environment
<b>NFP_03:</b> The rover shall be able to map a room with floor space 5m^2 by 5m^2 in one hour.<br>
<i>Since the rover is autonomous, it's not essential that it map quickly. As long as it doesn't take forever.</i><br>
<i>Source: Me</i><br><br>

<b>NFP_04:</b> The rover should be capable of traversing a pile of clothes 0.25 m high.<br>
<i>There may be clothes on the floor in it's path, and I don't want these to be an obstacle to the rover.</i><br>
<i>Source: Me</i><br><br>

<b>NFP_05:</b> The rover shall be able to turn on the spot.<br>
<i>In order to map the floor effectively, the rover needs good agility. This is an arbitrary requirement, but reasonable.</i><br>
<i>Source: Me</i><br><br>

### Map Environment
<b>NFI_01:</b> The rover shall send it's internal map to a PC for visualisation.<br>
<i>I want to be able to see the map that it produces. The actual software to visualise the map needs to be written too, but that's a separate project.</i><br>
<i>Source: CONOP Scenario 6</i><br><br>

<b>NFI_02:</b> The system shall mark what it thinks are temporary obstacles on the map.<br>
<i>It would be nice for the system to know what is permanently part of the environment, and what is only temporarily so. It should identify when it finds a temporary object like a box on the floor.</i><br>
<i>Source: CONOP Scenario 1</i><br><br>

### Manage Rover
<b>NFP_06:</b> The rover shall not operate in darkness.<br>
<i>I don't want the rover to operate at night because of the noise of it being in the room. Also, there is a danger of standing on it in the dark.</i><br>
<i>Source: CONOP Scenario 2</i><br><br>

<b>NFP_07:</b> The rover shall be able to operate for at least 1 hour on a single charge.<br>
<i>If I want to demonstrate it, I want the rover to keep going to at least an hour without having to recharge.</i><br>
<i>Source: Me</i><br><br>

<b>NFI_03:</b> The Rover shall perform a start up check to confirm that it's functioning properly.<br>
<i>Performing a start up check will allow the Rover to catch problems before it begins to move.</i><br>
<i>Source: CONOP Scenario 3</i><br><br>

<b>NFI_04:</b> The Rover shall communicate a failed start status to the user if a system check detects a problem.<br>
<i>The Rover should alert the user to any problems it finds.</i><br>
<i>Source: CONOP Scenario 4</i><br><br>

<b>NFP_08:</b> The system shall detect when it gets stuck.<br>
<i>The system should recognise when it gets stuck so that it can make some attempt to get loose.</i><br>
<i>Source: CONOP Scenario 5</i><br><br>

<b>NFI_05:</b> The system shall attempt to free itself when stuck.<br>
<i>The system should attempt to free itself so that it can continue to explore the room autonomously. </i><br>
<i>Source: CONOP Scenario 5</i><br><br>

<b>NFI_06:</b> The system shall signal if it is truly stuck.<br>
<i>If the system is truly stuck and can't escape, it should let the user know so that it can be freed.</i><br>
<i>Source: CONOP Scenario 5</i><br><br>

<b>NFI_07:</b> The system shall transmit data when it detects a suitable connection. <br>
<i>The system should automatically pick up a connection and send it's map data over that connection if it's strong enough.</i><br>
<i>Source: CONOP Scenario 6</i><br><br>
