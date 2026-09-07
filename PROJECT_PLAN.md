# Group 4 Project Plan

## Goal

Use the provided VGG16 notebook as a tool to understand how a pre-trained image classifier behaves with different kinds of images and how its predictions change after rotation and noise.

## What Each Person Does

1. Choose one image type. James is using a photo of people. Everyone else should choose a different type of image so the group has something useful to compare.
2. Upload the image in Colab and record the original top 3 predictions and scores.
3. Run the shared comparison settings: **Rotation = 20°** and **Noise = 20**.
4. Save a screenshot showing the original, rotated, and noisy versions with the results.
5. Write a short reflection: What did you expect? What changed? What surprised you? What did you learn about VGG16 as a tool?
6. Create two slides using the same pattern:
   - Slide 1: expectation + original result + what you learned
   - Slide 2: rotation/noise results + what changed + why it matters

## Suggested Image Types

- James: people
- Member 2: clear common object
- Member 3: object with a busy background
- Member 4: drawing, unusual angle, blurry image, or another different image type

## What the Group Compares

- Which image types VGG16 handled best or worst
- Whether rotation or noise caused the bigger change
- Whether the prediction score changed even when a label stayed similar
- What the results suggest about preprocessing, robustness, and the limits of a pre-trained classifier

## Slide Deck Structure

1. Cover slide
2. Introduction: what VGG16 is and why we are using it
3. Two slides from each member
4. Group conclusion
5. Individual contributions

## Final Submission

- One combined reflective journal
- One group slide deck
- Clear individual contributions
- Final filename: `L02_GroupName_ITAI2376`
