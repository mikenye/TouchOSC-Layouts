# Edward Foleyart Instrument

[Edward Foleyart Instrument](https://tovusound.com/shop/edward-foley-artist-instrument/) "brings real recorded and natural randomized Foley Artist footsteps to every audio production studio: offers high end quality and parameters to adjust distance and environment based on Native Instruments Kontakt engine."

Also works perfectly with the [Real Outdoor Footsteps](https://tovusound.com/shop/real-outdoor-footsteps-efi/) expansion.

This layout allows you to:
* Play footsteps
* Control volume, pitch, mic selector, shoe type and surface type (requires learning MIDI CC Automation in Kontakt)

In order to use this layout, you will need the following:
* TouchOSC installed on your phone/tablet
* TouchOSC Editor installed on your Mac/PC
* TouchOSC Bridge installed on your Mac/PC
* Network connectivity between your phone/tablet and your Mac/PC
* Optionally, a DAW



## The Layout
This basic layout features two types of controls.
* Play footsteps - this works "out of the box"
* Control volume, pitch, shoe type and surface type - this requires learning MIDI CC Automation in Kontakt, but don't be put off as this is really easy. I'll explain how lower down.

<img src="https://github.com/mikenye/TouchOSC-Layouts/raw/master/Edward%20Foleyart%20Instrument/img/Layout.png" alt="Edward Foley Art (iPhone) Layout Image" width=444px>



## Getting started
1. Install TouchOSC on your phone/tablet
1. Install TouchOSC Editor on your Mac/PC
1. Install TouchOSC Bridge on your Mac/PC
1. Make sure your phone/tablet and your Mac/PC are on the same network


### Install the Layout
1. Launch TouchOSC Editor
1. Download and Open "Edward Foleyart Instrument (iPhone).touchosc" in TouchOSC Editor
1. Press the "Sync" button in TouchOSC Editor
1. On your phone/tablet, launch TouchOSC and navigate to Layout > Add, select your Mac/PC from the list in TouchOSC. The layout should be downloaded and appear in your list of layouts


### Playing Edward Foleyart Instrument "live"
1. Launch TouchOSC Bridge on your Mac/PC
1. Launch TouchOSC on your phone/tablet
    1. Under Connections > TouchOSC Bridge, under "Found Hosts" select your PC/Mac. It will connect and you'll be taken back to the main menu
    1. Under Layout, choose the Edward Foleyart Instrument layout
    1. Press "Done" (top right), and you'll be taken to the Edward layout.
1. Launch Kontakt and load the Edward Foleyart Instrument or the Edward Real Outdoor Footsteps instrument and customise as desired.
1. In Kontakt preferences, go to MIDI > Inputs. TouchOSC Bridge should show up as one of the input devices. Change its status from "Off" to "Port A" and press "Close"
1. On your phone/tablet, press the "SLOW", "WALK", "FAST", "CREEP", "STOP", "SCUFF", "SPIN", "SET" and "LAND" buttons to play samples.


### Recording Edward Foleyart Instrument in Reaper DAW
1. Launch TouchOSC Bridge on your Mac/PC
1. Launch TouchOSC on your phone/tablet
    1. Under Connections > TouchOSC Bridge, under "Found Hosts" select your PC/Mac. It will connect and you'll be taken back to the main menu
    1. Under Layout, choose the Edward Foleyart Instrument layout
    1. Press "Done" (top right), and you'll be taken to the Edward Foleyart Instrument layout.
1. Launch Reaper.
    1. In Reaper's preferences, under Audio > MIDI Devices, double-click "TouchOSC Bridge" and make sure "Enable input from this device" and "Enable input for control messages" are both ticked.
    1. Create a new track.
    1. Bring up the track FX window
     1. Add Kontakt AU/VST
      1. In the Kontakt AU/VST, load the Edward Foleyart Instrument or the Edward Real Outdoor Footsteps instrument and choose a preset and customise as desired
      1. Close the FX window
    1. In the track's recording input, select "Input: MIDI" > "TouchOSC Bridge" > "All Channels"
    1. Change the track's "Record Monitoring" to "ON" (by clicking the little speaker button)
    1. Arm the track for recording
1. You should now be able to play Edward by pressing the "SLOW", "WALK", "FAST", "CREEP", "STOP", "SCUFF", "SPIN", "SET" and "LAND" buttons to play samples.
1. To record a MIDI item to control Edward:
    1. Press "Record" on the transport
    1. Press the the "SLOW", "WALK", "FAST", "CREEP", "STOP", "SCUFF", "SPIN", "SET" and "LAND" buttons to play samples. You should see your MIDI data being recorded.
    1. Press "Stop" on the transport (press "Save All" if prompted), rewind and hit "Play". You should hear back your recorded foley.

### Learning MIDI CC Automation for Volume, Pitch, Mic Selector, Shoe Type, Surface Type (Optional)

In order to control volume, pitch, mic selector, shoe selector and surface selector, you need to learn MIDI automation for these items. You can do this by performing the following:

* For Volume: In Kontakt (plugin or standalone application), in the Edward instrument, right-click the volume knob and choose "Learn MIDI CC# Automation". In TouchOSC, move the volume fader. You should then see volume in Edward increase/decrease as you move the fader in TouchOSC.

* For Pitch: In Kontakt (plugin or standalone application), in the Edward instrument, right-click the pitch knob and choose "Learn MIDI CC# Automation". In TouchOSC, move the volume fader. You should then see pitch in Edward increase/decrease as you move the fader in TouchOSC.

* For Mic Selector: In Kontakt (plugin or standalone application), in the Edward instrument, right-click the Mic Selector fader and choose "Learn MIDI CC# Automation". In TouchOSC, move the Mic Selector fader. You should then see the fader in Edward increase/decrease as you move the fader in TouchOSC.

* For Shoe Selector: 
    * In Kontakt (plugin or standalone application), in the Edward instrument, right-click the left arrow (<) next to the shoe type, and choose "Learn MIDI CC# Automation". In TouchOSC, press the left arrow next to "shoe type".
    * In Kontakt (plugin or standalone application), in the Edward instrument, right-click the right arrow (>) next to the shoe type, and choose "Learn MIDI CC# Automation". In TouchOSC, press the right arrow next to "shoe type".
    * You should then see the shoe type in Edward change as you press the shoe type buttons in TouchOSC.

* For Surface Selector: 
    * In Kontakt (plugin or standalone application), in the Edward instrument, right-click the left arrow (<) next to the surface type, and choose "Learn MIDI CC# Automation". In TouchOSC, press the left arrow next to "surface type".
    * In Kontakt (plugin or standalone application), in the Edward instrument, right-click the left arrow (>) next to the surface type, and choose "Learn MIDI CC# Automation". In TouchOSC, press the right arrow next to "surface type".
    * You should then see the surface type in Edward change as you press the shoe type buttons in TouchOSC.

* If you screw up, just right click the control in Kontakt that isn't working properly, and choose "Remove MIDI Automation", then try again.

* You'll need to set this up before the Volume, Pitch, Mic Selector, Shoe Type and Surface Type controls work in the TouchOSC layout. Otherwise they'll just do nothing.

