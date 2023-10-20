---
Class: Script
Type: Long Form
Pinned: true
Status: Draft
Topic:
  - "[[Music Production]]"
Created: Saturday, August 26th 2023, 3:30:01 pm
Modified: Thursday, October 5th 2023, 2:40:36 pm
---

# Notes

## Premise

## Title Ideas

- Ableton Veteran Tries Bitwig Studio 5 for the First Time

## Main Points

# Intro

*Intro bumper goes here…*

# Why I’m Trying Bitwig

Why am I trying Bitwig? Well, aside from the fact that Bitwig recently dropped version five, I’ve been feeling pretty limited by Ableton’s native modulation capabilities.

For me, this translates directly to a lack of quality of life features when it comes to creating custom macros and tools that help speed up my workflow. Let me explain.

# Gripes With Ableton

## VCA Tracks

One of my biggest gripes with Ableton is the lack of VCA tracks or any native hackarounds to get past Ableton’s limitations without resorting to learning MAX4LIVE or downloading someone else’s MAX device that may not do exactly what you want, break down the line, contain bugs, misbehave, or simply look like dogshit.

*Let’s be real, we’re music producers here, most of us probably aren’t UI designers.*

## Myriad of Modulators

Bitwig allows for any single modulator to control any parameter anywhere in your project. This means I can make a pseudo-VCA using a single modulator, and I can put it wherever it’s most convenient for me.

Bitwig’s group header views mean I can make these pseudo-VCA mappings on my *master channel’s macro section* and then *view them from any channel* to quickly add mappings.

# A Rant About MAX4LIVE

## Max 4 Live Feels *Wrong*

I’m well aware that MAX4LIVE opens up an entire world of possibility in Ableton, but to me using other people’s MAX devices always felt like playing a game like Minecraft or Skyrim with way too many different mods installed.

Each mod having potentially very different design philosophies makes for a “hacked together” sort of feeling that I just can’t get over, and results in a fragmented user experience.

Don’t get me wrong, I’ve used some FANTASTIC MAX devices, and there are some INSANE creators who I have massive respect for, but nevertheless… this fact bothers me.

## Woes Of Unmaintained Devices

Additionally, MAX devices are often left unmaintained by their creators, leading to forks of devices and deprecated pages on the MAX4LIVE website.

Opening old projects containing these devices can easily break parts of projects, or entire projects depending on how often you used that device and how important it is.

If you’ve done, say, a hundred projects in Ableton, I can almost GUARANTEE you’ve experienced this tragedy at LEAST once before. Good luck opening someone’s MAX patch and having a SINGLE clue how to fix it.

I’ve also had an instance in the past where a fresh install of Ableton *somehow* did not package the latest version of MAX4LIVE with it, which I was unaware of for *months*, leading me to abandon using MAX devices altogether due to absolutely none of them functioning as expected.

## MAX4LIVE Is an IDE

Lastly, MAX4LIVE feels like an IDE, which is short for iterative development environment. This is what programmers use to write and test code. MAX4LIVE is essentially this, another program used to create devices for Ableton.

I don’t know about you, but I don’t really want to have to be in a separate development environment when I’m making music. Sure, I love to get into the technical details and math of advanced sound design and use my analysis tools to build ridiculous sounds, but the interface and user experience *should only exist to make that process feel like second nature.*

# Scopes of Control

## Hierarchy is Important

I’m going to talk about a concept I’ve been calling “scopes of control.” This is essentially the idea of creating a hierarchy of universally useful, or even specialty macros at specific track groupings in your project.

Every grouping is a “scope” which affects tracks contained within it and is similarly affected by scopes it’s inside of. This concept of “scopes” is also taken from programming and is basically just another way of representing a Russian nesting doll sort of structure, except that in this case every doll can contain as many smaller sized dolls as your CPU is capable of handling before it inevitably catches fire.

This concept is essentially what a track bus is at all. The bus represents a high-level scope, where the bus volume fader affects the volume of all of the low-level tracks inside of it. Now, this is probably an overly complicated way of saying something that probably may feel like common sense to you, *but bear with me here.*

## Reusability is King

*The goal is to create re-usable macros* that leverage scope-level parameters in your DAW to accomplish multiple things at once, resulting in a faster and more streamlined workflow, more consistent results across projects, and re-usable tools that will contribute to your overall style.

*The goal of creating macros in general is to combine and streamline contexts of information across multiple scopes.* When I say context, I literally mean the ability to compare one thing to another and gather actionable information that contributes to you finishing your song. I often refer to how “useful” or not a context of information is.

