# grainfields (Max for Live edition)
#### 8 voice granular synthesizer for monome 128 grids

grainfields turns your 128 grid into a granular synthesizer with 8 voices - each with up to 10 constant streaming grains. Modulate grain parameters (pitch, duration, loop rate, position etc.) of each voice to create a large variety of interesting timbres and textures. Record and loop pattern gestures to create rythmic and melodic sequences.

#### Getting started

Before launching the grainfields Max for Live device make sure that your grid is connected. 

1st step in Ableton is to drop 'grainfields_master.amxd' on an empty track. This device establishes the osc connection with monome (and Lemur on iPad). Show/hide osc settings with the toggle at the bottom of the device. Your monome should auto-detect.

![alt tag](https://raw.githubusercontent.com/kasperskov/monome_grainfields_m4l-v1.0/master/grainfields_master.png)

2nd step is to drop 'voice_1.amxd', 'voice_2.amxd', 'voice_3.amxd' (...and so on) on separate audio tracks (as suggested below). When a new voice m4l device is loaded on an audio track in Ableton, the device will automatically activate the corresponding lights on your monome grid. If you only need e.g. 3 voices then load 'voice_1', 'voice_2', and 'voice_3'. You don't need to load all voices.

![alt tag](https://raw.githubusercontent.com/kasperskov/monome_grainfields_m4l-v1.0/master/overview.png)

#### 8 rows / up to 8 voices

Every row represents a voice, and each voice contains a buffer with up to 10 individual grains. To change buffer content simply drag and drop an audio file into the waveform display of a voice.

#### Grid controls

- Each voice is activated by pressing the far left toggle on the grid.
- The pattern recorder is activated when pressing the second toggle from the left.
- Step 3-15 on each row control the playback position of the buffer audio content.
- The far right toggle records an input into the buffer of the selected voice (change input source in the 'audio & osc setup' menu in the app).

#### Grain parameters

Control the grain density, base pitch and deviation, duration, loop rate, amplitude, envelope slope, and stereo spread of each voice. Additional parameters include:

- 'speed' - sets the speed of moving between grain positions in miliseconds.
- 'fade' - sets the fade in / out time when activating / deactivating a voice.
- 'rec length' - sets the length of recording into the buffer.

#### Global transport & pattern recorder

Start / stop transport by pressing the space bar. The transport needs to be activated in order to record pattern gestures.

Set the desired length of the pattern loop in bars (default=2).

#### Recording into buffer

When recording an input source into a buffer the buffer will autosave the recording into the project folder (located inside the "media" folder).

#### Master presets

Saving a preset (shift>click on a slot) will store all current parameter settings in each voice as well as the file path of buffer contents.

#### Lemur interface 

Control individual voices directly in Ableton or via the included Lemur interface (requires Lemur on iPad).

Install the interface on iPad ('monome_grainfields.jzml' located in the project folder) and make sure to provide the correct port and host settings for incoming and outgoing OSC.

Max for Live devices created by Kasper Fangel Skov 2016
