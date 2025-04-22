# BRAID: Brain Representation to Artificial Image via Diffusion

## Description

**BRAID** is a project that aims to develop a model that takes fMRI features and generates images similar to the original stimulus image. The goal is to reconstruct what a subject is seeing using only neuronal activity, particularly focusing on the primary visual cortex (V1) and higher cortices.

## Proposal Document

[Project Proposal PDF](https://drive.google.com/file/d/1xiPgDY-aN5qrdm-rH8hykxNLwl5zz4Nv/view?usp=sharing)

## Motivation

Reconstruction of visual stimuli from neuronal activity in an interpretable manner could open a window into cognition and perception. Object decoding is a major leap in brain-computer interface (BCI) research with many potential applications.

## Existing Work

Notable related works include:
- MindEye (Scotti et al., 2023)
- MindEye2 (Scotti et al., 2024)
- Brain-Streams (Joo et al., 2024)
- NeuroPictor (Huo et al., 2024)

These works commonly rely on multi-modal data and subject-specific training, which introduce complexity and limit scalability.

## Proposed Solution

This project proposes a cross-modal approach using:
- An fMRI encoder trained with contrastive loss
- A Vision Transformer (ViT) acting as a teacher model
- A shared latent space for both fMRI and image embeddings

This eliminates the need for auxiliary modalities and promotes subject generalization.

## Timeline

| Week        | Milestone                                                |
|-------------|-----------------------------------------------------------|
| 4–6         | Literature review, data preprocessing, baseline analysis |
| 6           | Model architecture setup                                 |
| 7           | Implement distillation and contrastive loss              |
| 8           | Model training                                           |
| 9           | Evaluation and analysis                                  |
| 10          | Final write-up and submission                            |

## References

- [Scotti et al., 2023 – *Reconstructing the Mind's Eye: fMRI-to-Image with Contrastive Learning and Diffusion Priors*](https://arxiv.org/abs/2305.18274)  
- [Scotti et al., 2024 – *MindEye2: Shared-Subject Models Enable fMRI-To-Image With 1 Hour of Data*](https://arxiv.org/abs/2403.11207)  
- [Joo et al., 2024 – *Brain-Streams: fMRI-to-Image Reconstruction with Multi-modal Guidance*](https://arxiv.org/abs/2409.12099)  
- [Huo et al., 2024 – *NeuroPictor: Refining fMRI-to-Image Reconstruction via Multi-individual Pretraining and Multi-level Modulation*](https://arxiv.org/abs/2403.18211)