The intention is to set yourself up with as much “useful” contextual information as possible in a project with the least effort. However, gathering context requires knowing what to look for, which requires intention.

Most situations in writing or mixing a song are going to require becoming familiar with *many different kinds of contextual awareness* to be able to “tap in” to your flow state and have an efficient producing session.

# Resolution Limits Context

## This May Be Tough to Hear

*This is going to get a bit complicated, but I promise it’ll be worth it.*

There’s two “devices” at play in every good song, those being contrast and change over time. If no processing whatsoever is used on an audio source, both of these are simply functions of the audio source’s dynamic range.

## The MIDI Codec

*The MIDI codec limits the resolution of controls,* or the number of increments, to to a limited range of 128 values *(0-127).* MIDI has *discrete, linearly spaced increments* where every increment is a single integer. This range of allowed values can not and will not change until MIDI 2.0 is released. It’ll always be 128.

Because of this, it’s easy to measure, compare, and create different MIDI macros at any scope level. Every increment is the same, making MIDI inherently linear. Any automation curve you make for that macro will multiply linearly as well and therefore when the macro changes over time, the resulting effect is as linear or non-linear as you make the automation curve.

Due to this flexibility, macro mappings can be controlled from any scope level by simply adding another macro mapping where you want it, and the result is the same. It will always provide 100% useful context as to what every increment in the range of the macro will do.

For example, say we have a MIDI macro and we mapped it across the entire range of the frequency cutoff knob on a filter. Fully closed to fully open. Simple, right? If at any point in time we go back to that macro, *we can simply look at the macro and its relationship to the frequency cutoff knob is self evident* *without any other information needed for context.*

We know MIDI values start at 0, we know they end at 127, and we know all of the numbers in between. We also know that the audible frequency range is 20 Hz to 20 kHz, so let’s say that’s the range of our frequency knob. By knowing that both the macro and the cutoff knob’s control ranges start and end at tangible, fixed values, we can reasonably determine what will happen at any value between the start and the end of the macro.

*With MIDI values, the system for us to gather context* is the fact there are 128 pieces of easily understandable pieces information encoded into it which we can change over time to *compare and contrast the differences or similarities assigned to each value.* The needed context is contained within the MIDI macro, *only because it’s a data set* and *not a single piece of data*. Remember, context is only gained through comparing multiple pieces of data.

## Dealing With Audio

Audio always needs the context of another audio source to be evaluated for the information we want out of it, which in this case is how its track-level dynamics will affect the master-level dynamics. *The resolution of acceptable dynamic range is from -inf dB to 0dB at unity,* where unity represents the current output volume of whatever device you’re listening on, however loud that may be. Volume has continuous, non-linearly spaced increments, where each increment has more or less perceived value depending on how far up or down the audible decibel range that increment sits. Because of this, dynamics plugins *cannot necessarily be replicated or cloned* to any scope and be expected to have the same perceived volume change at that scope. What this means is that any useful context we think we’ve gathered about how much a given setting on a dynamics plugin will affect the perceived loudness of a sound in the context of the mix is only really useful for the particular scope we’re listening to.

Context is implicit when it comes to changing MIDI values, and as a result, using MIDI is more or less intuitive to everyone despite my attempts to make why we understand it so easily all technical and complicated. Conversely, we all know it’s hard to compare volume remotely objectively when decibels basically aren’t a self-consistent increment, right? So how can we gather useful context that’s self-consistent enough to allow us to make gain changes that affect the perceived loudness of tracks similarly across all scopes in the project?

# Creating a System for Gathering Context

## Context v. Volume

With volume, gathering context in a systematic way is harder to understand due to dynamic range being a non-linear data set, and every audio source having a unique dynamics. So how can we bring our ability to compare dynamic range and perceived loudness into a more objective and coherent realm? Let’s try something. Instead of representing the resolution of either MIDI or volume by counting increments, let’s disregard that and say for now that the range of -inf dB to 0db can be represented as a generic 0-100% value in the case of volume, and similarly 0 - 127 can be represented as a generic 0-100% value in the case of MIDI. Both MIDI and volume now scale nicely to the same easy to understand range of values, right?

## Context v. MIDI

