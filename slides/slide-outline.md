# Group 4 Slide Deck Outline

## Slide 1 – Cover

**Group 4 – L02 VGG16 Image Prediction Project**  
ITAI 2376 – Deep Learning

Using a pre-trained image-classification tool to learn what it does, why its workflow matters, and where its limits appear.

## Slide 2 – Introduction: What Are We Actually Using?

VGG16 is a pre-trained image classifier developed by Oxford's Visual Geometry Group. It became influential during the 2014 ImageNet era.

Key ideas:
- **Pre-trained** – learned from labeled images before we used it.
- **Classifier** – chooses among categories it already knows.
- **Preprocessing** – prepares an image in the size and numerical format the model expects.
- **Inference** – uses an already-trained model to make a prediction.

Our question: **How reliably does VGG16 recognize different kinds of images, and how sensitive are its predictions to rotation and noise?**

## Slide 3 – James Delgado: What I Expected vs. What VGG16 Saw

Test image: photograph of a young child sitting on a wooden crate.

Expectation: I expected the model to recognize the person or something close to the main subject.

Original top results:
1. sombrero – 23.13%
2. panpipe – 10.33%
3. cowboy hat – 5.61%

Learning point: VGG16 is not describing the whole scene. It is matching the image to categories it already learned.

## Slide 4 – James Delgado: What Changed and Why It Matters

75° rotation:
1. Band-Aid – 26.22%
2. bath towel – 25.89%
3. bib – 3.48%

Noise level 15:
1. panpipe – 17.32%
2. poncho – 17.10%
3. sombrero – 9.30%

Learning point: the image still looked like the same subject to me, but VGG16's predictions changed as the pixels changed. This gave me a practical understanding of **robustness**, meaning how consistently a model behaves when the input changes. A higher prediction score also did not mean a better answer.

## Slides 5–10 – Other Group Members

Each member follows the same two-slide pattern:

1. Expectation + original result + what was learned
2. Rotation/noise results + what changed + why it matters

## Final Slide – Group Conclusion

Compare:
- which image types VGG16 handled best or worst
- whether rotation or noise caused the larger change
- whether prediction scores changed even when labels stayed similar
- what the experiments taught us about preprocessing, robustness, and the limits of a pre-trained classifier

The final conclusion should be completed after all group members add their results.
