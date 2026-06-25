# NaLA: A 3D Native LLM Layout Agent for High-quality 3D Scene Generation

**ECCV 2026**

<p align="center">
  <a href="https://adamcwan.github.io/NaLA/"><strong>Project Page</strong></a> |
  <a href="https://arxiv.org/"><strong>arXiv</strong></a> |
  <a href="https://github.com/adamcwan/NaLA-code"><strong>Code</strong></a>
</p>

<p align="center">
  <img src="assets/teaser.jpg" alt="NaLA teaser" width="90%">
</p>

---

## Introduction

This is the official implementation of **NaLA**, a 3D-native LLM layout agent for high-quality 3D scene generation, accepted at ECCV 2026. Existing LLM-based layout agents are limited to text or image inputs, which fail to capture detailed 3D geometry, and rely on token-by-token textual pose prediction that is inefficient and imprecise. NaLA addresses both issues by encoding point clouds of scenes and assets as native 3D tokens and generating placements through a coarse-to-fine pose decoding strategy, enabling end-to-end reasoning over 3D geometry for physically and semantically plausible layouts.

### Pipeline Overview

NaLA follows an end-to-end pipeline. First, point clouds of the scene and each asset are encoded into tokens. These input 3D tokens are combined with text tokens and fed into the LLM. Then, the model utilizes specially-designed output anchoring tokens to predict a coarse grid location and orientation, followed by output residual tokens that produce fine-grained pose residuals, scale, and rotation refinement. Special ID tokens ensure each predicted pose is matched to the correct asset.

---

## Code Release

🚧 **Code is coming soon.** We are currently cleaning up and organizing the codebase for public release. Stay tuned!
