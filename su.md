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

Sù is a musical interface for directly manipulating a real-time generative AI audio model through responsive feedback. It translates a technically complex latent synthesis model into hands-on creative controls, enabling creators to explore and shape sound within the model’s latent domain.

## [-] Concept

Control of generative audio systems typically involves manipulating input and output audio signals in the time or sample domain. This limits the creative possibilities available to users by restricting where they can intervene in the generative process.

Sù extends user control into the model’s latent domain, opening up different creative and aesthetic possibilities for generating and modifying sound.

I was drawn to feedback as a creative design approach, inspired by [Tom Mudd’s research](https://dl.acm.org/doi/10.1145/3544548.3580662). The possibility of nonlinear interaction bringing unpredictability, immediacy, and entangled agency to our experiences with technological interfaces suggested new directions for AI-powered creative tools. In Sù, this motivated an exploration of feedback as a way for creators and the generative system to shape an evolving musical process together.

The project began during my research internship with Dolby’s Advanced Technology Group in Australia in 2025, exploring how latent-domain feedback could support creative control of generative audio.

## [-] My contribution

I designed and developed the musical interface, translating the latent synthesis model into creative controls for generating and modifying sound through responsive feedback. I independently delivered the mixed reality prototype and collaborated on latent-domain feedback research through experimental audio prototyping, contributing as a co-inventor to a US patent.

## [-] Interaction and development

The sound engine uses [RAVE](https://github.com/acids-ircam/rave) for real-time generative audio. We explored feedback loops within the latent synthesis model, allowing creators to intervene in an evolving sound process whose responses can be immediate and unpredictable. This approach combines direct manipulation with opportunities for discovery as the performer and system influence one another.

I developed the prototype with supervision and mentoring from David Gunawan, Benjamin Southwell, and David Cooper. The sound engine was implemented in `Max/MSP`. A supporting mixed reality interface enables object-based audio spatialisation, built in `Unity` and `C#` for Meta Quest 3 using the Meta OpenXR SDK.

## [>] Outcome

The prototype demonstrates how direct latent-domain control and the use of feedback concept can turn a complex generative AI audio model into a tool for creative sound exploration. It gives creators a way to influence sound within the generative process, expanding the possibilities for generating and modifying musical material. The performance recording above shows Sù in use at NIME 2026.

<figure style="max-width: 560px; margin: 2rem auto;">
  <img src="{{ '/assets/img/work/su-system-diagram.png' | relative_url }}" alt="Sù system diagram showing an outer audio feedback loop and an adjustable inner feedback loop for latent variables between the RAVE encoder and decoder." style="display: block; width: 100%; height: auto;" loading="lazy">
  <figcaption>Sù's outer audio feedback loop and adjustable inner feedback loop between the RAVE encoder and decoder.</figcaption>
</figure>

[Back to all projects]({{ '/works' | relative_url }})
