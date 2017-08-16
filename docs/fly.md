---
currentMenu: fly
---

# Fly

## Mission preparation

Steps for the day(s) prior to when you are planning to fly.
- Research the place you plan to fly
  - Know (and obey) any regulations, flight restrictions, etc.
      - Federal Aviation Adminstration (FAA) rules on UAS [<i class="fa fa-fw fa-external-link"></i>](https://www.faa.gov/uas/)
      - Academy of Model Aeronautics (AMA) [<i class="fa fa-fw fa-external-link"></i>](http://www.modelaircraft.org/)
      - Global drone regulations database  [<i class="fa fa-fw fa-external-link"></i>](https://www.droneregulations.info/)
      - USA aeronautical charts online  [<i class="fa fa-fw fa-external-link"></i>](https://skyvector.com/)
      - USA flight restrictions map [<i class="fa fa-fw fa-external-link"></i>](https://app.airmap.io/)
  - Note any hazards or risks such as power lines, cell towers, etc.
- Cache the basemap for the area in Mission Planner
- Charge laptop batteries, camera batteries, transmitter batteries
- Charge flight batteries
  - **Caution:** inspect batteries for any bulging or damage, and do not use if bulging or damaged
  - **Caution:** never charge batteries unattended!
  - Plug in your battery charger and add the XT-60 (or appropriate connector)
      - Caution: if you attached the battery to the connector first you risk creating sparks when plugging the leads in and damaging your charger
  - Plug the battery's XT-60 and balancer into the charger
  - Select `LiPo` and then `Balance charge` on the charger
  - Press start and then set the amps
      - Charge the battery at a level appropriate (lower amps will be a slower charge but is better for the strength of the final charge and overall battery life)
  - Press `start` again and set the number of cells (a 4S battery is 4 cells)
  - Press and hold the `start` button, and the charger will check the battery
  - Confirm the settings are correct and press `start` again to begin the charge
  - Return batteries to storage level if more than a couple of days without use, check every month or so
- Pack everything for transport to flight location

## Pre-flight checklist

- Pilot safety
  - Remote Pilot in Command (PIC) preparedness
  - Physically and mentally fit, no alcohol in previous 8 hours and BAC <0.04 (12 hours bottle to throttle is a good guideline for pilots of manned aircraft as well as remote pilots flying drones)
  - Good practice to have a visible observer
- Assemble the drone
  - Attach wings, tail, and connect servo wires
  - Multiple rubber bands on wings
  - Attach propeller
      - **Caution:** always remove the propeller during any diagnostics or troubleshooting and never attach propellor unless you are ready to fly
      - Numbers printed on the propeller should face forward
      - Hold motor housing when tightening propeller nut
  - Place battery
  - Check center of gravity
      - Drone should be level or 5 degrees nose down at most (not tail down)
- Visual check
  - No visible damage
  - Check all connections (electronic, control horns, servo linkages, and other physical)
  - Control surfaces neutral
- Turn on GCS, connect the base station telemetry via USB, and open Mission Planner
- Power on transmitter
  - **Caution:** make sure throttle is all the way down
- Plug in battery on drone
  - Make sure drone is flat and level
  - Power on where you want the drone to loiter in RTL mode
  - Pixhawk [Main LED](https://pixhawk.org/users/status_leds) indicator
      - Solid any color: Armed
      - Breathing any color: Standby
      - Amber: Low battery or failsafe (e.g. return to home)
      - Blue: GPS not locked
      - Green: GPS locked
      - Fast Blink & Red: Arming error
      - Blink & Red: Other error
- Connect GCS to drone in Mission Planner
- Accelerometer calibration
- Compass calibration
  - Compass calibration may not be necessary if you have not travelled a great distance from the last flight location where the compass was calibrated (the Earth's magnetic field varies depending on your location relative to the poles)
  - Check declination on GCS display, the red line emerging from the front of the drone icon should match the direction the physical drone is facing
- Check your pitch roll and yaw angle on the GCS HUD and verify that they match the rotation of the drone
- Check camera settings and test trigger camera manually
- Flight mode check
  - **Caution:** check that drone is disarmed!
  - Toggle flight mode switch and confirm on the display in Mission planner that the drone is switching between the desired modes (FBWA ←→ Auto ←→ RTL)
- Arm the drone by pressing and holding the arm button (the light changes to a solid from blinking)
  - **Caution:** ensure drone is in FBWA and the transmitter is on with throttle all the way down!
  - **Caution:** if the drone is in Auto or RTL it will immediately start the propeller!
  - **Caution:** if the transmitter is off, a failsafe will likely switch the drone into RTL mode!
- RC Transmitter control check for elevon planes [or] 4-channel planes
  - Right stick forward: both elevons down [or] elevator down
  - Right stick back: both elevons up [or] elevator up
  - Right stick left: left elevon up, right elevon down [or] left aileron up, right aileron down
  - Right stick right: left elevon down, right elevon up [or] left aileron down, right aileron up
  - Left stick left: nothing [or] rudder left
  - Left stick right: nothing [or] rudder right
  - (**Caution:** with helper holding drone and well clear of propeller) Left stick forward: motor on full
  - Left stick back: motor off
- FBWA response check for elevon planes [or] 4-channel planes
  - Roll drone left: left elevon down, right elevon up [or] left aileron down, right aileron up
  - Roll drone right: left elevon up, right elevon down [or] left aileron up, right aileron down
  - Pitch drone forward (nose down): both elevons up [or] elevator up
  - Pitch drone back (nose up): both elevons down [or] elevator down


## Post Mission

- Power off drone first, then transmitter and GCS
- Check your camera memory card
