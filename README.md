# Autoencoder
Build an autoencoder model to learn, compress, and reconstruct the images of pullovers and dresses.
# Objective:
- Reconstruct images of pullover and dress using dimension reduction.
- Data preprocessing: Normalize the pixel values and reshape into a 4D array for each image sized as (28, 28, 1).
- Data concatenation: merged both train and test data for a unified split into 80% training, 10% validation, and 10% test sets.
- The base model consists of an encoder that compresses input images into a 128-dimensional latent space and a decoder to reconstruct the compressed images. The model is compiled utilizing the adam optimizer.
- Modifies the model to use transposed convolutional layers (Conv2Dtranspose) in the decoder model for improving the reconstruction images; also adds dropout to avoid overfitting.
- Evaluate the model using SSIM to determine whether the new images are similar compared to the input.
