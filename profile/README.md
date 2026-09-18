Open Engineering Video

Open Engineering Video is the implementation repository of the definitions from Open Engineering Videos.

Open Engineering Video provides the software, tooling, pipelines, and runtime components required to create, process, compose, render, and publish engineering videos from their definitions.

Relationship with Open Engineering Videos

Open Engineering separates what something is from how it is implemented.

* Open Engineering Videos — definitions of engineering videos, their structure, scenes, sequences, assets, narratives, and production intent.
* Open Engineering Video — implementation of those definitions through software, workflows, generators, renderers, and supporting services.

This follows the Open Engineering convention:

Plural = definition · Singular = implementation

Purpose

Open Engineering Video turns declarative video definitions into reproducible video artifacts.

A video definition can describe, for example:

* the subject and narrative
* scenes and sequences
* cameras and viewpoints
* 3D models and other assets
* animation and motion
* narration and dialogue
* music and sound effects
* transitions and timing
* captions and on-screen text
* rendering requirements
* output formats and destinations

The implementation repository provides the machinery to turn those definitions into actual video productions.

From Definition to Video

Open Engineering Videos
        │
        │  video definitions
        ▼
Open Engineering Video
        │
        ├── assets
        ├── scenes
        ├── cameras
        ├── animation
        ├── narration
        ├── audio
        ├── composition
        └── rendering
        │
        ▼
   Video Artifact

The goal is a pipeline in which the definition remains the source of truth, while the implementation can evolve independently.

Engineering Videos as Artifacts

Open Engineering Video treats a video as an engineered artifact rather than merely a rendered file.

A production can therefore be:

1. Defined — expressed through Open Engineering Videos.
2. Resolved — references to models, images, textures, audio, text, and other assets are resolved.
3. Composed — scenes, cameras, animation, narration, and timing are assembled.
4. Rendered — the production is rendered into one or more media formats.
5. Published — resulting video artifacts can be distributed through appropriate channels.
6. Reproduced — the same definition can be processed again as the implementation evolves.

Integration

Open Engineering Video is intended to integrate with other Open Engineering repositories, including:

* Open Engineering Models — 3D engineering models and scene assets
* Open Engineering Images — generated and processed visual assets
* Open Engineering Textures — UVs, decorations, and texture assets
* Open Engineering Tours — camera-driven journeys through engineering scenes
* Open Engineering Presentations — presentation-oriented visual narratives
* Open Engineering Architecture — architectural models and engineering context

Together these repositories can form a composable production pipeline:

Definitions
     │
     ├── Architecture
     ├── Models
     ├── Images
     ├── Textures
     ├── Tours
     └── Presentations
             │
             ▼
    Open Engineering Video
             │
             ▼
       Video Artifacts

Design Principles

Declarative

Describe what the video should contain, rather than hard-coding every production step.

Reproducible

A video should be reproducible from its definition and referenced assets.

Composable

Scenes, models, images, audio, tours, presentations, and other assets should be reusable building blocks.

Automated

Where practical, production steps should be executable by software rather than manually repeated.

Traceable

A rendered video should be traceable back to its definition, assets, implementation version, and production parameters.

Open

The implementation should favor open formats, open tooling, and composable interfaces.

The Production Loop

Open Engineering Video is intended to support a continuous production loop:

Define
  ↓
Compose
  ↓
Render
  ↓
Review
  ↓
Refine
  ↓
Render again

Changes to a definition or its underlying assets should therefore be able to flow through the production pipeline without rebuilding the entire workflow manually.

Repository Scope

This repository is concerned with implementation.

Definitions belong in:

Open Engineering Videos

Implementations belong here:

Open Engineering Video

This separation allows definitions to remain stable while implementations, rendering engines, automation, and production technology continue to evolve.

⸻

Open Engineering Video
Implementation for engineering videos defined by Open Engineering Videos.
