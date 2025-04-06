# Neural-Network-HW3

Autoencoder for MNIST Digit Reconstruction
This project implements a simple fully connected autoencoder using TensorFlow/Keras to reconstruct images from the MNIST dataset. The autoencoder compresses 28x28 grayscale images (flattened to 784-dimensional vectors) into a smaller latent space and learns to reconstruct them. \

Encoder: Reduces the input to a lower-dimensional representation (e.g., 32 units). \

Decoder: Reconstructs the original image from this compressed representation. \

Loss Function: Binary cross-entropy, optimized using Adam. \

Evaluation: Original vs. reconstructed digits are visualized to assess performance. \

We also analyze how changing the latent space size (e.g., 16, 32, 64) affects reconstruction quality and compression. \

