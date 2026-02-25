

# Generative Video Translation for Ultrasound

[📄 Paper](https://arxiv.org/pdf/2511.03255)

AI has huge potential in medical imaging, but clinical ultrasound datasets are messy. Ultrasound contains multiple views, structures, and sub-modalities—like grayscale (B-mode) and color flow Doppler (CFD)—that are often imbalanced or confounding. Traditional image translation struggles in this domain due to noise and overlapping signals.

In my recent work, I propose a video translation pipeline that converts CFD ultrasound to grayscale while preserving anatomical fidelity, producing high-quality, clinically realistic videos for deep learning tasks.

---

## Features

- **High-quality synthesis**: Average SSIM of 0.91±0.04 between synthetic and real videos.
- **Clinically indistinguishable**: Blinded clinician evaluation showed 54±6% accuracy in distinguishing synthetic from real.
- **DL-ready synthetic data**: Synthetic videos perform equivalently to real ones in classification (F1 0.93–0.95) and segmentation (Dice 0.97±0.03) tasks.
- **Generalization**: Model trained on cardiac ultrasound also works across other anatomical sites (SSIM 0.91±0.05).
- **High efficiency**: ~164× faster than SOTA diffusion-based methods for real-time video inference.

---

## Impact

- **Dataset augmentation**: Recovered >40% more usable data for clinical deep learning tasks, improving class balance and diversity of **rare pathologies** in fetal ultrasound screening.
- **Foundational capability**: Reconstructs complex anatomy even under dense CFD signal, generalizing to structures not seen during training.
- **Clinical validation**: Combines computational metrics and blinded clinician perception to ensure realism and diagnostic integrity -- therefore improving trust in AI for healthcare.
- **Future potential**: Approach can extend to denoising, super-resolution, and other imaging modalities.

---

# code coming soon
