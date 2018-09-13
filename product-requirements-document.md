## System Attributes
<b>NFS_01: </b>Low Cost<br>
<i>I don't want to spend loads on this, it's only supposed to be a replacement for a Udacity course.</i><br><br>

<b>NFS_02: </b>Large Growth Capacity<br>
<i>I want to be able to add things to it later on when I learn new technologies or have other ideas.</i><br><br>

<b>NFS_03: </b>High Reliability<br>
<i>I don't want to have to be repairing it all the time.</i><br><br>

<b>NFS_04: </b>High Durability<br>
<i>I don't want to have to be super careful when I'm around it. Since it's autonomous, it should be fairly robust to accidents, drops, things falling on it etc.</i><br><br>

<b>NFS_05: </b>High Maintainability<br>
<i>If anything goes wrong, I want to be able to fix it fairly easily.</i><br><br>

<b>NFS_06: </b>Exciting<br>
<i>I want to be able to show it off to people at interviews, to friends, and at work. It's got to be reasonably cool for that.</i><br><br>

## Functional Requirements
### Sense Environment
### Traverse Environment
<b>NFP:</b> The rover should be able to map a room with floor space 5m^2 by 5m^2 in one hour.<br>
<i>Since the rover is autonomous, it's not essential that it map quickly. As long as it doesn't take forever.</i><br><br>
<b>Trace:</b><br>
<b>Verification Activity:</b><br>
<b>Verification Outcome:</b>

### Map Environment
<b>NFI:</b> The rover shall send it's internal map to a PC for visualisation.<br>
<i>I want to be able to see the map that it produces. The actual software to visualise the map needs to be written too, but that's a separate project.</i><br><br>
<b>Trace:</b><br>
<b>Verification Activity:</b><br>
<b>Verification Outcome:</b>

<b>NFI:</b> The system shall mark what it thinks are temporary obstacles on the map.<br>
<i>It would be nice for the system to know what is permanently part of the environment, and what is only temporarily so. It should identify when it finds a temporary object like a box on the floor.</i><br><br>
<b>Trace:</b> CONOP1<br>
<b>Verification Activity:</b><br>
<b>Verification Outcome:</b>

### Manage Rover
<b>NFP:</b> The rover shall not operate in darkness.<br>
<i>I don't want the rover to operate at night because of the noise of it being in the room. Also, there is a danger of standing on it in the dark.</i><br><br>
<b>Trace:</b> CONOP2<br>
<b>Verification Activity:</b><br>
<b>Verification Outcome:</b>

<b>NFI:</b> The system shall have a low power standby mode where it monitors for user commands to start.<br>
<i>Turning the rover on should be as easy as commanding it to start exploring. It should be waiting, ready to start exploring as soon as the user requests it to.</i><br><br>
<b>Trace:</b> CONOP3<br>
<b>Verification Activity:</b><br>
<b>Verification Outcome:</b>

