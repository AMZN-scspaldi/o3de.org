---
title: "Developer Guide"
description: "Learn about the systems and interfaces behind the Atom Renderer"
toc: true
weight: 600
---

This section provides a deeper technical read into the systems and interfaces underlying the Atom Renderer. 

| Contents                        | Details |
|--------------------------------------|---------|
| [Frame Rendering](frame-rendering/) | The frame rendering process describes how a scene is processed from Render Components, through Render Passes in the RPI, and to the RHI. |
| [Material System](materials/) | The material system processes materials and material types and builds them into assets to use in the simulation. |
| [Shader System](shaders/) | The shader system processes shaders written in AZSL (Amazon Shading Language) and builds them into shader assets that can be used in your project. |
| [Render Pipeline Interface (RPI)](rpi/) | The Render Pipeline Interface (RPI) contains the main interface for developers to program the render pipeline. |
| [Passes](passes/) | The pass system transforms data from a scene into a final rendered output. |
| [Rendering Hardware Interface (RHI)](rhi/) | The Rendering Hardware Interface (RHI) provides a low-level interface that abstracts platform-specific code. |
