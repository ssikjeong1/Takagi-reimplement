# Takagi-reimplement
Reimplement of the High-resolution image reconstruction with latent diffusion models from human brain activity (CVPR 2023)

## Environment setup
1. Download ``nsddata``, ``nsddata_betas``, and ``nsddata_stimuli`` from NSD and place them under the ``nsd`` directory.
2. ``pip install -r requirements.txt``
3. Install Stable Diffusion v1.4 (under the ``diffusion_sd1/`` directory), download checkpoint (``sd-v1-4.ckpt``), and place it under the ``codes/diffusion_sd1/stable-diffusion/models/ldm/stable-diffusion-v1/`` directory.
4. __(optional)__ For incorporating GAN, install ``bdpy`` (under the ``gan/`` directory), download ``VGG_ILSVRC_19_layers`` and ``bvlc_reference_caffenet_generator_ILSVRC2012_Training`` from https://figshare.com/articles/dataset/brain-decoding-cookbook/21564384, and place them under the ``codes/gan/models/pytorch/`` directory.
5. For incorporating decoded depth, install Stable Diffusion v2.0 (under the ``diffusion_sd2/`` directory), download checkpoint (``512-depth-ema.ckpt``), and place it under the ``codes/diffusion_sd2/stablediffusion/models/`` directory. 

## MRI Preprocessing
```
cd codes/utils/
python make_subjmri.py --subject subj01
```







# Acknowledgement
Our implementation of this work builds on the following repositories. We would like to thank the authors.

> https://github.com/yu-takagi/StableDiffusionReconstruction

> https://github.com/CompVis/stable-diffusion

> https://github.com/Stability-AI/stablediffusion

> https://github.com/gallantlab/himalaya

> https://github.com/tknapen/nsd_access

> https://github.com/salesforce/BLIP

> https://github.com/KamitaniLab/bdpy

> https://github.com/KamitaniLab/brain-decoding-cookbook-public

> https://github.com/isl-org/DPT

# Contact
Plase [email](ssikjeong1@korea.ac.kr) if you have any questions.
