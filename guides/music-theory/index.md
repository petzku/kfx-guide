# KFX in terms of music theory

One of the important core concepts for making your KFX look visually pleasing and match the feel of the music is understanding what the sound is actually _doing_. If this sounds obvious to you, great. If not, don't worry, I'll try to explain both what I mean by this, as well as how to actually apply this understanding to your styling.

## Envelopes

When talking about sound or music, "envelope" usually describes how a given sound behaves over time. Different instruments can produce very differently-shaped sounds:

- A piano key or a guitar string produces a near-instant sound when played, that slowly decays over time as long as the note is held, and mutes as soon as the key is released or the string muted
- A bowed string instrument like a violin takes a longer time to produce the peak volume when the string is bowed, and only remains that way as long as the player bows the string, but the sound still decays somewhat slowly afterwards
- Some percussion instruments, primarily drums, produce a sound immediately when struck, but cannot be held, and thus decay to nothing very quickly too. Some drums, such as snare drums, decay somewhat slower than others, but the sound still cannot really be _held_, as you might on a piano.
<!-- TODO: add more examples here? -->

Here, we'll mostly be focusing on the first kind of sounds, though the ideas are transferrable to other kinds of envelopes, too. This kind of envelope is usually thought of as an idealized "ADSR" model, standing for "Attack, Decay, Sustain, Release". The diagram below demonstrates what each of these mean:

![Diagram of the idealized ADSR envelope](https://upload.wikimedia.org/wikipedia/commons/thumb/e/ea/ADSR_parameter.svg/800px-ADSR_parameter.svg.png)
*Diagram of an idealized ADSR envelope. © Abdull / Wikimedia Commons / CC-BY-SA-3.0*

The durations of these all can vary, but typically Attack is much shorter than the others. Decay can start immediately after Attack is over (i.e. the sound has reached its peak), but the sound can also be Sustained at or near the peak (such as with the violin), before Release, where the amplitude drops back down to zero. Typically, Release is slightly longer than Attack.
