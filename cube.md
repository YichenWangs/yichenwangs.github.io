---
layout: post
title: cube.
permalink: /cube
gallery:
    - image_path: ../../../assets/img/performance/sound-exploration.jpeg
      caption: Performing with Charles Martin at Canberra Cotemporary Art Space (May, 2024)
    - youtube_id: 86yEZquWsPs?si=l-RldIIzjEwYE1Jq&t=1406
      caption: Performance at "Andromeda is Coming and Artificial Friends" (May, 2024)
---

is an augmented reality musical instrument composed of tonal cubes arranged in a 3D spiral. Musicians use freehand gestures to activate tonal drone synthesis, playing combinations of cubes to form chords or individual cubes to explore tones with poly-synthesised textures.

## [-] Concept

What could a musical instrument look and feel like when it no longer needs a physical surface? *cube.* explores how spatial placement, movement, and gesture can become expressive musical controls in head-mounted AR system.

The virtual instrument can be positioned in the surrounding space, allowing musicians to move around it or place themselves within its large-scale form.

<figure>
  <img src="{{ '/assets/img/work/cubing-sound-inapp.jpg' | relative_url }}" alt="Final cube instrument: tracked hands reach into a cylindrical arrangement of coloured sound cubes to play individual notes and chords." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Final design: individual note cubes support direct finger interaction, chords, and flexible spatial composition.</figcaption>
</figure>

## [-] My contribution

I designed and prototyped three AR interaction concepts through iterative self-testing, followed by a study of the final design with 20 musicians. The work explored learnability, creative exploration, and the relationship between spatial interaction and musical expression.

## [-] Three interaction designs

The instrument evolved through [autobiographical design](https://doi.org/10.1145/3492342): building, playing, and reflecting on each prototype to explore how spatial interaction could support musical expression.

### 1. Sound cubing as a physical interface

The first design drew on a physical synthesiser interface: a virtual panel of buttons and faders mapped to synthesis parameters on one side of a 3D cube. The left side provided tuning controls for two oscillators, while the right side contained an ADSR envelope and a filter. Musicians could operate the controls with hand gestures and freely reposition the whole cube in space.

This design explored how a traditional synthesiser interface would work in an AR headset. Through self-testing, I found that precise freehand manipulation of the panel was slow through the hand-tracking interface, making real-time sound tuning difficult.

<figure>
  <img src="{{ '/assets/img/work/p1-label.jpg' | relative_url }}" alt="First prototype: a movable virtual synthesiser panel with labelled oscillator, envelope, and filter controls, alongside a hand interacting with its sliders." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>First design: translating a physical synthesiser panel into AR exposed the difficulty of precise freehand control.</figcaption>
</figure>

### 2. Sound cubing through spatial interaction

The second design simplified the interface into two connected cubes, each representing an oscillator, with the movement of one modulating the other. Sound controls were mapped to movement around the performer’s body, extending interaction beyond a single panel in front of them.

Using far-pointer hand interactions, musicians could move the cubes horizontally and vertically or change their size to adjust the sound. Vertical movement controlled pitch, horizontal movement adjusted modulation, and size controlled volume. Filter controls were hidden with predefined settings, allowing performers to walk freely while continuing to shape the synthesis process.

In self-testing, consolidating multiple sound parameters into spatial controls made the interface easier to use. The simplification also reduced sonic diversity and musical richness.

<figure>
  <img src="{{ '/assets/img/work/p2-label.jpg' | relative_url }}" alt="Second prototype: two oscillator cubes with annotations mapping vertical movement to pitch, horizontal movement to modulation, and cube size to volume." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Second design: moving and resizing two sound cubes simplified control, with a trade-off in sonic variety.</figcaption>
</figure>

### 3. Sound cubing through flexible finger composition

The final design consists of individual sound cubes, each representing a musical note, arranged as a cylindrical MIDI keyboard. Musicians activate a cube by intersecting it with a finger. Full-hand tracking allows multiple notes to be played simultaneously, supporting chords and different note combinations.

The cylinder was sized so that most cubes could be reached from one standing position. Musicians could grab its centre to rotate the arrangement and access different notes. Colours distinguish tones, while rim lights identify semitones.

As in the second prototype, synthesis parameters were predefined. The design focused on ease of finger interaction and flexibility in musical composition, allowing performers to explore individual notes and chords within a spatial arrangement.


## [∞] Building the instrument

I built the prototypes in `Unity` with `Microsoft MRTK`, using `C#` and [DisunityST](https://github.com/digego/DisunityST) for real-time audio synthesis.

## [>] Evaluation and insights

The study with 20 musicians explored how mobility and the tangibility of spatial interaction shaped their experience. The research identified opportunities for intuitive, exploratory interaction, alongside a need for customisable sound controls to accommodate different creative preferences.

## [>] Research and performances

- [Design and development paper](https://nime.pubpub.org/pub/w82of2do/release/1), NIME 2022.
- [User study](https://zenodo.org/records/11189129), NIME 2023.
- [beyond realms.](https://youtu.be/5QUpw_7yZqU?si=2zG3zBatRQoHtkLE), with Sandy Ma at ACMC 2023.
- [Musicality](https://youtu.be/gQ5jUTbto1M?si=plS0cD1szBdlMb), with Charles Martin at NIME 2023.
- Watch the performance with Charles Martin at Canberra Contemporary Art Space in the video above.

[Back to all projects]({{ '/works' | relative_url }})
