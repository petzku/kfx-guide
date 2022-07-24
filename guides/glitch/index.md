# Glitch effects

The other day, I came across someone asking for suggestions to reflect "glitched" audio in their subs. Now, while I don't advocate for doing this universally, it can work really well when done right. Unfortunately, as for many things, there's a million more ways to do it wrong than to do it right, and "right" can mean different things for different people.

One important thing to keep in mind when designing the "glitch" effects is to limit their impact to the viewer. You typically want the viewer to still be able to read your line, after all. The most obvious options are to only affect a small part of the line at a time (like [Corruption](#corruption)), or only show up briefly (like [CRT distortion](#crt-distortion)).

So, assume we know we want to be doing this. Let's look at some of our options.

## Different types of "glitching"

### Scramble

The first effect I made in this vein wasn't even with templates. It uses the Unscramble mode of [Typewriter][typewriter], though the effect from that script can't really be applied to dialogue. See [Asakura's Tensura](asakura-tensura-unscramble.webm) (note: the sign, not dialogue) for a sample of the script in action.

This is probably best saved for pre/postline effects, since it has the potential to be quite disorienting, but a temporally-limited one could work well. The main issue is with the entire structure of the line (potentially) changing as actual text content is changed.

### CRT distortion

This is probably the first actual *dialogue* effect I made. The specific one is synchronized to static sounds in the audio.

This is essentially a vertical clip-based gradient, with each stripe getting a random horizontal position and `\fax` every frame. In fact, the `\fax` is apparent e.g. in how the `f` behaves below.

![Dialogue text periodically shuffles sideways in strips, akin to a CRT display](kaleido-hf3-crt.gif)

### Corruption

I can't really take credit for this; I was largely inspired by Zahuczhy's KFX on the Lycoris Recoil opening. My version here is a fairly stripped version of what the full effect is in that release, but it serves to demonstrate the idea.

Nevertheless, the concept is simple: discolor and dislocate a small part of the line very briefly. Repeat a bunch over the line's duration and length.

![Lorem ipsum, with randomly-appearing fragments of the same text in various colors, slightly offset from the original text](corruption.gif)

[typewriter]: https://github.com/petzku/Aegisub-Scripts#typewriter

## Actually making these

TODO
