---
date: 2017-5-5
published: true
title: "MIDI to LED"
description: "Transform MIDI keyboard signal to Visual LEDs"
project_tags: python, class project
media: Website
ownership:
time_period: Spring 2017
thumbnail: "/projects/midi/leds.gif"

website:
  button_text: Visit the project github.
  url: https://github.com/sahahn/midi_2_led

intro: |
  The goal of this class project was to convert MIDI signal into DMX signal, where MIDI is generated from something like an electric keyboard and DMX signal is used to control professional LED lights. This project by far represents the highest ratio of cool idea to bad coding of any project I've ever done. To be fair though, I had only learned python a few months earlier and this was the largest project I had attempted - and also in the end, it worked without bugs magically ... so who says you can't code in one giant file filled with nested for loops? See the [terrible code](https://github.com/sahahn/midi_2_led). Or really... just check out the videos below instead and please never look at the code. The video's importantly contain audio.
  
  Shown below are a number of different examples of different modes that were programmed, where the base behavior across all examples is the idea that color of the lights is determined by the note being played based on the traditional 12 note scale. Further, the intensity of the light also matches how hard the key is played on the keyboard.

content_layout:

  - section_layout: 2col
    videos:
      - caption: Example showing modes "Value Shift" and "Chord Chaos". Value shift makes it so that when a note or multiple notes are held, they will start to shift to the left, and the longer they are held, the faster they will shift. This results in the observed behavior where lights in the video above start to move faster and faster across the lines of lights. The other activated mode, chord chaos, says that when multiple notes are played, as in a chord, their initial placement will be random - resulting in a "chaotic" positioning of which lights are activated. 
        description: Example 1
        url: https://www.youtube.com/embed/Q8Tk1M4IgpE

      - caption: This example video exhibits the "Double" mode. Double describes the behavior that when notes are pressed, they should appear on both the far left and far right, and if multiple notes pressed, they be filled in the next avaliable spot on either end. This results in behavior where when any notes are played they appear on two lights to either side.
        description: Example 2
        url: https://www.youtube.com/embed/bsNoRV7Eb2Y

      - caption: The example highlights two different modes, "single note" and "sticky". Single note says that all of the avaliable lights should change to the color of the last played note. Further, sticky mode says that this value will not fade out, but instead stay even if the key is released. This results in the observed behavior shown in the video where the lights retain 
        description: Example 3
        url: https://www.youtube.com/embed/w3B-1EW2MSo

      - caption: This examples shows modes "sticky" and base "chord" behavior. Sticky says that after a note is played, it will not fade out, but instead remain with the same color and intensity as defined by the original input. This is combined with "chord" behavior, where each played note controls a single LED, and is assigned sequentially from left to right across the avaliable lights.
        description: Example 4
        url: https://www.youtube.com/embed/042kaBATpds

      - caption: This example shows modes "Chord Chaos", "Strobe" and use of the pitch wheel. Chord Chaos mode just says that when multiple notes are played, as in a chord, their initial placement will be random - resulting in a "chaotic" positioning of which lights are activated. The shown strobe function is applied when the "mod" wheel of the MIDI keyboard is used. Essentially when activated, any lights currently on will flicker in a strobe like manner, where the speed of the flickering is set by the value of the "mod" wheel. The other shown function in this video is the use of the pitch wheel, which lowers a played note by up to one octave, and as a result the note will change colors accordingly to match whatever the note, or value between notes, is being heard.
        description: Example 5
        url: https://www.youtube.com/embed/Eih_KhQyiv0

      - caption: This video shows modes "single note", but highlights the ability to customize how long each light can be set to both fade in and fade out. Fading in defined how long it should take while a note is being held for it to reach the maximum intensity as defined by the velocity of the initial  press. Fade out defines the amount of time after the note is released until the light is fully off. This video in particular highlights some interesting interactions that occur when the fade-out time is long, where the previous color will still be fading out even after a new color is fading in, which results in combinations of colors as calculated by a mix of the new and old colors.
        description: Example 6
        url: https://www.youtube.com/embed/-cOBobb4gyw

      - caption: This example shows special mode "leftify" which says that notes should always be as far left as possible, and show up according to the order they were pressed. This difers from other modes in that if a previous key is released, it essentially frees up an earlier spot, so that all notes being held to the right will then shift to fill the free spot.
        description: Example 7
        url: https://www.youtube.com/embed/pIqBf1KsHaQ

      - caption: This example shows special mode "leftify" which says that notes should always be as far left as possible, and show up according to the order they were pressed. This difers from other modes in that if a previous key is released, it essentially frees up an earlier spot, so that all notes being held to the right will then shift to fill the free spot.
        description: Example 8
        url: https://www.youtube.com/embed/qmIDU4kbc8s

      - caption: This example shows a case where the program is extended to work with other MIDI devices, in this case a drum-machine. In this example I cycle through a few different modes and behaviors.
        description: Example 9
        url: https://www.youtube.com/embed/PC34eS8qTjY

      - caption: This shows another example where a drum machine is used to trigger LED signals instead of a keyboard. A few different modes are cycled through in this example.
        description: Example 10
        url: https://www.youtube.com/embed/-K-Lj-gQw3A


---
