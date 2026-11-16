# The Suspicious Stop: Tracking a Boat's Detour

**Type:** GEOINT and OSINT

> Challenge from the [OSINT Industries CTF](https://ctf.osint.industries/challenges).

## Scenario

A small boat leaving Marseille follows the same route to the same destination every day. On one particular day, it unexpectedly left its usual route and stopped at a specific location.

The detour is suspected to be linked to black-market activity. Intelligence indicates that the boat's owner met someone who arrived on a bike, and that the two then went into a nearby restaurant together.

I was given a file of NMEA 0183 data containing the boat's coordinates.
## Challenge objective
 
Identify:
 
- The name of the restaurant where they met
- Its full address

## Step 1: Plotting the trajectory

I loaded the file into [GPS Visualizer](https://www.gpsvisualizer.com/) to see the boat's path and analyse it.\
<img width="702" height="705" alt="image" src="https://github.com/user-attachments/assets/a3333555-5f2b-4887-8281-925fb27eaa50" />


## Step 2: Ruling out the usual destination

I looked at the last port and compared it with the first, to confirm the meeting did not happen there. The area around the last port is rocky for many kilometers, so nobody could have reached it by bike.\
<img width="1217" height="665" alt="image" src="https://github.com/user-attachments/assets/75881282-7ec4-4cc0-8c01-5cbf3eb8e350" />


## Step 3: The unusual stop

The detour stop is at **43.22849, 5.34874**. On the map, there is no port there, which is already suspicious.\
<img width="729" height="703" alt="image" src="https://github.com/user-attachments/assets/cbbe2b73-a1e4-4df8-bfcf-f9e09cc345ce" />


## Step 4: Looking closer

In the satellite view, the boat's stop is by the Calanque de Samena (circled), and a parking area just inland shows signs of bikes. That matches the intelligence that the suspect met someone who arrived by bike.\
<img width="1505" height="1007" alt="image" src="https://github.com/user-attachments/assets/2653d661-2ccd-4b97-af6a-44fe8026399c" />


In Street View, bikes and scooters are parked in that area. The map also shows a restaurant close by.\
<img width="1050" height="1092" alt="image" src="https://github.com/user-attachments/assets/a418eecd-ad3c-447b-af71-9fe7138d31c8" />


## Result

The closest restaurant, where they met, is at **40 Bd de la Calanque de Samena, 13008 Marseille, France**.

<sub>Trajectory plotted with GPS Visualizer, using OpenStreetMap data. Satellite and Street View imagery © Google.</sub>