While we *can* convert both MIDI and volume to a percentage format to make it easier to compare their resolution in some ways, it doesn’t change the fact that MIDI values have clearly defined constraints by nature of having two integers as start and end points, while dynamic range doesn’t have constraints. Well, this only half true, it does have constraints, but they’re as hidden as they are obvious. We know that the start point of volume is no volume at all, nothing, -inf dB. Negative infinity as a mathematical value is impossible to translate into actionable information or gain much useful context from, other than knowing that no sound is playing. But what about the end point? That’s 0 dB. Unity, the clip threshold. While we can constrain MIDI within two concrete, tangible points, with volume there is only one, and that’s unity. A fixed threshold you don’t want to cross. Then we have the threshold of audible sounds, which is somewhere around -70dB in Ableton, after which it simply turns the sound off altogether. So what does this mean for our scopes of control?

## Unity Saves Us All

*Unity is the only reliable, fixed endpoint we can gain 100% useful context from* in terms of dynamic range and perceived loudness. As we move towards -inf dB we lose useful context exponentially until the sound disappears altogether, where the available useful context then instantly becomes 100% again, only because we know there is silence. Now that we know we can use unity to forever provide a much needed constraint, it will allow us to avoid guessing how to gain stage across scope levels to achieve the dynamic range and perceived loudness we want. There is a single, fixed piece of data you can reference to mix every single track and bus in your project against. Again, that may seem like a complicated way of saying something that seems obvious, but this is where a LOT of people miss what this implies.

## Climbing to New Heights

So now we know we WANT to use 0db as a fixed endpoint because constraints provide better context. *To do this, we have to limit or clip every track and bus right up to the unity threshold such that the peak is always at unity when the track fader is set to unity, and only then mix the track into context*. This way we know our audio always peaks exactly at where the track fader is set and we instantly remove the struggle of gathering context concerning dynamic range across scopes and scope levels. This is quite literally the only way to ensure you can reference and gather reproducible context about how “perceptually loud” your numeric gain changes will be up, down, and across scopes. It’s relatively impossible to gain context on how multiple things interface with each other if none of those things share a common rule. This applies to basically every form of analytics in existence.

## New Scene #review

*Stop allowing your audio to float around your dynamic range without any constraints, and as a result without any coherent context. It only compounds mixing issues as you move up the scope hierarchy towards your master track. If you don’t push your tracks to unity and leave them floating without constraint, you’ll find that the correlation between perceived loudness and decibel values become increasingly meaningless the further you move to higher scopes.*

For example, you chose not to have volume limitations at the track level. That means that at the bus level, your input gain also has no fixed limitation. Even if you do put a limiter right at the start, unpredictable peaks will push your plugin chain harder than you intended. So to stop that, you decide to turn down the tracks inside the bus. The bus is still set to the same volume as it was, the same volume as its sibling busses at the same scope level, but now sounds significantly quieter. So you try to find a happy medium of gain staging not too hard and not too soft. Now perhaps that works fine, and perhaps your bus compressor is now struggling to function optimally because it’s trying to apply a dynamics process to several audio sources that have no common dynamics ceiling. The bus compressor itself struggles to gain the necessary context in this case, and you’ll find yourself trying to fix it at the bus level when the problem is at the track-level and wondering why it’s not sitting in the right dynamic range “pocket.” This issue compounds further the more nested busses you have in your project, until by the time you reach the master, the overall proportion and consistency of your dynamics choices will be horribly inconsistent from track to track.

# Why Any of This Matters

## Predictability Creates Consistency

*The goal is to have coherent and predictable results across every process* you have to go through while creating a song. Understanding scopes of control quickly highlights quality of life functions that simply don’t exist inside of Ableton. Ableton doesn’t allow for polymorphism across scope level, where Bitwig easily succeeds in this manner.

Of course at the end of the day you should always be mixing with your ears, but anything you can do to make that process as consistent and streamlined as possible is a step you should take. The perceived value of a decibel will change as a sound gets louder or quieter, and that can’t be avoided. However, maximizing your track to unity by capping your FX chains with clipping or limiting ensures that the position of every fader informs you with the accurate context concerning dynamics, which then informs perceived loudness. This makes a MASSIVE difference when it comes to quickly getting that final mix to sit in the desired dynamic range.

## It's a Mental Framework

The point of all of this is to illustrate a general philosophy for getting the absolute tightest and most musical mixes possible. You want to precisely create your macros so that no values are being overshot and no dead or unwanted values are being sent. For example, if you were automating a filter frequency cutoff over time, instead of freely automating the cutoff directly and drawing points on your timeline at precise frequencies, set up a macro that explicitly covers only the frequency range that will be necessary in the song. Every cutoff automation can then be drawn in as 0% - 100%, or some other calculation based on frequency ratios, thereby utilizing the full resolution of the macro while staying in the desired frequency pocket. You could then create a “master” macro that controls several of these filter macros across different tracks or busses to easily automate transitions.

# Outro
