---
layout: post
title: arMIDI
permalink: /collab-ar
gallery:
    - image_path: ../../../assets/img/performance/unspoken-nime-min.jpg
      caption: Unspoken
    - youtube_id: nwfC2Ch97O0?si=qoYGaxDczSdHXoyI
      caption: Unspoken at NIME Conference
---

arMIDI is a collaborative augmented reality interface that visualises musicians’ hand positions, eye gaze, and instrument activity. It gives electronic musicians a shared view of their interaction to support awareness and coordination while playing together.

**Keywords:** Interaction design, spatial visualisation, and functional prototyping.

## [-] The design challenge

Electronic instruments often have small controls that are obscured during performance. A musician’s movements may also reveal little about the resulting sound, making it difficult for collaborators to follow changes or anticipate one another’s actions. I explored how AR could make this information visible while musicians continued playing their existing instruments.

<figure>
  <img src="{{ '/assets/img/work/collab-ar-system.png' | relative_url }}" alt="Comparison of arMIDI’s bodily and instrument information: hand and gaze markers on the left, and highlighted notes and control values on the right, shown above the corresponding physical keyboard interactions." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Two visual design of feedback: hand and gaze positions (left), and notes and control changes (right). The upper panels show simulated views for the collaborator.</figcaption>
</figure>

## [-] Designing the interface

Each performer sees a virtual representation of their collaborator’s keyboard through a HoloLens 2 headset. The design combines two layers of information: bodily cues that communicate movement and attention, and instrument data that shows notes and control changes.

### Visual cues for movement and attention

Yellow spheres labelled “L” and “R” represent the collaborator’s palm positions. During iterative in-lab development, these offered more stable tracking and less visual clutter than fully rendered hands, which were prone to jitter.

A blue sphere shows gaze position. When the collaborator looks towards the virtual instrument, the marker freezes and enlarges to signal their attention. This approach communicates gaze while limiting distracting movement in the performer’s view.

### Making instrument interaction visible

The keyboard representation highlights active notes and controls in yellow. Animated knobs and faders reflect changes, with pink annotations displaying their current values. Bright colours were chosen for visibility through the headset under office lighting.


## [∞] Building the prototype

I built the interface in `Unity` and `C#` with `Microsoft MRTK`, with 3D modelling in `Blender`. A QR code anchors the virtual keyboard beside the physical instrument. A `Node.js` and `WebSocket` backend exchanges MIDI data between performers’ computers and headsets in real time.

## [>] Evaluation and design insights

A study with **eight musicians in four pairs** compared bodily cues, instrument activity, combined feedback, and no visualisation through improvisation, questionnaires, and interviews.

The combined feedback was preferred overall and supported greater self-reported awareness than bodily cues alone or no visualisation. Instrument feedback was considered easiest to understand and respond to, while hand and gaze cues helped some musicians anticipate actions and coordinate roles.

The study also highlighted an attention trade-off: additional information could distract from listening or be difficult to translate into a musical response. This points towards more selective feedback that prioritises meaningful changes and limits unnecessary detail.

## [>] Paper and performances

- [Seeing the Sound: Supporting Musical Collaboration with Augmented Reality](https://doi.org/10.1145/3698061.3726905), Creativity & Cognition 2025 — design and user study.
- [System demo](https://youtu.be/X6kQouxTiWM).
- Watch *Unspoken*, an artistic configuration performed at NIME 2024, in the video above.
- The interface also informed [off-the-shelf]({{ '/embodied-ai-ar' | relative_url }}), exploring visual feedback in human–AI musical collaboration.

[Back to all projects]({{ '/works' | relative_url }})
