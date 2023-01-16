# flaggio
Hi!
This program takes an image input of a flag and returns to the user its best guess for what country it is.
The model uses fastai and was trained on a set of 30 images of each flag, pulled from ddg.
The actual learning model uses resnet50 (a 50 layer neural network) and is finetuned 5 times on the data.

The final product uses the gradio interface on huggingface and is available through this link:
https://huggingface.co/spaces/swemol/flaggo

Along with the name of the flag it also returns its "certainty" - this number varies from 0 to 1.
Certainties below 0.5 are often unreliable and usually arise when the image is highly distorted.