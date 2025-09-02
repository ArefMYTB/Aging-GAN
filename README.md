# Latent Age Editing with StyleGAN1 (PyTorch)

This repository implements StyleGAN1 from scratch (PyTorch) and demonstrates how to control facial age by discovering a latent-space age boundary.

The overall flow used in this project:

- Train a StyleGAN1 generator on FFHQ (16 hours on Colab T4 GPU - reach out for the PyTorch model weights).

- Compute an age boundary in the generator’s W-space using CelebA (pairs of young/old).

- Edit images (inverted real images or generated samples) by moving their latent code along boundaries['age'] to make faces older/younger.

---

Sample Images:

<img width="128" height="128" alt="image" src="https://github.com/user-attachments/assets/0ea6a36d-5608-45fd-ab2c-18d035b98336" />

<img width="128" height="128" alt="image" src="https://github.com/user-attachments/assets/9bffa023-6d60-4afb-98c1-ea391be2dd49" />
