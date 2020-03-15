# Troopduino-Code
Code for Troopduino Voice Changer and Effects Board

This project uses an Arduino nano to create clicks and static when talking.  
Features:
<ul>
  <li>Voice changer
  <ul>
  <li>Bandpass Filter</li>
  <li>Bitcrusher</li>
  <li>Reverb</li>
</ul>
  </li>
  <li>PTT (Push to Talk) Mode</li>
  <li>Voice Activation Mode</li>
  <li>Sound Effects</li>
  <li>Looping Background Effects</li>
</ul>

https://github.com/BipeFlyer/Troopduino

### Button Functionality

- Button 1
  - Long Press
    - Normal Mode: PTT
    - Config Mode: Cycle to next configuration
  - Single Click
    - Normal Mode: Play "move along" sound effect
    - Config Mode: Increment current configuration value
  - Double Click
    - Normal Mode: Toggle PTT/voice activation mode
- Button 2
  - Long Press: Enter/exit config mode
  - Single Click
    - Normal Mode: Play "ask ID" sound effect
    - Config Mode: Decrement current configuration value
- Button 3
  - Long Press: Enter Chatter Mode
  - Single Click
    - Normal Mode: Play "scream" sound effect
- Button 4
  - Single Click
    - Normal Mode: Play "scream" sound effect    
