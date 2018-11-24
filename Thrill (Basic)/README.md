# Basic TouchOSC Layout for Thrill

[Thrill](http://www.galaxy-instruments.com/thrill.html) is an amazing "performance instrument for playing spine-chilling atmospheres, clusters, and hybrid textures" by [Native Instruments](https://www.native-instruments.com/en/products/komplete/cinematic/thrill/) / [Galaxy Instruments](http://www.galaxy-instruments.com/thrill.html). It is a Kontakt instrument that works with the free Kontakt player.

This basic [TouchOSC](https://hexler.net/software/touchosc) layout allows you to:
* Perform real-time control of Thrill's XY pad
* Perform simple note-on/note-off
* Play Thrill's "live" (useful for stage performances)

In order to use this layout, you will need the following:
* TouchOSC installed on your phone/tablet
* TouchOSC Editor installed on your Mac/PC
* TouchOSC Bridge installed on your Mac/PC
* Network connectivity between your phone/tablet and your Mac/PC
* Optionally, a DAW



## The Layout
This basic layout features two controls.
* An XY Pad labelled "Thrill X/Y Control"
* A button labelled "Hold to THRILL!"

The idea is that you set Thrill up in the way you want, select your preset, modify as required, then use the TouchOSC layout to "play" Thrill, either live or while recording MIDI input with your DAW.



## Getting started
1. Install TouchOSC on your phone/tablet
1. Install TouchOSC Editor on your Mac/PC
1. Install TouchOSC Bridge on your Mac/PC
1. Make sure your phone/tablet and your Mac/PC are on the same network


### Install the Layout
1. Launch TouchOSC Editor
1. Download and Open "Thrill XY Basic (iPhone).touchosc" in TouchOSC Editor
1. Press the "Sync" button in TouchOSC Editor
1. On your phone/tablet, launch TouchOSC and navigate to Layout > Add, select your Mac/PC from the list in TouchOSC. The layout should be downloaded and appear in your list of layouts


### Playing Thrill "live"
1. Launch TouchOSC Bridge on your Mac/PC
1. Launch TouchOSC on your phone/tablet
  1. Under Connections > TouchOSC Bridge, under "Found Hosts" select your PC/Mac. It will connect and you'll be taken back to the main menu
  1. Under Layout, choose the Thrill XY Basic layout
  1. Press "Done" (top right), and you'll be taken to the Thrill layout.
1. Launch Kontakt and load the Thrill instrument and choose a preset and customise as desired.
1. In Kontakt preferences, go to MIDI > Inputs. TouchOSC Bridge should show up as one of the input devices. Change its status from "Off" to "Port A" and press "Close"
1. On your phone/tablet, press the "Hold to THRILL!" button and move your finger around the XY pad. It should control Thrill.


### Recording Thrill in Reaper DAW
1. Launch TouchOSC Bridge on your Mac/PC
1. Launch TouchOSC on your phone/tablet
  1. Under Connections > TouchOSC Bridge, under "Found Hosts" select your PC/Mac. It will connect and you'll be taken back to the main menu
  1. Under Layout, choose the Thrill XY Basic layout
  1. Press "Done" (top right), and you'll be taken to the Thrill layout.
1. Launch Reaper.
  1. In Reaper's preferences, under Audio > MIDI Devices, double-click "TouchOSC Bridge" and make sure "Enable input from this device" and "Enable input for control messages" are both ticked.
  1. Create a new track.
  1. Bring up the track FX window
    1. Add Kontakt AU/VST
    1. In the Kontakt AU/VST, load the Thrill instrument and choose a preset and customise as desired
    1. Close the FX window
  1. In the track's recording input, select "Input: MIDI" > "TouchOSC Bridge" > "All Channels"
  1. Change the track's "Record Monitoring" to "ON" (by clicking the little speaker button)
  1. Arm the track for recording
1. You should now be able to play Thrill by pressing the "Hold to THRILL!" button on your phone/tablet and moving your finger around the XY pad
1. To record a MIDI item to control Thrill:
  1. Press "Record" on the transport
  1. Before pressing the "Hold to THRILL!" button, move the XY pad to the desired starting position. We need to do this so Thrill receives the MIDI control messages and sets its XY pad to the desired position before playing audio. This prevents Thrill starting at an undesired volume/intensity.
  1. Press the "Hold to THRILL!" button and move the XY pad around. You should see your MIDI data being recorded.
  1. Press "Stop" on the transport (press "Save All" if prompted), rewind and hit "Play". You should hear back your recorded Thrill.
