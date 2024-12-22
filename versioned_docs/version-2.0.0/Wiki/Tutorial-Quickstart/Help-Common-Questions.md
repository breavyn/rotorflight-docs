---
sidebar_position: 30
---

# Help - Frequent questions?

A list of common config issues and the solutions?

## Motor won't start
1. Is ARM mode configured? 
    * Please check your Arm Mode has been enabled. See details in the [Modes](../Tutorial-Setup/Modes#arm) 
    * Note!! Arm and Throttle hold need to be on different switches. The FC must see minimum throttle before Arm is enabled; therefore, if Arm activates at the same time as throttle hold is removed, it will fail the minimum check. 
    * Check status page for Arming disables  
3. Using a Governor?  
    * Does the Motor spool in Governor 'passthrough'. If not this could indicate a pin or timer allocation issue. Also please check your Receiver is connected and has the correct channel order.  
    * Does the Motor spool in Governor 'Mode 1'. Please confirm you have either Frequency input or Bi-directional Dshot enabled and functioning. Using the Motor override run the motor at minimum speed and confirm there an RPM signal present  
    * Governor mode 'Mode 2'. If the motor is able to spool in the other modes but not Mode 2 it means the Battery Voltage is not available. Please update this in the Power tab. 


## Servo don't respond
1. Are servos visible in the servo Tab? 
    * Review the [remapping](../Tutorial-Setup/Remapping.md) and add servos

2. From the servo override does the servo move?
    * Confirm connection of the servos
    * Confirm servos are powered
    * Check all servos.

3. Servo moves in override but not 
    * Confirm miser has been chosen from the [Mixer](../Tutorial-Setup/Mixer.md) tab.