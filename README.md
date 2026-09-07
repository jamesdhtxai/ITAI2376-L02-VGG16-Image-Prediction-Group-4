# Group 4 – L02 VGG16 Image Prediction Project

ITAI 2376 – Deep Learning

## Project Purpose

This project uses a provided Google Colab notebook and the pre-trained VGG16 image-classification model as a learning tool. The goal is not to learn how to write the model code from scratch. Instead, we are learning how to use the tool and understand the **what and why** behind the workflow:

- What kind of input does VGG16 expect?
- Why does an image have to be preprocessed?
- What does a pre-trained model already know before we use it?
- What does a prediction score actually tell us?
- How much can the model's answer change when the image is rotated or has noise added?

## Shared Group Question

**How reliably does VGG16 recognize different kinds of images, and how sensitive are its predictions to rotation and noise?**

## Important Terms

- **VGG16** – A convolutional neural network created by Oxford's Visual Geometry Group for image classification.
- **Pre-trained** – The model learned from labeled images before we started using it.
- **Classifier** – A model that chooses among categories it already knows.
- **ImageNet** – The labeled image collection used to train this version of VGG16.
- **Preprocessing** – Preparing an image in the size and numerical format the model expects.
- **Inference** – Using an already-trained model to make a prediction rather than training it.
- **Prediction score** – A numerical score showing how strongly the model matched an image to a category. A higher score does not guarantee that the answer is correct.
- **Robustness** – How consistently a model behaves when the input changes.

## Group Method

Each group member will:

1. Choose a different type of image.
2. Upload the image to the provided Colab activity.
3. Record VGG16's original top predictions and scores.
4. Compare the same image after rotation and after noise is added.
5. Save screenshots of the results.
6. Create two slides focused on what was expected, what happened, and what was learned.
7. Add a short individual reflection.

For the shared group comparison, everyone should use the same settings:

- **Rotation:** 20°
- **Noise:** 20

Additional stronger tests can be included as optional exploration.

## James Delgado – Example Test

Test image: a photograph of a young child sitting on a wooden crate.

### Original
- sombrero – 23.13%
- panpipe – 10.33%
- cowboy hat – 5.61%

### 75° Rotation
- Band-Aid – 26.22%
- bath towel – 25.89%
- bib – 3.48%

### Noise Level 15
- panpipe – 17.32%
- poncho – 17.10%
- sombrero – 9.30%

The main learning point was that the image still looked like the same subject to a human, while VGG16's predictions changed significantly. This helped show the limits of the classifier and the importance of input presentation and robustness.

## Repository Structure

```text
.
├── README.md
├── PROJECT_PLAN.md
├── notebook/
│   └── README.md
├── slides/
│   └── README.md
├── results/
│   ├── group-results-template.md
│   └── james-delgado.md
└── reflections/
    └── james-delgado.md
```

The final Colab notebook, PowerPoint/Google Slides export, screenshots, and other group-member files can be added to these folders as the project is completed.

## Final Deliverables

- One combined reflective journal
- One group slide deck
- Individual results and contributions from each member
- Final filename: `L02_GroupName_ITAI2376`
