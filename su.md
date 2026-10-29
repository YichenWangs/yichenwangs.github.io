---
layout: post
title: "Sù 溯: AI-assisted Musical Interface"
permalink: /su
gallery:
    - image_path: ../../../assets/img/work/feedback-latent-system.jpg
      caption: "回溯: Co-constructing a Dual Feedback Apparatus — performance at NIME 2026."
    - youtube_id: 7RdtMOFNOSM?si=BaasZyeqb2ILJeXv
      caption: Performing 溯 at NIME 2026.
---

Sù is a musical interface for direct manipulation of a real-time generative audio system built around [RAVE](https://github.com/acids-ircam/rave). The project explores how a technically complex latent synthesis model can become a tool for creative control and audio spatialisation.

## [-] Design and Development

The work began as a greenfield research project during my research internship at Dolby's Advanced Technology Group in Australia in 2025.

I was drawn to the appealing concept of "feedback" in creative control design, inspired by [Tom Mudd's research](https://dl.acm.org/doi/10.1145/3544548.3580662). The possibility of nonlinear interaction bringing unpredictability, immediacy, and entangled agency to our experiences with technological interfaces seemed exciting, opening up space for the future design of AI-powered creative tools.

With supervision and mentoring from David Gunawan, Benjamin Southwell, and David Cooper, we explored the implementation of feedback loops within a latent synthesis model. This approach combines direct control with a degree of randomness or chance, inviting users and creators to explore and discover sounds during content creation.

The core sound engine, including the RAVE component, was implemented in `Max/MSP`, alongside a mixed reality interface for object-based audio spatialisation developed in `Unity` using `C#` and the Meta OpenXR SDK, running on a Meta Quest 3 headset.

<figure style="max-width: 560px; margin: 2rem auto;">
  <img src="{{ '/assets/img/work/su-system-diagram.png' | relative_url }}" alt="Sù system diagram showing an outer audio feedback loop and an adjustable inner feedback loop for latent variables between the RAVE encoder and decoder." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Sù's outer audio feedback loop and adjustable inner feedback loop between the RAVE encoder and decoder.</figcaption>
</figure>

[Back to all projects]({{ '/works' | relative_url }})
