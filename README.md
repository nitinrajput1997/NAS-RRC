# NAS-RRC
SDAp is unique for User-Plane Protocol Stack . Similarly RRC and NAS are unique to Control-Plane Protocol Stack. They are responsible for connection set up, mobility and security related functions.

**NAS(UE-AMF)**<br />
NAS function operate between AMF in core network and the device. It includes following functions NAS(Non-Access Stratum):-<br />
1. Authentication<br />
2. Security<br />
3. Idle-Mode Procedures(Paging)<br />
4. Assigning IP Addresses to the devices<br />

**RRC(UE-gNB)**<br />
It operates between RRC in gNB and RRC in UE. It is responsible for handling the RAN related control-plane procedures such as<br />
1. System Inforamtion Broadcast<br />
2. Paging<br />
3. Connection Management<br />
4. Mobility Functions<br />
5. Measurement Configuration and reporting<br />
6. handling of devices capabilities<br />

In NR there are 3 states of RRC:-<br />
1. RRC Idle<br />
2. RRC Connected<br />
3. RRC Inactive<br />

The **RRC Idle** are used soon aftre the device is powered ON or when the device first enter to the coveerage area of network.

In RRC Idle there is no RRC context that means there is no necessary parameter for communication between the UE/device and network.

The necessary parameter that are esrablished as apart of connection preocedure, hepls with the communication between the UE/device and network.But in Idle State,these information is not yet available. And the device does not belong to any specific cell yet.

No data transfer take place because the device just sleeps most of the time to reduce the batter consumption in this state. It periodically wakes up to receive paging information if there is any paging information from the network. If there is any uplink data to be sent from device then the device has to do the random access procrdure to get the UL-Synchronization scheduling.

This will leads the device from **RRC Idle to RRc Connected** State.

