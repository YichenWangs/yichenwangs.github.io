---
layout: post
title: arMIDI
permalink: /adc-poster/collab-ar
gallery:
    - image_path: ../../../assets/img/performance/unspoken-nime-min.jpg
      caption: Unspoken
    - youtube_id: nwfC2Ch97O0?si=qoYGaxDczSdHXoyI
      caption: Unspoken at NIME Conference
---

is a mixed reality interface that explores how augmented reality (AR) can enhance musician's awareness and mutual engagement in collaborative electronic music-making. The system presents a head-mounted AR visualisation of a generic electronic music keyboard, inspired by [Artural MiniLab 3](https://www.arturia.com/products/hybrid-synths/minilab-3/overview). The interfaces visualises each musician's hand positions, eye gaze and MIDI interaction on the keyboard in real-time through a WebSocket network infrastructure.

The project addresses a [wicked issue](https://nime.org/proc/nime22_35/index.html) in digital musical instruments: the challenges of effective communication and engagement due to limited visibility and reduced gestural or non-verbal interaction. These constraints can hinder musicians' situational awareness, making cohesive performances more difficult to achieve.

## [-] Design and Development

The interface was developed in `Unity` in `C#` with `Microsoft MRTK` for HoloLens 2, and the 3D model was created in Blender.
On the back end, musical interaction (MIDI) data from each performer's keyboard and computer was captured by a [`Node.js`](https://github.com/nodejs/node) application and transmitted to the other performer’s headset via a server using [`WebSocket`](https://github.com/websockets/ws) messages. The virtual keyboard appears next to each musicians’ physical electronic instrument [e.g., MiniLab 3], and can be anchored in space using a QR code tag.


## [>] More

- A user study with 8 musicians was conducted to explore their experiences regarding awareness and engagement in collaborative music-making. If you would like to know more, please feel free to email me for additional information!
- Watch _Unspoken_, an alternative artistic configuration of the system, performed at NIME'24 in the video link at the top.
- You can also watch the system [demo](https://youtu.be/X6kQouxTiWM).



<br>
<br>
[Back to Projects](../../../adc%20poster)
