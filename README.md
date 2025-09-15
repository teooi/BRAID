# BRAID: Brain Representation to Artificial Image via Diffusion

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1WBlca3QtmsvAw67JJrmFbC0rJkmmLGSC?usp=sharing)

**BRAID** reconstructs images from fMRI brain activity using a cross-modal encoder and a pre-trained latent diffusion model (LDM). fMRI signals from the visual cortex are mapped into a latent space, which is then decoded into images by the frozen LDM and VAE decoder.

## Paper

[Project Paper (PDF)](https://drive.google.com/file/d/1j9X0CCV02v-jsGaxnceoX1eZoIzQR_OL/view?usp=sharing)

## Method

- A lightweight MLP encodes fMRI feature vectors into latent representations.
- Latents are injected into the SSD-1B image-to-image diffusion model.
- Only the encoder is trained; the diffusion model and decoder remain frozen.
  
## References

- [MindEye (Scotti et al., 2023)](https://arxiv.org/abs/2305.18274)
- [MindEye2 (Scotti et al., 2024)](https://arxiv.org/abs/2403.11207)
- [Brain-Streams (Joo et al., 2024)](https://arxiv.org/abs/2409.12099)
- [NeuroPictor (Huo et al., 2024)](https://arxiv.org/abs/2403.18211)
