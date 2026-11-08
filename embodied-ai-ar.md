---
layout: post
title: off-the-shelf.
permalink: /embodied-ai-ar
gallery:
    - image_path: ../../../assets/img/work/yichen-off-the-shefl.jpg
      caption: off-the-shelf at "Andromeda is Coming and Artificial Friends" gig
    - youtube_id: ZXX3JvFNL2k?si=JUcDsBIt67U3fZFz
      caption: Performance recording
---

off-the-shelf is an augmented reality interface for collaborative music-making with an AI musician. It visualises notes, controls, and sound parameters so performers can follow contributions and respond while improvising.

**Keywords:** Interaction design, functional prototyping, performance-based iteration, and user research.

## [-] The design challenge

Electronic music can be difficult to follow through sound alone. When several instruments overlap, musicians may struggle to identify who is contributing and which parameters are changing.

I explored how visual feedback could help musicians understand this activity while staying engaged in the creative process.

## [-] Designing the interface

I adapted my [arMIDI]({{ '/collab-ar' | relative_url }}) system into a working AR prototype connected to the [IMPSy](https://github.com/cpmpercussion/impsy/tree/main) generative music system. Three decisions shaped the interface:

- **Represent musical interaction data.** A generic keyboard-and-control layout organises note events, control changes, and parameter values across different electronic instruments. It represents musical activity at the data level, rather than reconstructing bodily gestures.
- **Make changes visible as they happen.** Keys light up yellow when notes play, while seven virtual knobs reflect changes to sound parameters. Performers can connect what they hear with what is changing.
- **Distinguish collaborators.** In group sessions, grey and purple representations separate the human and AI contributors, with yellow highlights showing current activity. The visualisations sit within the performance space through an AR headset.

<figure>
  <img src="{{ '/assets/img/work/holo-in-app-view-processed.jpg' | relative_url }}" alt="View through the AR headset showing a grey representation of the human musician’s activity on the left and a purple representation of the AI musician’s activity on the right, with yellow highlights on active notes and controls." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Human (left, grey) and AI (right, purple) musical interaction data visualised in AR. Yellow highlights indicate active notes and control changes.</figcaption>
</figure>

I built the interface in `Unity` with `Microsoft MRTK` for HoloLens 2, using `Node.js` and `WebSocket` to exchange MIDI data in real time.

<figure>
  <img src="{{ '/assets/img/work/off-system-architect.jpg' | relative_url }}" alt="System diagram connecting the musicians, AI music system, and AR interface through a network." style="display: block; max-width: 100%; width: 560px; margin: 0 auto;" loading="lazy">
  <figcaption>The interface translates live musical interaction data into visual feedback.</figcaption>
</figure>

## [-] Prototyping through performance

I explored the prototype through recorded demos, a live research concert, and trio improvisation. Each setting exposed different constraints.

The first setup visualised notes but offered limited control over sound character. A later configuration expanded the system’s parameter control, creating more varied textures and opportunities for musical call and response. Trio sessions added visualisations for both collaborators and explored shared versus separate instruments, revealing how the setup shaped the AI’s perceived role.

These experiences also exposed a persistent interaction problem: fast-changing activity could be visible without being easy to follow.

## [-] Evaluating with 16 musicians

I conducted a study with 16 experienced electronic musicians to understand how visual feedback affected their creative experience, both alone with the AI and alongside another human musician.

<!-- Every participant tried four conditions:

| Setting | Visual feedback off | Visual feedback on |
| --- | --- | --- |
| One human + AI | Sound only | AI activity shown |
| Two humans + AI | Sound only | Human and AI activity shown |

Participants attended individual and group sessions on separate days, completing 5–10-minute improvisations followed by semi-structured interviews. Visualisation order was balanced. Headsets were worn in all conditions; group participants sat back-to-back to focus communication on sound and the interface. -->
<!-- 
I led coding and theme development from **431 minutes of interview data**, refining the analysis with my collaborator. -->

## [>] Outcome

**Visibility needs to support action.** Seeing notes and parameter changes helped some musicians identify contributions and respond deliberately. Rapid activity could still be difficult to interpret, and clearer information did not consistently lead to better collaboration.

<!-- **Feedback should respect creative attention.** Some musicians valued the visual reference; others preferred to listen. This suggests opportunities for contextual feedback that offers clarification when needed. Adaptive feedback remains a direction for future prototyping. -->

**Design for people creating together.** A second human often provided stability and shared understanding. The interface supported this connection as well as awareness of the AI, highlighting the importance of supporting human coordination in creative tools.

The study informed design directions for readable, attributable feedback and flexible collaboration. It provides qualitative insights from music sessions with experienced musicians.

## [>] Papers and performance

- [AI See, You See](https://doi.org/10.1145/3706599.3720052), CHI Extended Abstracts 2025 — interface design and performance-based exploration.
- [Practice-based research paper](https://aimc2024.pubpub.org/pub/ll85912p/release/1), AIMC 2024.
- *Negotiating Human–AI Co-Creativity in Music with In-Process Visualisation* — manuscript reporting the 16-musician study.
- Watch the performance recording above.

[Back to all projects]({{ '/works' | relative_url }})
