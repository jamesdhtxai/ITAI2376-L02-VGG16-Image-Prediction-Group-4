# James Delgado – VGG16 Image Test Results

## Test Image

A photograph of a young child sitting on a wooden crate.

## Original Image

1. sombrero – 23.13%
2. panpipe – 10.33%
3. cowboy hat – 5.61%

## Rotated 75°

1. Band-Aid – 26.22%
2. bath towel – 25.89%
3. bib – 3.48%

## Noise Level 15

1. panpipe – 17.32%
2. poncho – 17.10%
3. sombrero – 9.30%

## Observation

The image still looked like the same subject to me, but VGG16's predictions changed significantly when the orientation or pixel values changed. Rotation changed the prediction set more dramatically than the lighter noise. The rotated image also produced a higher top score than the original even though the label was not a useful description of the image. This showed me that a higher prediction score does not automatically mean a better answer.

## Main Learning Point

This test helped me understand **robustness**: how consistently a model behaves when the input changes. It also reinforced that VGG16 is a classifier choosing among ImageNet categories rather than describing the entire scene the way a person would.
