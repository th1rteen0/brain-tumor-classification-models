# Brain Tumor Classification — Training Notebooks

This repository contains the Google Colab notebooks used to train and evaluate
the CNN models that power the
[Brain Tumor Classification Web App](https://github.com/th1rteen0/brain-tumor-classification-application).

---

## Notebooks

| Notebook | Description |
|---|---|
| `binary_classification.ipynb` | Trains a custom CNN to detect the presence or absence of a brain tumor |
| `multiclass_classification.ipynb` | Fine-tunes EfficientNetB1 to classify tumor type (glioma, meningioma, pituitary, none) with Grad-CAM explainability |

---

## Dataset

- **Source:** [Brain Tumor MRI Dataset — Kaggle](https://www.kaggle.com/datasets/masoudnickparvar/brain-tumor-mri-dataset)
- **Size:** 7,000+ labeled MRI images
- **Classes:** Glioma, Meningioma, Pituitary Tumor, No Tumor

---

## Model Performance

| Model | Architecture | Accuracy |
|---|---|---|
| Binary Classifier | Custom CNN | 97.02% |
| Multi-Class Classifier | EfficientNetB1 (fine-tuned) | 98.86% |

---

## How to Use

1. Open the desired notebook in [Google Colab](https://colab.research.google.com)
2. Connect to a GPU runtime (**Runtime → Change runtime type → T4 GPU**)
3. Mount your Google Drive or upload the dataset manually
4. Run all cells in order
5. The trained model will be exported as a `.keras` file — download it and:
   - For **local development**, place it in the `models/` directory of the web app
   - For **production**, upload it to your Amazon S3 bucket so the app can load it at runtime

---

## Tech Stack

- Python, TensorFlow / Keras
- EfficientNetB1 (ImageNet pre-trained, fine-tuned for multi-class)
- NumPy, Matplotlib, scikit-learn
- Grad-CAM via [VizGradCAM](https://github.com/gkeechin/vizgradcam)
- Google Colab (GPU-accelerated training)

---

## Research

This project is accompanied by an IEEE paper detailing the full methodology,
results, and clinical context.

📄 [Read the Paper](https://drive.google.com/file/d/1-Tr_ZdCki3MIbFk6pB3Z-5wmAxz0eSmh/view?usp=sharing)

---

## Related Repository

🔗 [Brain Tumor Classification Web App](https://github.com/th1rteen0/brain-tumor-classification-application)

---

## License

MIT License — see [LICENSE](LICENSE) for details.

---

𝑺𝑬𝑬 𝒀𝑶𝑼 𝑺𝑷𝑨𝑪𝑬 𝑪𝑶𝑾𝑩𝑶𝒀 . . .💫
