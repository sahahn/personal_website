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

  The following videos exhibit a few interesting different modes:
  
  - "Value Shift": Value shift makes it so that when a note or multiple notes are held, they will start to shift to the left, and the longer they are held, the faster they will shift. This results in the behavior where lights will start to move faster and faster across the lines of lights.
  
  - "Base Chord": The base choard behavior defines behavior where each played note controls a single LED, and is assigned sequentially from left to right across the avaliable lights. So if two keys are pressed, the first will be assigned to the far left, and the next, one light to the right. 

  - "Chord Chaos": This mode says that when multiple notes are played, as in a chord, their initial placement will be random - resulting in a "chaotic" positioning of which lights are activated.

  - "Double Mode": Double describes the behavior that when notes are pressed, they should appear on both the far left and far right, and if multiple notes pressed, they will fill in the next avaliable spot on either end. This results in behavior where when any notes are played they appear on two lights to either side. 
  
  - "Single Note": Single note says that all of the avaliable lights should change to the color of the last played note. This means that only a single color will be active at once, and will be displayed across all avaliable lights.

  - "Sticky Mode": Sticky mode says that whatever the last value / color displayed will not fade out, but instead stay even if the key that triggered it is released. 

  - "Strobe": The shown strobe function is applied when the "mod" wheel of the MIDI keyboard is used. Essentially when activated, any lights currently on will flicker in a strobe like manner, where the speed of the flickering is set by the value of the "mod" wheel.

  - "Pitch Wheel": The pitch wheel function can be used to lower or raise the played notes by up to an octave, and as a result the note will change colors accordingly to match whatever the note, or value between notes, is being heard.
  
  - "Leftify": This mode says that notes should always be as far left as possible, and show up according to the order they were pressed. This difers from other modes in that if a previous key is released, it essentially frees up an earlier spot, so that all notes being held to the right will then shift to fill the free spot.
content_layout:

  - section_layout: 2col
    videos:
      - caption: Example showing modes "Value Shift" and "Chord Chaos", as described above.
        description: Example 1
        url: https://www.youtube.com/embed/Q8Tk1M4IgpE

      - caption: This example video exhibits the "Double" mode, as described above.
        description: Example 2
        url: https://www.youtube.com/embed/bsNoRV7Eb2Y

      - caption: The example highlights two different modes, "Single note" and "Sticky".
        description: Example 3
        url: https://www.youtube.com/embed/w3B-1EW2MSo

      - caption: This examples shows modes "Sticky" and "Base Chord" combination of modes. 
        description: Example 4
        url: https://www.youtube.com/embed/042kaBATpds

      - caption: This example shows modes "Chord Chaos", "Strobe" and "Pitch Wheel". 
        description: Example 5
        url: https://www.youtube.com/embed/Eih_KhQyiv0

      - caption: This video shows mode "Single note", but highlights the ability to customize how long each light can be set to both fade in and fade out. This video in particular highlights some interesting interactions that occur when the fade-out time is long, where the previous color will still be fading out even after a new color is fading in, which results in combinations of colors as calculated by a mix of the new and old colors.
        description: Example 6
        url: https://www.youtube.com/embed/-cOBobb4gyw

      - caption: This example shows mode "Leftify".
        description: Example 7
        url: https://www.youtube.com/embed/pIqBf1KsHaQ

      - caption: This example shows mode "Leftify".
        description: Example 8
        url: https://www.youtube.com/embed/qmIDU4kbc8s

      - caption: This example shows a case where the program is extended to work with other MIDI devices, in this case a drum-machine. In this example I cycle through a few different modes and behaviors.
        description: Example 9
        url: https://www.youtube.com/embed/PC34eS8qTjY

      - caption: This shows another example where a drum machine is used to trigger LED signals instead of a keyboard. A few different modes are cycled through in this example.
        description: Example 10
        url: https://www.youtube.com/embed/-K-Lj-gQw3A


---
