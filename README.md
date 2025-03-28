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

| Model       | Inception Score (IS) | Fréchet Inception Distance (FID) |
|-------------|----------------------|----------------------------------|
| **LSGAN**   | 1.74 ± 0.11          | 248.95266723632812               |
| **WGAN**    | 2.11 ± 0.14          | 241.6168975830078                |
| **WGAN-GP** | 1.88 ± 0.13          | 243.53286743164062               |

✅ **WGAN-GP** performed the best in both realism and closeness to real distribution.


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
