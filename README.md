Nocturn Remote Script for Ableton Live
======================================

Introduction
------------

Nocturn RS4L is an unfficial software to control Ableton Live remotely. You have access to mixer,
scene, devices, transport and other parameters from an Novation Nocturn controller.

Developed in 2009 by Guillermo Ruiz Troyano

License
-------

All files of this product are subject to the GNU Public License (GPL). The text of the GPL is
included in the distribution (License.txt).

Installation
------------

You need to configure both Ableton Live and Novation Automap.

### Ableton Live

* Mac OS X:
    * Open Finder and go to your Ableton Live folder, right click (Ctrl+Click) on Live and show
      package contents. In there go to the folder *Contents/App-Resources/MIDI Remote Scripts/* and
      move the folder Nocturn in there.
    * Start Live.
    * Go to Preferences, MIDI/Sync tab and select Nocturn in the dropdown list of available control
      surfaces. Select Automap MIDI port as input and output. Below, enable Remote on both ports.

* Windows:
    * Open Program *Files\Ableton\Live\Resources\MIDI Remote Scripts* and move the folder Nocturn in
      there.
    * Start Live.
    * Go to Preferences, MIDI/Sync tab and select Nocturn in the dropdown list of available control
      surfaces. Select Automap MIDI port as input and output. Below, enable Remote on both ports.

### Novation Automap

* Set the MIDI input and output ports to 'Automap MIDI' in the Automap settings menu.
* Activate MIDI channel 1,2,3,4 from the Automap settings menu.
* Open Mixer.automap from Automap folder. Select Mixer as group on top left of Automap window.
* Open Instr.automap and select Instr. as group.
* Open Fx.automap for Fx group.
* Open User.automap and select the User group.
* Select 'Set As Default Control Map for this Client' in File menu if you want to save each section
  as default client.

Enjoy!


Control specification
---------------------

### Mixer Section

* Page 1:
    * Rotary encoder 1-8: Volumes of tracks
    * Buttons 1-8: Track on
* Page 2:
    * Rotary encoder 1-8: Panning of tracks
    * Buttons 1-8: Track solo
* Page 3:
    * Rotary encoder 1-4: Volumes of return tracks
    * Buttons 1-4: Return track on
    * Rotary encoder 5: Master volume
    * Button 5: Enable arm of tracks or only selection
    * Rotary encoder 6: Master panning
    * Rotary encoder 7: Cue volume
    * Button 6,7: Tempo nudge down and nudge up
    * Rotary encoder 8: Tempo
    * Button 8: Tap tempo

    
### Instrument Section

* Page 1:
    * Rotary encoder 1-8: Parameters of selected device.
    * Buttons 1-8: Track arm and/or selection (see Mixer Section, Page 3, Button 5)
* Page 2:
    * Rotary encoder 1-8: Parameters of selected device.
    * Buttons 1-8: Parameters bank 1-8 of selected device (max. 64 parameters)


### Fx Section

* Page 1:
    * Rotary encoder 1-8: Send A of tracks
    * Button 1-8: Tracks bank 1-8, 9-16, 17-24, 25-32, 33-40, 41-48, 49-56, 57-64
* Page 2:
    * Rotary encoder 1-8: Send B of tracks
    * Button 1-8: Tracks bank 1-8, 9-16, 17-24, 25-32, 33-40, 41-48, 49-56, 57-64
* Page 3:
    * Rotary encoder 1-8: Send C of tracks
    * Button 1-8: Tracks bank 1-8, 9-16, 17-24, 25-32, 33-40, 41-48, 49-56, 57-64
* Page 4:
    * Rotary encoder 1-8: Send D of tracks
    * Button 1-8: Tracks bank 1-8, 9-16, 17-24, 25-32, 33-40, 41-48, 49-56, 57-64


### User Section

* Page 1:
    * Button 1: Metronome on/off
    * Button 2: Play
    * Button 3: Stop
    * Button 4: Record
    * Button 5: Overwrite on/off
    * Button 6: Punch in
    * Button 7: Loop enabled
    * Button 8: Punch out
    * Rotary encoder 1: Select a scene in session view
    * Rotary encoder 2: Select a track
    * Rotary encoder 3: Change the global quantization
    * Rotary encoder 4: Move the global position
    * Rotary encoder 5: Move the playing position of selected clip
    * Rotary encoder 6: Move the loop start of selected clip or arrangement (if the master section
                        is selected)
    * Rotary encoder 7: Move the loop length of selected clip or arrangement (if the master section
                        is selected)
    * Rotary encoder 8: Change the coarse pitch of an audio clip. Transpose selected notes or all
                        notes of a MIDI clip.
* Page 2:
    * Button 1-8: Playing status of clip slot of selected scene of each track
        * Off: The clip is stopped
        * On: The clip is playing
        * Blinking: The clip is triggered
        * Rotary encoder 1-8: See page 1
* Page 3:
    * Button 1-8: Show if each track is playing a clip
        * Off: Track don't play any clip. Pressing the button trigger the clip of selected scene.
        * On: Track play a clip. Pressing the button stop this clip.
        * Blinking: A clip slot is triggered.
    * Rotary encoders: See Page 1

Revisions
---------

2009-12-16:
Bug fixed on parameter bank select with 3rd party plugins

2009-10-18:
* Transport controls added.
* Now all or selected notes of a MIDI clip can be transposed.
* Loop control improvement and bug fixed.
* Free buttons of User section (last page) now stop all clips.

2009-09-01:
Bug fixed when a device has less of 8 parameters.
