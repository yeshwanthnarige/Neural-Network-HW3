# Neural-Network-HW3

# Autoencoder for MNIST Digit Reconstruction 

This project implements a simple fully connected autoencoder using TensorFlow/Keras to reconstruct images from the MNIST dataset. The autoencoder compresses 28x28 grayscale images (flattened to 784-dimensional vectors) into a smaller latent space and learns to reconstruct them. 

Encoder: Reduces the input to a lower-dimensional representation (e.g., 32 units). 

Decoder: Reconstructs the original image from this compressed representation. 

Loss Function: Binary cross-entropy, optimized using Adam. 

Evaluation: Original vs. reconstructed digits are visualized to assess performance. 

We also analyze how changing the latent space size (e.g., 16, 32, 64) affects reconstruction quality and compression. 

# Denoising Autoencoder for MNIST  

This model enhances the basic autoencoder by learning to remove Gaussian noise from images. The network is trained to reconstruct clean MNIST digits from noisy inputs.

Noise Added: Gaussian noise (mean=0, std=0.5).

Objective: Input = Noisy image, Output = Clean image.

Evaluation: Visual comparison of noisy input vs. denoised output.

Real-world Application:
Denoising autoencoders are widely used in medical imaging to remove artifacts and enhance scan clarity (e.g., MRI, CT scans), improving diagnosis accuracy.

# Character-Level Text Generation using LSTM
This project uses a Recurrent Neural Network (LSTM) to generate character-level text based on a training corpus (e.g., Shakespeare’s works).

Input: Sequences of 40 characters.

Target: The next character.

Model: LSTM followed by a softmax output over the character set.

Output: New text generated one character at a time.

 Temperature Scaling
Controls randomness in text generation:

Low temperature (e.g., 0.2) → more predictable, repetitive text.

High temperature (e.g., 1.0) → more creative, but possibly less coherent text.

# Sentiment Classification using LSTM (IMDB)
This project uses a Recurrent Neural Network (LSTM) to classify movie reviews from the IMDB dataset as either positive or negative.

Data: IMDB reviews (binary labels: 0 = negative, 1 = positive)

Preprocessing: Tokenization + Padding sequences to uniform length

Model: Embedding → LSTM → Dense(sigmoid)

Evaluation: Classification report and confusion matrix

⚖️ Why Precision-Recall Tradeoff Matters
Precision: Of all predicted positives, how many were actually positive?

Recall: Of all actual positives, how many were correctly predicted?

In sentiment analysis, this matters when:

Misclassifying a negative review as positive could lead to poor customer experience.

High recall ensures we detect most of the true positive sentiments, but we also want high precision to avoid falsely labeling negative reviews as positive.

Balancing both is crucial for trust in predictions.



