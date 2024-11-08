# brain-tumor predictor
A brain-tumor classifier. Classify a tumor as one of these types `glioma_tumor, meningioma_tumor, no_tumor, pituitary_tumor` applying classical machine techniques. The dataset has hundreds of images of an x-ray scan for individuals' head, whome might have a type of tumor in their brain.

# Example image
This is an example of an x-ray scan of a person's brain diagonsed with `glioma_tumor`, which is mostly malignant.

![giloma tumor](<Training/glioma_tumor/gg (1).jpg>)


# Tools
python, numpy, pandas, scikit-learn

# Techniques
- **Feature Engineering**: 
    - loaded images with a constant resolution size, so all images are loaded with equal resolutions.
    - Dimensionality Reduction: by removing RGB values for each pixel by a single value (whitness), since the x-ray images are inherently gray.
- **Normalization**: used *min-max* scaling technique to scale pixel values to a value between 0 and 1.
- **Principal Component Analysis (PCA)**: are used to minimze the number of features to a managable size while keeping most of the information/variation of the data.
- **GridSearch**: are used for tuning the *hyperparameters* of the model.
- **Confusion Matrix**: used to evaluate model performance on important metrics (i.e. *precision*, *recall*).
