# James Delgado

## L02 Reflection Journal: Learning VGG16 as a Tool

When I started this lab, my goal was not to learn how to write VGG16 code. The notebook was given to us, so I focused on understanding the tool: what goes in, what it does, and what comes out. I learned that VGG16 is a pre-trained image classifier. Pre-trained means it learned from labeled images before I used it, and a classifier chooses among known categories. Knowing that VGG16 came from Oxford's Visual Geometry Group and became influential during the 2014 ImageNet era also helped me understand that it was built for a specific image-recognition task.

One first principle that made the workflow clearer is that the model does not see a photo the way I do. The image has to be preprocessed, meaning prepared in the size and numerical format VGG16 expects. Then I use the model for inference, meaning I am asking an already-trained model to make a prediction rather than teaching it something new. This changed my mental model from "AI looks at my picture" to "the tool compares a prepared image with patterns it learned before I arrived."

My test image was a photo of a young child sitting on a wooden crate. I expected the model to recognize the person, but its top prediction was sombrero at 23.13%. After a 75° rotation, the top prediction became Band-Aid at 26.22%. With a noise level of 15, panpipe became the top result at 17.32%. The image was still obviously the same to me, but the model's predictions changed as the pixels changed. This helped me understand robustness, meaning how consistently a model behaves when the input changes. I also learned that a higher prediction score does not necessarily mean a better answer.

Overall, this lab moved me from simply pressing a button and reading the result toward understanding what question the tool is actually answering. I did not write the program, and that was not the point. What mattered was learning what the model was built for, why preprocessing is needed, how to interpret its prediction scores, and where the tool can fail. That is the kind of understanding I want to keep building as we use more deep learning tools in this course.
