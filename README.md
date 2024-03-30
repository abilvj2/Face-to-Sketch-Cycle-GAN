# Face-to-Sketch-Cycle-GAN
GAN network for converting real face images to artistic sketches


1. Model Architecture:
   - The first code snippet uses a simple generator model with dense and convolutional layers, while the second code snippet uses a more complex generator model with convolutional and upsampling layers.
   - The second code snippet also includes a discriminator model for adversarial training, while the first code snippet does not.

2. Preprocessing:
   - The first code snippet converts the input face images to grayscale using OpenCV's `cvtColor` function, while the second code snippet uses a combination of grayscale conversion, Gaussian blur, and image inversion.
   - The second code snippet also resizes the input images to (128, 128) dimensions.

3. Training Loop:
   - The first code snippet uses a custom training loop with manual optimization steps, while the second code snippet uses the `train_on_batch` method provided by Keras for training the discriminator and GAN models.
   - The second code snippet includes separate discriminator models for each direction of image translation (X to Y and Y to X).

4. Dataset Handling:
   - The first code snippet loads the face image dataset from a specified folder, while the second code snippet loads the dataset using the `train_test_split` function from scikit-learn.
   - The second code snippet also organizes the dataset into separate lists for input and output images.

5. Image Generation and Visualization:
   - Both code snippets generate and save images during training, but the second code snippet saves the generated images for both directions of image translation (X to Y and Y to X).

