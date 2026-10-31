---
title: 'Depth-augmented ACoT-VLA'
subtitle: 'AgiBot World Challenge 2026 project'
summary: 'Multimodal policy adaptation with LoRA, depth conditioning, and coarse-to-fine action generation.'
type: page
date: 2026-10-31
draft: false
toc: true
share: false
commentable: false
image:
  filename: architecture.png
  alt_text: 'Depth-augmented ACoT-VLA inference architecture'
  preview_only: false
---

[Back to research](/#other-research) · [Architecture PDF](architecture.pdf) · [Full-resolution diagram](architecture.png)

## Project overview

As team lead for an AgiBot World Challenge 2026 project, I worked on adapting a pretrained pi0.5-LIBERO policy to the competition's robotic tasks. The project explored LoRA-based adaptation with depth information and iterative evaluation in Genie Sim 3.0.

The architecture shown here describes **Depth-augmented ACoT-VLA**: a visual-language backbone supplies task context, while depth information conditions a coarse-to-fine action-generation pipeline.

## How the architecture works

1. **Visual-language context.** RGB views are encoded by SigLIP, and language instructions are embedded into a PaliGemma main LLM adapted with LoRA. Prefix key-value features provide context to the action streams.
2. **Compact depth representation.** A shared DepthExpert processes depth maps and validity masks from head, left, and right views. A two-layer encoder and query pooling produce four tokens per view, giving 12 depth tokens with dimension 256.
3. **Coarse-to-fine actions.** The coarse Gemma expert produces an initial trajectory. The fine stream combines this trajectory with context-derived reasoning features and generates an action chunk. Both action streams receive depth information through separate projections and gated fusion.

**Where adaptation happens.** LoRA is applied in the main LLM; depth is fused into the action-expert inputs. The diagram omits separate noisy-action inputs, time conditioning, and iterative flow-matching updates for clarity.

## Event photograph

![Robot manipulation demonstration at an AgiBot event](agibot-demo.png)

*Robot manipulation demonstration at an AgiBot event.*

[Return to my homepage](/)
