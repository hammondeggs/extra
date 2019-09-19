# extra
Add extra paraphonic voices to your minilgoue xd synthesizer!

# As always, especially with the KORG user oscillators, these are to be used at your own risk!


### A quick word...
I've been having a ton of fun creating these plugins, and it's thirsty work. If you like stuff like this and my other work, by all means feel free to contribute whatever you can to the fund to help fund the beer supply!

This can be done here :  [Donate!](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=MSTCVLXMG7Z5J&source=url)


### installation

Ensure you have the KORG minilogue/prologue sound librarian installed. Now, before you do anything else, **perform a full and complete backup of your synthesizer and save this to disk before continuing**. See the sound librarian manual for instructions on how to do this if required.

Next, select the USER OSCILLATORS tab on the librarian, and drag and drop the requisite file to an available slot in the librarian :
 - for Minilogue xd users, please use extra.mnlgxdunit

#Note there is no prologue support at this time - prologue can already have at least 8 voices - this is primarily intended for minilogue users!#

You should now see Extra V1.00-1 listed in your user oscillators. Press "Send All" under USER OSC / FX to send all of your user oscillator / effects to your synthesizer

*please note if you do not do this correctly you may run the risk of losing data. As always, backup, backup, backup!*


### usage

Extra, doesn't "really" give you extra voices on your synthesizer. But it can sound like it! It does this, by having 2 or 3 "voices" for each user oscillator, that cycle through as new notes are played. Due to the way voices are assigned though, you can only ever sustain up to 4 of these, if you have sustain enabled. In addition, as the user oscillators were never intended for this, you will likely run into some un-intended artifacts, some of which though can be purposed into features. Typically, for an initial set up, it's reccomended you start with the filter wide open, and the AMP eg set to 0 attack 0 decay, full sustain and full release. We will use the envelopes on the user oscillator, which can be adjusted as such:

- Shape : Adjust the 'decay' time
- Shift-Shape : Adjust the 'attack' time

One particular caveat to note however, is that currently user oscillators stop executing once it's 'voice' has closed it's AMP eg. So, if your oscillator was in the middle of it's own EG phase, it will pause, and resume once that voice's analog AMP eg has retriggered. This also will apply to filter EG, but you can use this to an effect much like on a traditional paraphonic synthesizer.

### edit menu

#### Waveform
- 1 : Single saw. Support for up to 12 notes simultaneously
- 2 : Double saw. Support for up to 8 notes simultaneously, with a detunable second saw waveform
- 3 : Pulse / PWM. Also support for up to 8 notes simultaneously, with pulse width and PWM

#### Detune
Applies to waveform type 2 only. Detunes the second sawtooth waveform up to +1 octave

#### PW 
Applies to waveform type 3 only. Sets the initial / fixed pulse width

#### PWM Rate
Sets the PWM LFO oscillator rate.

#### PWM Amount
Sets the amount to modulate the pulse width by. A value of '1' is 'no pwm'.


#### Sustain
- 1 : No sustain. Notes will attack up to full and then switch to decay
- 2 : Sustain. Notes, that can sustain, will attack up to full and hold the note, decaying when the note is released - or when the note is re-assigned via the synthesizers default voice assignment.


#### Other caveats

Oscillator pitch is 'latched' on note on. So if you move the pitch bender before playing a note, it will latch that note value. This also means that the pitch LFO will not work as well. These are due to the user oscillator playing and tracking 2 or 3 notes at the same time.

Also, as this crams 2 or 3 'voices' into a single user oscillator, there is *much* less CPU time vs a single oscillator, thus the anti-aliasing isn't as great as it can be with a single proper digital 'oscillator'.


It isn't perfect, but it's something different to try with your synthesizer!




#
*All product names, trademarks and registered trademarks are property of their respective owners.*






