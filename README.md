# GAN Evaluation on MedMNIST (PathMNIST Dataset)

This repo compares **LSGAN**, **WGAN**, and **WGAN-GP** trained on the **PathMNIST** dataset using the MedMNIST collection.

## 🚀 Objective

Evaluate GAN performance on medical image synthesis using:

- 🔍 Visual Inspection (via TensorBoard & PNGs)
- 📊 Inception Score (IS)
- 📉 Fréchet Inception Distance (FID)

## 🧠 Models Compared

| Model    | Type                    |
|----------|-------------------------|
| LSGAN    | Least Squares GAN       |
| WGAN     | Wasserstein GAN         |
| WGAN-GP  | WGAN + Gradient Penalty |

## 📊 Evaluation Results

| Model     | Inception Score (IS) | Fréchet Inception Distance (FID) |
|-----------|----------------------|----------------------------------|
| **LSGAN** | 4.12 ± 0.18          | 41.5                             |
| **WGAN**  | 3.95 ± 0.22          | 47.2                             |
| **WGAN-GP** | 4.68 ± 0.20        | 34.9                             |

✅ **WGAN-GP** performed the best in both realism and closeness to real distribution.

## 🖼 Sample Outputs

| LSGAN | WGAN | WGAN-GP |
|-------|------|---------|
| ![](images/lsgan_45.png) | ![](images/wgan_45.png) | ![](images/wgan-gp_45.png) |

## 📂 Folder Descriptions

- `gansexp.ipynb`: Full training and evaluation code
- `images/`: Generated samples
- `runs/`: TensorBoard logs
- `models/`: (optional) Saved model weights

## 📈 Visual Inspection

Launch TensorBoard:
```bash
tensorboard --logdir=runs
```

## 🔗 Author

Sharry Dhiman – [LinkedIn](https://www.linkedin.com/in/sharrydhiman)
