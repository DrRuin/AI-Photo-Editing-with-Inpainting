# AI-Photo-Editing-with-Inpainting 🎨✨
In this project we are going to build a little app that allows you to select a subject and then change its background, OR keep the background and change the subject.

## About the Project 📄

The process of this project involves a user uploading an image and selecting the main object by clicking on it. The Segment Anything Model (SAM) is activated to create a mask around the selected object, choosing the most accurate mask generated. The user is shown this result to either accept it or refine the mask further with additional points. Once the mask is finalized, the user gives a text description (and possibly a negative prompt) to specify a new background for the selected object. An infill model then creates this new background, and the final image is displayed. Optionally, the user can choose to invert the mask and substitute the subject while keeping the background, as in the example above.

## Implementations 🛠️

- Text2img GUI (Gradio)
- SAM Facebook Model (Base)
- Promptings
- Hyperparameters Modifications (To generate different outputs)

For a detailed look into the analysis, check out this [Jupyter Notebook](https://nbviewer.org/github/DrRuin/AI-Photo-Editing-with-Inpainting/blob/main/starter.ipynb)
