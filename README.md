# Emergency vs Non-Emergency Vehicle Image Denoising

Some images in the Emergency vs Non-Emergency Vehicle Classification dataset are corrupted with noise. This project addresses the problem of image denoising, aiming to enhance images by reducing noise and recovering clearer visuals. Effective denoising enables better vehicle classification and improves model accuracy.

---

## 📝 Problem Statement

Some images in the Emergency vs Non-Emergency Vehicle Classification dataset have been corrupted with noise. The goal is to convert these noisy images into clearer images with most (if not all) of the noise removed. We approach this as an image denoising problem using a convolutional autoencoder.

---

## 📊 Dataset

- **Clean images:** 1,999
- **Corrupt (noisy) images:** 353

The dataset contains two sets of images: **train** and **test**.
- The train set includes both clean images and their noisy counterparts.
- The test set consists of new images to evaluate the model’s performance.

---

## 📥 Data Download

You can download the dataset from the appropriate location (update with your actual dataset link or instructions).

---

## 🚗 Approach

1. The dataset is split into train and test sets.
2. **Training:** The autoencoder is trained using noisy images as input and clean images as output.
3. **Model Architecture:** A convolutional autoencoder is used to learn the denoising mapping.
4. **Evaluation:** The reconstructed images are compared to the clean images to compute the loss (e.g., MSE).
5. **Testing:** The trained model is applied to the test set to denoise new images.

### Model Workflow

1. **Input:** Noisy image
2. **Autoencoder Model:** Learns to map noisy to clean images
3. **Output:** Denoised (reconstructed) image

---

## 🔬 Results

Sample results comparing noisy test images and their denoised outputs:

| Noisy Test | Denoised Output |
|:----------:|:---------------:|
| ![noisy_sample](docs/noisy_sample.jpg) | ![denoised_sample](docs/denoised_sample.jpg) |

> _Replace the above example images with your own sample outputs._

---

## 🛠️ Usage

1. **Clone this repository:**
   ```bash
   git clone https://github.com/manola1109/-Emergency-vs-Non-Emergency-Vehicle-Image-Denoising.git
   cd -Emergency-vs-Non-Emergency-Vehicle-Image-Denoising
   ```

2. **Open and run the Jupyter notebook in Google Colab or locally:**
   - Follow the instructions in the notebook to train and evaluate the autoencoder.

3. **(Optional) Update dataset paths in the notebook as needed.**

---

## 📈 Evaluation

- Loss is computed as the difference between the reconstructed (denoised) image and the clean image.
- Metrics such as MSE, PSNR, or SSIM can be used for quantitative evaluation.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to open an issue or submit a pull request.

---

## 📄 License

This project is licensed under the MIT License.  
See the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- Inspired by real-world challenges in vehicle image classification.
- Dataset and task based on the Emergency vs Non-Emergency Vehicle Classification dataset.

